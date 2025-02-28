CMD Docker
--------


## Lệnh xóa toàn bộ Docker để làm sạch hoàn toàn

```
docker rm -f $(docker ps -aq)
docker rmi -f $(docker images -aq)
docker builder prune -a -f
docker volume rm $(docker volume ls -q)

```

## Chạy container từ image vừa build

```
docker run --rm -it <name-images> bash

```

## Docker build

```
docker build --no-cache -t <name-images> .
```






