CMD Docker
--------


## Lệnh xóa toàn bộ Docker để làm sạch hoàn toàn

```
docker rm -f $(docker ps -aq)
docker rmi -f $(docker images -aq)
docker builder prune -a -f
docker volume rm $(docker volume ls -q)

```

## Docker build

```
docker build --no-cache -t <name-images> .
```
VD:
```
docker build --no-cache -t snipeit-build .
```

## Chạy container từ image vừa build

```
docker run --rm -it <name-images> bash

```


## Kiểm tra cổng 8888

```
sudo lsof -i :8888
```

## Mở cổng kết nối

```
sudo ufw allow 8888
sudo ufw reload
```






