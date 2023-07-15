# httpwaf

#### 一 、介绍
httpwaf是一款永久免费的web应用防火墙，专注未知攻击对抗，也可以开源，是业界最好用的waf。

#### 二、承诺和不承诺
承诺：为了保证服务器安全，除首次安装，任何时候绝不联网，大量实战稳定可靠。

不承诺：无论任何原因引发的任何问题，都不负任何责任；请务必在测试环境完美演练后，再谨慎部署到生产环境。

注意：WEB管理9999端口禁止向公网开放，或者严格设置IP白名单访问权限。

#### 三 、两种安装架构
##### 1、直接安装在WEB服务器上

​    服务器原HTTP端口80改为其他如81，原HTTPS端口443改为4433，然后WAF占用80、443即可。

    WAF（80)<------------->127.0.0.1:81
    WAF（443)<------------>127.0.0.1:4433

##### 2、独立部署，反向代理WEB服务器

    WAF（80)<------------->WEB服务器:80
    WAF（443)<------------>WEB服务器:443


#### 四、安装步骤
支持Linux x86 64位系统，保证可以上网，并且80、443和9999端口没有被占用，以root权限运行下面命令：

    1、  wget http://59.110.1.135/himonitor
    2 、 chmod +x ./himonitor
    3 、 ./himonitor

首次安装下载大约半分钟，出现System is running.....代表安装成功，可以WEB管理口9999（防火墙允许）登录进去。

#### 五、运行停止卸载
启动运行:  ./himonitor         后台模式运行:   ./himonitor daemon

停止运行:  ./himonitor stop    卸载 :   rm  /hihttps/ -rf

默认没加开机启动，请自行把himonitor加入开机启动程序。

#### 六、免费演示地址

实战地址 [http://59.110.1.135/httpwaf/](http://59.110.1.135/httpwaf/)

#### 七、付费演示地址

httpwaf单机版永远免费，但开放源码、分布式集中管控、技术支持、功能增加等要收费。请用大屏电脑观看，首次加载大屏组件需要10秒：
攻击态势大屏 [http://59.110.1.135/atkmap.html](http://59.110.1.135/atkmap.html)
集中管控大屏 [http://59.110.1.135/center.html](http://59.110.1.135/center.html)

#### 八、源码部署请加微信号httpwaf

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/wechat.png)

#### 九、来一张首页图片

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/home.png)
