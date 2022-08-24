# 使用方法

docker compose up -d

cd htdocs

## コマンド一覧

### フォルダ作成

mkdir docker/mysql/store

### ファイル作成

type nul > htdocs/index.html

### ファイルに書込

echo "Hello World" > htdocs/index.html

### 削除

Remove-Item -Recurse -Force -Path htdocs/index.html

### 再ビルド

docker-compose down && docker-compose build && docker-compose up -d

### イメージ全削除

docker rmi $(docker images -q) -f

### コンテナ全削除

docker rm $(docker ps -a -q) -f

### 不要物一括削除

docker system prune
