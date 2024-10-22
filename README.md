<p align="center">
<img width="768" src="https://raw.githubusercontent.com/QiuSimons/Others/master/YAOF.png" >
</p>
<p align="center">
<img src="https://github.com/Tired-Fox/cargors/raw/aabd34c/assets/badges/built_with_love.svg">
<p>
<p align="center">
<img alt="GitHub All Releases" src="https://img.shields.io/github/downloads/QiuSimons/YAOF/total?style=for-the-badge">
<img alt="GitHub" src="https://img.shields.io/github/license/QiuSimons/YAOF?style=for-the-badge">
<p>
<p align="center">
<img src="https://github.com/QiuSimons/YAOF/workflows/R2C-OpenWrt/badge.svg">
<img src="https://github.com/QiuSimons/YAOF/workflows/R2S-OpenWrt/badge.svg">
<img src="https://github.com/QiuSimons/YAOF/workflows/R4S-OpenWrt/badge.svg">
<img src="https://github.com/QiuSimons/YAOF/workflows/X86-OpenWrt/badge.svg">
<p>


### 特性

- 基于原生 OpenWrt 23.05 编译，默认管理地址 192.168.1.1
- 默认开启了 SFE（修正了 udp 入站以及 sqm 兼容性问题）
- 内置升级功能可用，物理 Reset 按键可用
- 预配置了部分插件<b>(注意，使用 MosDNS 同时作为广告过滤手段及 dns 分流措施。)</b>
- 可无脑 opkg kmod
- R2C/R2S 核心频率 1.6（交换了 LAN WAN），R4S 核心频率 2.2/1.8（建议使用带有线损补偿的电源，死机大多数情况下，都是因为<b>你用的电源过于垃圾</b>，另外，你也可以选择使用<b>自带的 app 限制最大频率</b>，茄子 🍆）
- O2 编译，CFLAG 优化
- 插件包含：PassWall2，DAED，UPNP，FullCone(防火墙中开启，默认开启)，流量分载，irq 优化
- ss 协议在 armv8 上实现了 aes 硬件加速（请<b>仅使用 aead 加密</b>的连接方式）
- 集成并默认启用了 BBRv3，LRNG
- 如有任何问题，请先尝试 ssh 进入后台，输入 fuck 后回车，等待机器重启后确认问题是否已经解决
