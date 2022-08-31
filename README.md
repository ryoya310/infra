# 使用方法

docker compose up -d

[http://localhost:3000](http://localhost:3000)


イメージ全削除
docker rmi $(docker images -q) -f

コンテナ全削除
docker rm $(docker ps -a -q) -f

不要物一括削除
docker system prune

再ビルド キャッシュ削除
docker-compose build --no-cache