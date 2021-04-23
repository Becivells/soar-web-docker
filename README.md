# soar-web docker 自动生成仓库
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/becivells/soar-web-docker/Publish%20Releases%20to%20Hub) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/becivells/soar-web-docker) ![Docker Pulls](https://img.shields.io/docker/pulls/becivells/soar-web)   
地址：[https://hub.docker.com/r/becivells/soar-web/](https://hub.docker.com/r/becivells/soar-web/)   
使用 `github action` 生成docker镜像并且自动推送给 `DockerHub`

| 版本信息 | soar版本                                                     | soar-web版本                                                 | 说明                                    |
| -------- | ------------------------------------------------------------ | ------------------------------------------------------------ | --------------------------------------- |
| Latest   | 2021/03/22-[d0d0ce5](https://github.com/XiaoMi/soar/commit/d0d0ce57c9036f7e2e4c5a506e131ce42b332550) | 2020/12/01-[cdde5ef](https://github.com/xiyangxixian/soar-web/commit/cdde5effcbe35c912d53f4c90ae1742887cfbc10) | `docker pull becivells/soar-web:latest` |
| V2.0.3   | 2021/03/22-[d0d0ce5](https://github.com/XiaoMi/soar/commit/d0d0ce57c9036f7e2e4c5a506e131ce42b332550) | 2020/12/01-[cdde5ef](https://github.com/xiyangxixian/soar-web/commit/cdde5effcbe35c912d53f4c90ae1742887cfbc10) | `docker pull becivells/soar-web:v2.0.3` |
| v1.0.0   | 2019/01/05-g552ccf9                                          | 2019/01/05-g552ccf9                                          | `docker pull becivells/soar-web:v1.0.0` |

Dockerfile 见根目录 Dockerfile 文件

```
docker pull becivells/soar-web
docker run -d --name soar-web -p 5077:5077 becivells/soar-web
```

**也可以使用 Dockerfile 自行构建**

```
docker build --no-cache -t soar-web .
```

**访问**

在浏览器上输入 [http://127.0.0.1:5077](http://127.0.0.1:5077/) 进行访问。

## 参考链接

[build-push-action](https://github.com/docker/build-push-action)    
[docker-action-examples](https://github.com/metcalfc/docker-action-examples/)    
[soar-web](https://github.com/xiyangxixian/soar-web)     
[soar](https://github.com/XiaoMi/soar)
[github action - publishing-docker-images](https://docs.github.com/cn/actions/guides/publishing-docker-images)

