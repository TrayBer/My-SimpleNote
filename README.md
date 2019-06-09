# ◇ 浏览器在线代理

项目页面：https://github.com/EtherDream/jsproxy

代理演示页面：https://jsproxy.ga/

Google 搜索：https://jsproxy.ga/-----https://www.google.com

# ◇ SS/SSR 服务商列表

供应商列表及测速：https://github.com/DuyaoSS/SSR/issues/2

# ◇ Shadowsocks 服务GCP搭建

1）创建实例，地区选择台湾，防火墙同时选中「允许 HTTP 流量」、「允许 HTTPS 流量」，其它默认；

2）创建防火墙规则，添加出站、入站需要的TCP相应端口规则，例如端口443；

3）在浏览器新窗口打开SSH连接；

4）安装shadowsocks服务：

a. 获取root权限

`sudo su`

b. 使用一键脚本安装shadowsocks服务（根据提示对相关信息进行设置）：

`wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh`
`chmod +x shadowsocksR.sh`
`./shadowsocksR.sh 2>&1 | tee shadowsocksR.log`

安装好之后会提示如下的信息：

Congratulations, ShadowsocksR server install completed!

`Your Server IP        :  1.2.3.4` 

`Your Server Port      :  443` 

`Your Password         :  password` 

`Your Protocol         :  origin` 

`Your obfs             :  plain` 

`Your Encryption Method:  aes-256-cfb` 

Enjoy it!

c. 安装BBR加速：

`wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh`



参考页面：[http://www.mzh.ren/gcp-free-ss.html](http://www.mzh.ren/gcp-free-ss.html)





