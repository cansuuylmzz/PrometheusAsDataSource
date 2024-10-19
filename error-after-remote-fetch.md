2024-10-19 10:47:16.535 [info] [main] Log level: Info
2024-10-19 10:47:16.535 [info] [main] Validating found git in: "git"
2024-10-19 10:47:16.535 [info] [main] Using git "2.46.2" from "git"
2024-10-19 10:47:16.536 [info] [Model][doInitialScan] Initial repository scan started
2024-10-19 10:47:16.536 [info] > git rev-parse --show-toplevel [4ms]
2024-10-19 10:47:16.536 [info] > git rev-parse --git-dir --git-common-dir [0ms]
2024-10-19 10:47:16.536 [info] [Model][openRepository] Opened repository: /workspaces/PrometheusAsDataSource
2024-10-19 10:47:16.536 [info] [Model][doInitialScan] Initial repository scan completed - repositories (1), closed repositories (0), parent repositories (0), unsafe repositories (0)
2024-10-19 10:47:16.536 [info] > git config --get commit.template [19ms]
2024-10-19 10:47:16.537 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [9ms]
2024-10-19 10:47:16.542 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:47:16.544 [info] > git rev-parse refs/remotes/origin/main [2ms]
2024-10-19 10:47:16.559 [info] > git status -z -uall [7ms]
2024-10-19 10:47:16.824 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [265ms]
2024-10-19 10:47:16.853 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [10ms]
2024-10-19 10:47:16.860 [info] > git config --local branch.main.vscode-merge-base [1ms]
2024-10-19 10:47:16.860 [warning] [Git][config] git config failed: Failed to execute git
2024-10-19 10:47:16.864 [info] > git config --get commit.template [12ms]
2024-10-19 10:47:16.873 [info] > git reflog main --grep-reflog=branch: Created from *. [9ms]
2024-10-19 10:47:16.880 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [10ms]
2024-10-19 10:47:16.885 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:47:16.885 [info] > git symbolic-ref --short refs/remotes/origin/HEAD [5ms]
2024-10-19 10:47:16.895 [info] > git rev-parse refs/remotes/origin/main [10ms]
2024-10-19 10:47:16.910 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/origin/main refs/remotes/origin/main [15ms]
2024-10-19 10:47:16.918 [info] > git status -z -uall [17ms]
2024-10-19 10:47:16.918 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [9ms]
2024-10-19 10:47:16.925 [info] > git config --local branch.main.vscode-merge-base origin/main [8ms]
2024-10-19 10:47:16.932 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [9ms]
2024-10-19 10:47:16.937 [info] > git config --get commit.template [6ms]
2024-10-19 10:47:16.940 [info] > git config --local branch.main.vscode-merge-base [4ms]
2024-10-19 10:47:16.956 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/origin/main refs/remotes/origin/main [9ms]
2024-10-19 10:47:16.972 [info] > git merge-base refs/heads/main refs/remotes/origin/main [12ms]
2024-10-19 10:47:16.977 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [22ms]
2024-10-19 10:47:16.980 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:47:16.980 [info] > git diff --name-status -z --diff-filter=ADMR 5f5541a0b0f8054f1839f63b36a1157030894f54...refs/remotes/origin/main [4ms]
2024-10-19 10:47:16.982 [info] > git rev-parse refs/remotes/origin/main [2ms]
2024-10-19 10:47:16.996 [info] > git status -z -uall [7ms]
2024-10-19 10:47:16.999 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [5ms]
2024-10-19 10:47:17.146 [info] > git check-ignore -v -z --stdin [3ms]
2024-10-19 10:47:18.915 [info] > git config --get commit.template [21ms]
2024-10-19 10:47:18.917 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [3ms]
2024-10-19 10:47:18.925 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:47:18.927 [info] > git rev-parse refs/remotes/origin/main [3ms]
2024-10-19 10:47:18.938 [info] > git status -z -uall [5ms]
2024-10-19 10:47:18.940 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [3ms]
2024-10-19 10:47:21.688 [info] > git config --local branch.main.github-pr-owner-number [194ms]
2024-10-19 10:47:21.688 [warning] [Git][config] git config failed: Failed to execute git
2024-10-19 10:47:49.883 [info] > git show --textconv :02-journeyDocker.md [7ms]
2024-10-19 10:47:49.887 [info] > git ls-files --stage -- /workspaces/PrometheusAsDataSource/02-journeyDocker.md [6ms]
2024-10-19 10:47:49.895 [info] > git cat-file -s aa020bac0ca9f37e8575d4c6491833692705b9ca [2ms]
2024-10-19 10:53:50.025 [info] > git check-ignore -v -z --stdin [1ms]
2024-10-19 10:53:50.408 [info] > git config --get commit.template [5ms]
2024-10-19 10:53:50.409 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 10:53:50.412 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:53:50.412 [info] > git rev-parse refs/remotes/origin/main [0ms]
2024-10-19 10:53:50.421 [info] > git status -z -uall [6ms]
2024-10-19 10:53:50.421 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 10:54:05.179 [info] > git check-ignore -v -z --stdin [1ms]
2024-10-19 10:54:05.683 [info] > git config --get commit.template [4ms]
2024-10-19 10:54:05.684 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 10:54:05.686 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:54:05.687 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 10:54:05.695 [info] > git status -z -uall [5ms]
2024-10-19 10:54:05.696 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 10:54:39.806 [info] > git config --get commit.template [1ms]
2024-10-19 10:54:39.811 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 10:54:39.814 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:54:39.814 [info] > git rev-parse refs/remotes/origin/main [0ms]
2024-10-19 10:54:39.821 [info] > git status -z -uall [4ms]
2024-10-19 10:54:39.822 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [1ms]
2024-10-19 10:55:06.282 [info] > git check-ignore -v -z --stdin [1ms]
2024-10-19 10:55:06.787 [info] > git config --get commit.template [4ms]
2024-10-19 10:55:06.788 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 10:55:06.791 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:55:06.792 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 10:55:06.799 [info] > git status -z -uall [4ms]
2024-10-19 10:55:06.800 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 10:56:08.403 [info] > git config --get commit.template [4ms]
2024-10-19 10:56:08.404 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 10:56:08.407 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:56:08.408 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 10:56:08.417 [info] > git status -z -uall [4ms]
2024-10-19 10:56:08.419 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 10:56:29.099 [info] > git check-ignore -v -z --stdin [2ms]
2024-10-19 10:56:29.609 [info] > git config --get commit.template [4ms]
2024-10-19 10:56:29.609 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 10:56:29.614 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:56:29.615 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 10:56:29.624 [info] > git status -z -uall [4ms]
2024-10-19 10:56:29.626 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 10:56:55.656 [info] > git config --get commit.template [4ms]
2024-10-19 10:56:55.657 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 10:56:55.660 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:56:55.661 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 10:56:55.669 [info] > git status -z -uall [5ms]
2024-10-19 10:56:55.669 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 10:57:06.958 [info] > git check-ignore -v -z --stdin [2ms]
2024-10-19 10:57:07.463 [info] > git config --get commit.template [5ms]
2024-10-19 10:57:07.464 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 10:57:07.467 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 10:57:07.468 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 10:57:07.476 [info] > git status -z -uall [5ms]
2024-10-19 10:57:07.476 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:19:22.160 [info] > git log --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%D%n%B -z --shortstat --diff-merges=first-parent -n50 --skip=0 --topo-order --decorate=full --stdin [16ms]
2024-10-19 11:20:21.903 [info] > git add -A -- . [9ms]
2024-10-19 11:20:21.913 [info] > git -c user.useConfigOnly=true commit --quiet --allow-empty-message --file - [6ms]
2024-10-19 11:20:21.917 [info] > git config --get commit.template [1ms]
2024-10-19 11:20:21.926 [info] > git config --get commit.template [3ms]
2024-10-19 11:20:21.926 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:20:21.930 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:20:21.931 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 11:20:21.938 [info] > git status -z -uall [4ms]
2024-10-19 11:20:21.940 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:20:22.301 [info] > git merge-base refs/heads/main refs/remotes/origin/main [355ms]
2024-10-19 11:20:22.341 [info] > git diff --name-status -z --diff-filter=ADMR 5f5541a0b0f8054f1839f63b36a1157030894f54...refs/remotes/origin/main [35ms]
2024-10-19 11:20:22.404 [info] > git log --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%D%n%B -z --shortstat --diff-merges=first-parent -n50 --skip=0 --topo-order --decorate=full --stdin [67ms]
2024-10-19 11:20:22.557 [info] > git push origin main:main [602ms]
2024-10-19 11:20:22.557 [info] To https://github.com/cansuuylmzz/PrometheusAsDataSource
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/cansuuylmzz/PrometheusAsDataSource'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
2024-10-19 11:20:22.561 [info] > git config --local branch.main.github-pr-owner-number [40ms]
2024-10-19 11:20:22.561 [warning] [Git][config] git config failed: Failed to execute git
2024-10-19 11:20:22.684 [info] > git config --get commit.template [59ms]
2024-10-19 11:20:22.725 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [23ms]
2024-10-19 11:20:22.736 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:20:22.739 [info] > git rev-parse refs/remotes/origin/main [4ms]
2024-10-19 11:20:22.768 [info] > git status -z -uall [11ms]
2024-10-19 11:20:22.771 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [3ms]
2024-10-19 11:20:22.905 [info] > git config --get commit.template [4ms]
2024-10-19 11:20:22.908 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [4ms]
2024-10-19 11:20:22.913 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:20:22.915 [info] > git rev-parse refs/remotes/origin/main [2ms]
2024-10-19 11:20:22.921 [info] > git status -z -uall [3ms]
2024-10-19 11:20:22.924 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [3ms]
2024-10-19 11:20:23.339 [info] > git ls-files --stage -- /workspaces/PrometheusAsDataSource/02-journeyDocker.md [1ms]
2024-10-19 11:20:23.344 [info] > git cat-file -s aa020bac0ca9f37e8575d4c6491833692705b9ca [2ms]
2024-10-19 11:20:23.432 [info] > git show --textconv :02-journeyDocker.md [2ms]
2024-10-19 11:21:40.910 [info] > git check-ignore -v -z --stdin [2ms]
2024-10-19 11:21:41.413 [info] > git config --get commit.template [4ms]
2024-10-19 11:21:41.415 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 11:21:41.423 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:21:41.423 [info] > git rev-parse refs/remotes/origin/main [0ms]
2024-10-19 11:21:41.431 [info] > git status -z -uall [5ms]
2024-10-19 11:21:41.431 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [1ms]
2024-10-19 11:21:55.701 [info] > git check-ignore -v -z --stdin [1ms]
2024-10-19 11:21:56.205 [info] > git config --get commit.template [4ms]
2024-10-19 11:21:56.206 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:21:56.209 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:21:56.210 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 11:21:56.219 [info] > git status -z -uall [6ms]
2024-10-19 11:21:56.220 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:23:28.682 [info] > git check-ignore -v -z --stdin [1ms]
2024-10-19 11:23:28.983 [info] > git show --textconv :error-samblance [5ms]
2024-10-19 11:23:28.984 [info] > git ls-files --stage -- /workspaces/PrometheusAsDataSource/error-samblance [1ms]
2024-10-19 11:23:31.345 [info] > git config --get commit.template [3ms]
2024-10-19 11:23:31.346 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:23:31.350 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:23:31.351 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 11:23:31.359 [info] > git status -z -uall [5ms]
2024-10-19 11:23:31.359 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:23:45.157 [info] > git show --textconv :error-Samblence.md [4ms]
2024-10-19 11:23:45.158 [info] > git ls-files --stage -- /workspaces/PrometheusAsDataSource/error-Samblence.md [1ms]
2024-10-19 11:23:45.315 [info] > git check-ignore -v -z --stdin [1ms]
2024-10-19 11:23:45.819 [info] > git config --get commit.template [4ms]
2024-10-19 11:23:45.820 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:23:45.823 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:23:45.824 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 11:23:45.831 [info] > git status -z -uall [4ms]
2024-10-19 11:23:45.832 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:23:58.604 [info] > git config --get commit.template [4ms]
2024-10-19 11:23:58.605 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 11:23:58.608 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:23:58.609 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 11:23:58.620 [info] > git status -z -uall [7ms]
2024-10-19 11:23:58.622 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [3ms]
2024-10-19 11:27:22.156 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 11:27:22.156 [info] > git config --get commit.template [6ms]
2024-10-19 11:27:22.159 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/workspaces/PrometheusAsDataSource/.git/refs/remotes/origin/main'
2024-10-19 11:27:22.160 [info] > git rev-parse refs/remotes/origin/main [1ms]
2024-10-19 11:27:22.167 [info] > git status -z -uall [4ms]
2024-10-19 11:27:22.168 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [1ms]
2024-10-19 11:27:50.355 [info] > git config --get commit.template [2ms]
2024-10-19 11:27:50.359 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:27:50.366 [info] > git status -z -uall [4ms]
2024-10-19 11:27:50.368 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:27:50.375 [info] > git merge-base refs/heads/main refs/remotes/origin/main [1ms]
2024-10-19 11:27:50.379 [info] > git diff --name-status -z --diff-filter=ADMR 5f5541a0b0f8054f1839f63b36a1157030894f54...refs/remotes/origin/main [1ms]
2024-10-19 11:27:50.449 [info] > git config --local branch.main.github-pr-owner-number [1ms]
2024-10-19 11:27:50.449 [warning] [Git][config] git config failed: Failed to execute git
2024-10-19 11:27:52.426 [info] > git config --get commit.template [4ms]
2024-10-19 11:27:52.427 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:27:52.435 [info] > git status -z -uall [5ms]
2024-10-19 11:27:52.435 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [1ms]
2024-10-19 11:27:52.839 [info] > git ls-files --stage -- /workspaces/PrometheusAsDataSource/error-Samblence.md [2ms]
2024-10-19 11:27:53.045 [info] > git show --textconv :error-Samblence.md [1ms]
2024-10-19 11:28:34.986 [info] > git log --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%D%n%B -z --shortstat --diff-merges=first-parent -n50 --skip=0 --topo-order --decorate=full --stdin [4ms]
2024-10-19 11:29:04.197 [info] > git add -A -- . [9ms]
2024-10-19 11:29:04.205 [info] > git -c user.useConfigOnly=true commit --quiet --allow-empty-message --file - [5ms]
2024-10-19 11:29:04.208 [info] > git config --get commit.template [0ms]
2024-10-19 11:29:04.215 [info] > git config --get commit.template [3ms]
2024-10-19 11:29:04.216 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [1ms]
2024-10-19 11:29:04.225 [info] > git status -z -uall [5ms]
2024-10-19 11:29:04.227 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [3ms]
2024-10-19 11:29:04.365 [info] > git merge-base refs/heads/main refs/remotes/origin/main [131ms]
2024-10-19 11:29:04.372 [info] > git diff --name-status -z --diff-filter=ADMR 5f5541a0b0f8054f1839f63b36a1157030894f54...refs/remotes/origin/main [2ms]
2024-10-19 11:29:04.516 [info] > git log --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%D%n%B -z --shortstat --diff-merges=first-parent -n50 --skip=0 --topo-order --decorate=full --stdin [6ms]
2024-10-19 11:29:04.546 [info] > git config --local branch.main.github-pr-owner-number [1ms]
2024-10-19 11:29:04.546 [warning] [Git][config] git config failed: Failed to execute git
2024-10-19 11:29:04.588 [info] > git push origin main:main [349ms]
2024-10-19 11:29:04.588 [info] To https://github.com/cansuuylmzz/PrometheusAsDataSource
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/cansuuylmzz/PrometheusAsDataSource'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
2024-10-19 11:29:04.598 [info] > git config --get commit.template [4ms]
2024-10-19 11:29:04.602 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 11:29:04.609 [info] > git status -z -uall [4ms]
2024-10-19 11:29:04.610 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [1ms]
2024-10-19 11:29:04.820 [info] > git config --get commit.template [6ms]
2024-10-19 11:29:04.822 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/main refs/remotes/main [2ms]
2024-10-19 11:29:04.829 [info] > git status -z -uall [3ms]
2024-10-19 11:29:04.831 [info] > git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname) [2ms]
2024-10-19 11:29:05.681 [info] > git ls-files --stage -- /workspaces/PrometheusAsDataSource/error-Samblence.md [1ms]
2024-10-19 11:29:05.685 [info] > git cat-file -s b51490816a831834cb06c5b5087ad7308b789f91 [1ms]
2024-10-19 11:29:05.802 [info] > git show --textconv :error-Samblence.md [2ms]


