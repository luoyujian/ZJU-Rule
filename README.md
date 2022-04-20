# HNU Rule

基于 [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR/tree/master) 修改后的 HNU 分流规则

项目使用 CC-BY-SA-4.0 协议发布 [![CC-BY-SA-4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/deed.zh)

## 支持功能

+ 内网资源/学术资源分流（直连访问/内网穿透访问）
+ 节点自动选择
+ 节点故障转移
+ 节点负载均衡
+ Telegram 分流
+ Youtube 分流
+ Netflix 分流
+ 动画疯分流
+ 哔哩哔哩分流（解锁港澳台）
+ Google 服务分流
+ OneDrive 分流
+ Microsoft 服务分流
+ Apple 服务分流
+ 游戏平台分流（Steam/Epic/Sony）
+ 网易云音乐分流（灰色歌曲解锁）
+ 广告拦截/应用净化/AdBlock/隐私防护
+ 节点分地区管理（香港/日本/美国/台湾/狮城/韩国）
+ ...

## 使用方法

### 安装 Clash

+ 使用 [Clash](https://github.com/Dreamacro/clash) 作为代理工具，此工具支持 SS/SSR/V2Ray/Trojan/HTTP/HTTPS/SOCKS 等多种协议。不同平台的客户端如下：

  + Windows: [Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases)
  + Mac: [ClashX](https://github.com/yichengchen/clashX/releases)（推荐） 或 [Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases)
  + Android/HarmonyOS: [Clash for Android](https://github.com/Kr328/ClashForAndroid/releases)



### 转换订阅链接

+ 无论机场提供的订阅链接是 SS/SSR/V2Ray 等订阅链接，还是 Clash 订阅链接，都需要提取出其中的节点信息，再按照 HNU Rule 进行处理，生成处理后的 Clash 订阅链接

+ 订阅转换需要使用 [subconverter](https://github.com/tindy2013/subconverter)。subconverter 的部署较为复杂，推荐使用已在腾讯云香港部署完成的公用 ZJU Rule 转换服务。也可以自己搭建 subconverter 并使用 HNU Rule 规则进行订阅转换


### 配置分流方式

![](docs/clash.png)

Clash 采用继承的分流配置方式，例如，巴哈姆特设置为使用台湾节点，则将使用台湾节点分组中选中的节点进行代理。可以根据自己的需要进行配置，如将哔哩哔哩配置为香港/台湾节点以访问港澳台资源
