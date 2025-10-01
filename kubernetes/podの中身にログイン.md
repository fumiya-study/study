# podにログインする方法
kubectl exec -it sample-pod -- bash

```shell
$ kubectl exec -it sample-pod -- bash
root@sample-pod:/# ls
bin  boot  dev  etc  home  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
```

## コマンドを直接指定することもできる
```shell
$ kubectl exec -it sample-pod -- ls
bin   dev  home  lib64  mnt  proc  run   srv  tmp  var
boot  etc  lib   media  opt  root  sbin  sys  usr
```