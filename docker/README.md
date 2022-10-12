# docker

### 修改vm.max_map_count
```
# Linux:
/etc/sysctl.conf
# 添加 vm.max_map_count = 262144，如果已存在就修改，数值不能低于262144
sudo sysctl -p

# Windows cmd:
wsl -d docker-desktop
sysctl -w vm.max_map_count=262144
```

### kcompose: 将docker-compose迁移到k8s
```
kompose convert
```