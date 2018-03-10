# 阿卡信服务器快速搭建教程

## 两行命令拥有阿卡信服务器

通过我们发布的Docker镜像，可以最快速的完成服务器搭建工作，整个过程只需两行命令。

> 如果你没有Docker环境，请看下面的Docker一键安装教程。

````shell
# 请认准我们的官方镜像，无毒无害实时更新
docker pull registry.cn-qingdao.aliyuncs.com/akaxin/openzaly:latest

# hostBaseDir需要更改成你本地的绝对目录，服务器的日志、图片、数据库将存储在这个位置
docker run -tid -v hostBaseDir:/akaxin -p 2021:2021 registry.cn-qingdao.aliyuncs.com/akaxin/openzaly:latest

````

通过上面的两行命令安装完成后

````shell
docker ps -l
````

看到处于运行中的服务，代表程序运行成功，可以通过app访问站点。

## app访问站点

打开应用输入服务器地址，便可访问站点。初次访问的邀请码为000000，初次登录的用户默认为站点管理员。更详细的使用方法请参考：[APP使用简介](./how_to_login_site.md)

## 一键安装Docker教程

快速安装基于Docker，以下是Docker的一键安装教程，**如果你已经拥有Docker环境，请跳过**。

* [Linux](<demo.md>)
    * 直接通过yum、apt安装即可。
    * 或者访问：https://www.docker.com/community-edition#/download
* [Mac OSX](<https://store.docker.com/editions/community/docker-ce-desktop-mac>)
* [Windows Pro\Server](<https://store.docker.com/editions/community/docker-ce-desktop-windows>)


----

使用过程若有任何问题，欢迎联系我们 hi@akaxin.xyz