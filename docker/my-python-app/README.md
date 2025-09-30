- 下記サイトを参考
https://zenn.dev/joho0724/articles/sankaku0724-newcreate31

- dockerイメージを作成
```shell
docker build -t my-python-app .

# イメージが作成できたことを確認
$ docker image ls
REPOSITORY                    TAG        IMAGE ID       CREATED          SIZE
my-python-app                 latest     915c864513cc   19 seconds ago   120MB
gcr.io/k8s-minikube/kicbase   v0.0.48    c6b5532e987b   3 weeks ago      1.31GB
python                        3.9-slim   56cea0119ab6   7 weeks ago      120MB
```

- 実際にコンテナを起動
```shell
# 起動するコマンド
docker run my-python-app
hello, Docker!

# 起動したコンテナを確認する
docker ps -a
CONTAINER ID   IMAGE                                 COMMAND                  CREATED         STATUS            
           PORTS                                                                                                
                                  NAMES
9c2e0ab6d206   my-python-app                         "python app.py"          3 minutes ago   Exited (0) 3 minutes ago 
```