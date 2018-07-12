# Nvidia-Docker-Command
Nvidia Dockerでコンテナを作成した時に、まずセットアップする内容です<br>
<br>
コンテナの作成↓
```
$ nvidia-docker run -it --name "name" nvidia/cuda:8.0-cudnn7-devel-ubuntu16.04
```
コンテナの削除↓
```
$ nvidia-docker rm "name"
```
コンテナ一覧↓
```
$ nvidia-docker ps -a
```
起動↓
```
$ nvidia-docker start -i "name"
```
ログイン↓
```
$ nvidia-docker attach "name"
```
動作を止める↓
```
$ nvidia-docker stop "name"
```
デタッチ↓
```
ctrl+p+q　（キーボード同時押し）
```

環境作成後↓
```
$ apt-get update
$ apt-get install python-pip
$ apt-get install vim
```
