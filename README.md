# jupyterlab-env

## 概要
dockerを使ってjupyterlabを使える環境を構築するやつ

## 現状入ってるpythonライブラリ
- jupyterlabに入ってるもの
- tensorflow(CPU版)
- keras
- opencv-python

削除・追加したい場合はrequirements.txtを編集する

## 使用方法
1. `$ git clone https://github.com/ur0o/jupyterlab-env && cd jupyterlab-env`
1. `$ docker-compose build`
1. `$ docker-compose up`
1. ブラウザで`http://localhost:8888`にアクセス


## その他
- workspaceディレクトリをマウントしてるので、そこ以下のディレクトリのみjupyterで展開される
    - datasets: データセットを格納するディレクトリ。
    - notebooks: .ipynbファイルはここでやる感じにする。