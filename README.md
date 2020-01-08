# my-personal-proxy-settings
this repo archive my personal V2Ray proxy settings.

*****

这个仓库用于保存我本地的V2Ray客户端设定。供不会配置的人参考。


目前只有一个很简单的基础版本「sample.json」：
* 需要代理的网站，出口走 vmess 协议
* 预定义列表内的国内域名直连（不走代理）
* 预定义列表内的国内IP直连
* 局域网IP直连
* 预定义列表内的常见广告域名直接block掉，不发出
* 测速网站直连
* BT下载的流量直连
* 剩下所有流量都走V2Ray服务器转发

可以发现该文件内没有配置 inbounds ，因为我用的本地客户端是Mellow，它直接代理了全局流量。如果你也用Mellow，可以直接拿去用。(只需要修改 "vnext" 项内形如的 *XXXX* 的项目为你自己的服务器设定即可)
否则请自行配置 inbounds 规则。