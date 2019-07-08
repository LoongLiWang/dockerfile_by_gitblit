## gitblit 构建


## docker pull 镜像
```bash
# docker pull docker.io/2859413527/gitblit
```

## 运行容器
```bash
# docker run -d --restart=always --name gitblit-server -p 9010:9010 -p 29418:29418 -v /git:/git docker.io/2859413527/gitblit
```

此时，可以通过浏览器 ip:9010 进行访问了，默认用户名和密码为 admin:admin


## 其他
如果在运行docker容器时，需要将git目录通过-v给映射出来时，需要考虑selinux的因素，测试时关闭selinux
```bash
# setenforce 0
```

