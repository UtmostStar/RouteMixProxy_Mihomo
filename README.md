# RouteMixProxy_Mihomo
用于Mihomo的双路由器流量策略路由代理规则。  

适用于Clash Verge等基于Mihomo内核的软件。  

通过利用虚拟网卡（TUN 模式），本项目实现了在 Windows 环境下，根据域名、IP 规则自动将流量分发至不同物理链路（如：以太网/Wi-Fi、国内宽带/国际漫游）的功能。

🛠️ 快速开始
1. 前置准备
硬件连接：确保电脑同时接入两个网络（例如：网线连接本地 ISP，Wi-Fi 连接漫游网卡热点）。

客户端：推荐使用 Clash Verge 或其他支持 Mihomo 内核的客户端。

环境确认：以管理员权限打开 CMD，运行 netsh interface show interface 记录你的网卡准确名称。

2. 配置部署
以管理员模式运行Clash Verge 或其他支持 Mihomo 内核的客户端。

将仓库的配置片段导入进你的 Clash 配置文件中。

打开虚拟网卡（TUN 模式），选择规则代理模式。