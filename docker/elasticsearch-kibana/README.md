# elasticsearch-kibana

### 进入docker目录
```
$ cd ./document/docker/elasticsearch-kibana
```

### 启动容器
```
$ docker-compose up -d
```

### 浏览器打开kibana
```
http://localhost:5601
```

### 进入elasticsearch容器
```
$ docker container exec -it [containerID] /bin/bash
```

### 获取elasticsearch的kibana令牌
```
$ ./bin/elasticsearch-create-enrollment-token --scope kibana
```

### 设置账号密码
```
$ ./bin/elasticsearch-setup-passwords interactive
```
