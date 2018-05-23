# V2RAY 基于 CADDY 的 VMESS+H2+TLS+Website(Use Host) 

### HTTP Header 分流，自带 Website 伪装站点 http 强制跳转 https，支持ssl非443端口，自带Rinetd BBR加速 支持OpenVZ，自动生成客户端config.json配置文件 web在线下载，重装自动清除残余的Http服务，每天自动升级最新的V2ray内核，支持 cdn 嵌套，自动续签ssl证书，自动生成Windows客户端和便捷启动脚本 一键添加开机自启动服务 一键开启系统ie代理。

使用：1.解析好域名； 2.运行一键安装脚本；
```
wget -N --no-check-certificate git.io/h.sh && chmod +x h.sh && bash h.sh
```
[新手请使用 Debian8 纯净系统安装]

备用1：一键更换新的 UUID，同时升级 Windows 客户端 （new）
```
bash h.sh -n
```

备用2：一键删除服务器中储存的客户端 config.json 配置文件，防止 Website 被抓取 （rm）
```
bash h.sh -r
```

共享你的 V2ray 账号 （share）
```
bash h.sh -s

开启共享模式后，每周一自动更换 UUID 并推送至 Website 伪装站点首页。
为防止被恶意抓取，该模式下不提供客户端 config.json 文件下载。
```

赞助 V2ray 项目（xmr）
```
bash h.sh -x

注意：开启赞助功能后，会在 website 首页植入 xmr 挖矿脚本。
      任何电脑只要浏览器访问 website 点击允许，即可开始挖矿赞助 v2ray 项目，关闭网页停止挖矿。
声明：脚本不会在你的 vps 内植入任何挖矿脚本，不会利用你的 vps 进行挖矿，同时也不建议你自己使用 vps 挖矿（得不偿失）。
```

注册免费域名
```
http://www.freenom.com
需更换ns服务器，默认ns服务器在国内很不稳定。
```

HTTP2 CDN 嵌套
```
又拍云、七牛、阿里都不错，腾讯的 h2 还在内测，百度不清楚。
速度提升非常大，也非常稳定，高峰期毫无压力，在重点 IP 段也无所畏惧。
（cloudflare 不支持 http2）
```