---------------------------------------

It looks like you're looking for `git rebase` commands. Here’s a quick overview of some common rebase commands and scenarios:

### Basic Git Rebase Commands

1. **Start a Rebase:**
   ```bash
   git rebase <base_branch>
   ```
   This rebases your current branch onto `<base_branch>`.

2. **Continue After a Conflict:**
   If conflicts occur during the rebase, resolve them and then run:
   ```bash
   git rebase --continue
   ```

3. **Skip a Commit:**
   If you want to skip a commit during the rebase, use:
   ```bash
   git rebase --skip
   ```

4. **Abort a Rebase:**
   If you want to stop the rebase process and return to the state before starting it, run:
   ```bash
   git rebase --abort
   ```

5. **Interactive Rebase:**
   To edit, reorder, or squash commits, you can use:
   ```bash
   git rebase -i <base_branch>
   ```
   This opens an interactive editor where you can specify how to handle each commit.

### Example Use Cases

- **Rebase Current Branch with Master:**
   ```bash
   git checkout feature-branch
   git rebase master
   ```

- **Squash Commits in Interactive Rebase:**
   ```bash
   git checkout feature-branch
   git rebase -i HEAD~3
   ```
   This will allow you to modify the last 3 commits.

### Notes on Rebasing
- Rebasing rewrites commit history, so be cautious when using it on public branches.
- Always make sure your working directory is clean (i.e., commit or stash any changes) before starting a rebase.

Let me know if you need more specific information or examples!