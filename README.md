# kubernetes学習
minikubeを使ってクラスタを構築していく。
AWS EKSのクラスタなどは費用が莫大なため、OSSリソースを使用する。

https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable
上記を参考にminikubeをインストールする。

### 前提
インストールしておくもの
- docker
イメージを格納するレジストリなどで必要
- kubectl
クラスタ操作に必要なコマンドが格納されている。
*それぞれパスを通しておくと便利。人によってはaliasコマンドでkubectl="k"にする人もいる。