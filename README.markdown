## gitblit build


## docker pull image

```bash
# docker pull docker.io/2859413527/gitblit
```

## Run container

```bash
# docker run -d --restart=always --name gitblit-server -p 9010:9010 -p 29418:29418 -v /git:/git docker.io/2859413527/gitblit
```
Now, you can access it through the browser ip:9010, the default username and password are admin:admin

## Other

If you need to map the git directory to -v when running the docker container, you need to consider the selinux factor, and shut down selinux during the test.

```bash
# setenforce 0
```


