# Cloudflare-workers/pages代理脚本

### 本项目不提供优选IP订阅应用，仅支持单节点分享链接

--------------------------------
## CF vless方案说明及可自定义内容

### 支持workers部署，实现vless+ws+tls与vless+ws两种代理节点

### 支持pages部署，仅实现vless+ws+tls代理节点

#### 一：可直接修改workers.js文件

1、UUID必须自定义（第7行）

2、如果无法访问CF类网站或者ChatGPT，说明ProxyIP失效，可更换ProxyIP，自定义（第9行）

3、伪装网页目前留空，显示为400界面，可自定义（第765行）

#### 二：也可在CF-workers/pages界面中使用变量，方便修改
| 变量作用 | 变量名称| 变量值| 不设置该变量|
| :--- | :--- | :--- | :--- |
| 1、必要的uuid | uuid |符合uuid规定格式 |万人骑uuid：77a571fb-4fd2-4b37-8596-1b7d9728bb5c|
| 2、能上CF类网站 | proxyip |ipv4地址、域名、[ipv6地址]|proxyip域名：workers.cloudflare.cyou|

### 查看相关分享链接，在网页输入：(workers/pages/自定义)域名/自定义uuid

### 详细说明教程请参考[甬哥博客及视频教程](https://ygkkk.blogspot.com/2023/07/cfworkers-vless.html)

---------------------------------
---------------------------------
### CF-CDN优选公共大厂域名脚本，苹果安卓手机平板专用，(请参考教程，在本地网络环境下运行)：
```
curl -sSL https://gitlab.com/rwkgyg/CFwarp/raw/main/point/CFcdnym.sh -o CFcdnym.sh && chmod +x CFcdnym.sh && bash CFcdnym.sh
```
------------------------------------------------------------------------
### CF-优选官方IP+反代IP二合一脚本，苹果安卓手机平板专用，(请参考教程，在本地网络环境下运行)：
```
curl -sSL https://gitlab.com/rwkgyg/CFwarp/raw/main/point/cfip.sh -o cfip.sh && chmod +x cfip.sh && bash cfip.sh
```

-------------------------------------------------------------
### 感谢你右上角的star🌟
[![Stargazers over time](https://starchart.cc/yonggekkk/Cloudflare-workers-pages-vless.svg)](https://starchart.cc/yonggekkk/Cloudflare-workers-pages-vless)
------------------------------------------------------------------------
### 感谢：CF-vless代码作者[3Kmfi6HP](https://github.com/3Kmfi6HP/EDtunnel) CF优选IP程序作者[badafans](https://github.com/badafans/Cloudflare-IP-SpeedTest)、[XIU2](https://github.com/XIU2/CloudflareSpeedTest)

---------------------------------------
#### 声明：

#### 其中一键脚本使用base64加密，可自行解密，介意者请勿使用，[加密原因在此](https://ygkkk.blogspot.com/2022/06/github.html)

#### 所有代码来源于Github社区与ChatGPT的整合；如您需要开源代码，请提Issues留下您的联系邮箱
