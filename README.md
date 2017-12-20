# workerman-docker
workerman框架的docker版本

## 启动
Docker 对外暴露7272端口
挂载目录必须包括webapp子目录，启动文件为webapp下面的start.php

```
docker run -d -p 7272:7272 -v /mnt/workerman-chat-dev:/var/www  --name workerman-dev wisdombud/workerman:latest sh
```

## 构建镜像
```
docker build -t RoonyLi/workerman .
```