###### 安装

1. 根据官网步骤进行安装  
   [https://docs.docker.com/engine/install/centos/](https://docs.docker.com/engine/install/centos/)   
   *注意docker-ce国内下载缓慢，可使用阿里镜像加速服务*
   *[https://developer.aliyun.com/mirror/](https://developer.aliyun.com/mirror/)*


2. 安装完成后使用华为云（阿里云）docker镜像加速服务提升下载速度。
   *[https://console.huaweicloud.com/swr/?region=cn-east-3#/app/swr/huaweiOfficialList](https://console.huaweicloud.com/swr/?region=cn-east-3#/app/swr/huaweiOfficialList)*

###### 说明

[http://www.dockerinfo.net/document](http://www.dockerinfo.net/document)

- 容器化技术
- 数据隔离，网络隔离
- 使用统一文件系统，是以读写方式挂载
- [docker-compose:docker统一管理工具](http://www.dockerinfo.net/docker-compose-%e9%a1%b9%e7%9b%ae)

``` 
services:
  mongo1:
    image: mongo
    ports:
      - 38001:27017

  mongo2:
    image: mongo
    ports:
      - 38002:27017
```
