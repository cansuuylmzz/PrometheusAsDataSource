Minikube kullanarak bir Kubernetes kümesi oluşturup, Helm ile Prometheus, Grafana ve Thanos'u kurarak izleme ve metriklerin uzun süreli saklanmasını sağlamak harika bir yöntemdir. Bu adım adım kurulum rehberi, bu araçları nasıl yapılandıracağınızı anlatır.

### Gereksinimler
- [Minikube](https://minikube.sigs.k8s.io/docs/start/) kurulmuş olmalı.
- [Helm](https://helm.sh/docs/intro/install/) kurulmuş olmalı.
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/) kurulmuş olmalı.

### Adım 1: Minikube Başlat
Minikube kümesini başlatmak için şu komutu kullanın:
```bash
minikube start
```

Kümenin çalışıp çalışmadığını doğrulamak için:
```bash
minikube status
```

### Adım 2: Helm Depolarını Ekle
Helm ile Prometheus, Grafana ve Thanos için gerekli Helm depolarını ekleyin:

```bash
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo add grafana https://grafana.github.io/helm-charts
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update
```

### Adım 3: Helm ile Prometheus Kurulumu
Prometheus'u kurmak için şu komutu çalıştırın:
```bash
helm install prometheus prometheus-community/kube-prometheus-stack
```

Kurulumdan sonra, Prometheus podlarının çalışıp çalışmadığını kontrol edin:
```bash
kubectl get pods -n default
```

### Adım 4: Helm ile Grafana Kurulumu
Grafana’yı izleme için kurmak amacıyla şu komutu kullanın:
```bash
helm install grafana grafana/grafana --set persistence.storageClass="standard" --set adminPassword='admin' --values https://raw.githubusercontent.com/grafana/helm-charts/main/charts/grafana/values.yaml
```

Grafana admin şifresini almak için:
```bash
kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo
```

Grafana servisine erişmek için port yönlendirme yapın:
```bash
kubectl port-forward service/grafana 3000:80
```

Tarayıcınızdan `http://localhost:3000` adresine giderek Grafana'ya erişebilirsiniz.

### Adım 5: Thanos Kurulumu
Prometheus verilerini uzun süreli saklamak için Thanos'u Helm ile kurun:
```bash
helm install thanos bitnami/thanos --set service.type=LoadBalancer
```

### Adım 6: Thanos Sidecar Kurulumu
Prometheus’u Thanos ile entegre etmek için **Thanos Sidecar**’ı yapılandırmanız gerekir. Prometheus dağıtımını düzenleyip aşağıdaki gibi Thanos sidecar ekleyin:

```yaml
- name: thanos-sidecar
  image: quay.io/thanos/thanos:latest
  args:
    - sidecar
    - --prometheus.url=http://localhost:9090
    - --grpc-address=0.0.0.0:10901
    - --http-address=0.0.0.0:10902
```

Bu yapılandırmadan sonra Prometheus podlarını yeniden başlatın.

### Adım 7: Thanos Sorgu Aracını (Querier) Kurun
Thanos sorgulayıcısını kurarak farklı Prometheus instance'larından verileri toplayın:
```bash
helm install thanos-querier bitnami/thanos --set component=query
```

Thanos sorgulayıcıyı erişime açın:
```bash
kubectl port-forward service/thanos-querier 9091:10902
```

### Adım 8: Grafana’yı Thanos ile Bağlayın
Grafana üzerinde Thanos’u veri kaynağı olarak ekleyin:
- **Configuration > Data Sources > Add Data Source**'a gidin.
- **Prometheus** seçin.
- URL olarak `http://localhost:9091` girin.
- **Save & Test** diyerek kaydedin.

Bu adımlarla, Grafana üzerinden Thanos aracılığıyla uzun süreli metriklerinizi görüntüleyebilirsiniz.

### Örnek Senaryolar

- **Senaryo 1**: Pod'ların CPU ve bellek kullanımını Prometheus ile izleyin ve Grafana’da bu verileri grafik olarak görün.
- **Senaryo 2**: Thanos ile farklı Kubernetes kümelerindeki metrik verilerini toplayın ve merkezi bir izleme çözümü oluşturun.

---

Bu kurulum rehberi ile Minikube Kubernetes kümesi üzerinde Prometheus, Grafana ve Thanos kullanarak izleme ve uzun süreli veri saklama çözümü oluşturabilirsiniz.