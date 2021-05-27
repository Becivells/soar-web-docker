# soar-web docker 自动生成仓库
[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/becivells/soar-web-docker/Publish%20Releases%20to%20Hub)](https://github.com/Becivells/soar-web-docker/actions)
[![GitHub last commit](https://img.shields.io/github/last-commit/xiaomi/soar?label=soar%20commit)](https://github.com/XiaoMi/soar)
[![GitHub last commit](https://img.shields.io/github/last-commit/xiyangxixian/soar-web?label=soar-web%20commit)](https://github.com/xiyangxixian/soar-web)
[![GitHub last commit](https://img.shields.io/github/last-commit/becivells/soar-web-docker?label=soar-web%20docker%20commit)](https://github.com/Becivells/soar-web-docker)
[![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/becivells/soar-web-docker)](https://github.com/Becivells/soar-web-docker/tags)
[![Docker Pulls](https://img.shields.io/docker/pulls/becivells/soar-web)](https://hub.docker.com/r/becivells/soar-web/)  
地址：[https://hub.docker.com/r/becivells/soar-web/](https://hub.docker.com/r/becivells/soar-web/)   
使用 `github action` 生成docker 镜像并且自动推送给 `DockerHub`

|                  版本                   |                        使用的soar版本                        |                      使用的soar-web版本                      |                           镜像大小                           |
| :-------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `docker pull becivells/soar-web:latest` | 2021/05/27-[a5cb33b](https://github.com/XiaoMi/soar/commit/a5cb33b98f86ab92f99ea611409c3a280036cf07) | 2021/05/27-[a5cb33b](https://github.com/XiaoMi/soar/commit/a5cb33b98f86ab92f99ea611409c3a280036cf07) | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/latest) |
| `docker pull becivells/soar-web:2.0.7`  | 2021/05/27-[a5cb33b](https://github.com/XiaoMi/soar/commit/a5cb33b98f86ab92f99ea611409c3a280036cf07) | 2021/05/27-[a5cb33b](https://github.com/XiaoMi/soar/commit/a5cb33b98f86ab92f99ea611409c3a280036cf07) | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/2.0.7) |
| `docker pull becivells/soar-web:2.0.6`  | 2021/05/26-[9a47ddc](https://github.com/XiaoMi/soar/commit/9a47ddc1089f6a32fbc37d2c5e96216cd885eb3a) | 2020/12/01-[cdde5ef](https://github.com/xiyangxixian/soar-web/commit/cdde5effcbe35c912d53f4c90ae1742887cfbc10) | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/2.0.6) |
| `docker pull becivells/soar-web:2.0.5`  | 2021/05/19-[dd44876](https://github.com/XiaoMi/soar/commit/dd44876e6b4d154594886fb84c44e2c9b60db7b2) | 2020/12/01-[cdde5ef](https://github.com/xiyangxixian/soar-web/commit/cdde5effcbe35c912d53f4c90ae1742887cfbc10) | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/2.0.5) |
| `docker pull becivells/soar-web:2.0.4`  | 2021/04/30-[54e106c](https://github.com/XiaoMi/soar/commit/54e106ca4a380bbd6f70af1bf9a502258fca7810) | 2020/12/01-[cdde5ef](https://github.com/xiyangxixian/soar-web/commit/cdde5effcbe35c912d53f4c90ae1742887cfbc10) | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/2.0.4) |
| `docker pull becivells/soar-web:2.0.3`  | 2021/03/22-[d0d0ce5](https://github.com/XiaoMi/soar/commit/d0d0ce57c9036f7e2e4c5a506e131ce42b332550) | 2020/12/01-[cdde5ef](https://github.com/xiyangxixian/soar-web/commit/cdde5effcbe35c912d53f4c90ae1742887cfbc10) | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/2.0.3) |
| `docker pull becivells/soar-web:1.0.0`  |                      2019/01/05-g552ccf                      |                      2019/01/05-g552ccf                      | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/becivells/soar-web/1.0.0) |



Dockerfile 见根目录 Dockerfile 文件

```shell script
docker pull becivells/soar-web
docker run -d --name soar-web -p 5077:5077 becivells/soar-web
```

**也可以使用 Dockerfile 自行构建**

```shell script
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

