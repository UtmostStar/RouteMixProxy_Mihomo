# RouteMixProxy_Mihomo
用于Mihomo的双路由器流量策略路由代理规则。

适用于Clash Verge等基于Mihomo内核的软件。  

Clash Verge下载 ： https://github.com/clash-verge-rev/clash-verge-rev

通过利用虚拟网卡（TUN 模式），实现了在 Windows 环境下，根据域名、IP 规则自动将流量分发至不同物理链路（如：以太网/国内宽带、Wi-Fi/国际漫游）的功能。

方便Windows使用者身处中国大陆时，同时使用境内宽带和境外手机卡漫游。

大流量境外漫游卡推荐：中国移动香港（CMHK）、中国电信澳门（CT Macau)、中国联通香港（CUniq HK）、和记黄埔香港（3HK）、CelcomDigi等。  

🛠️ 快速开始  
1. 前置准备  

硬件连接：确保电脑同时接入两个网络（例如：网线连接本地 ISP，Wi-Fi 连接漫游网卡热点）。

客户端：推荐使用 Clash Verge 或其他支持 Mihomo 内核的客户端。

环境确认：以管理员权限打开 CMD，运行 netsh interface show interface 记录你的网卡准确名称，如果和仓库中代理规则的interface-name不同，请手动修改到和你的网卡相同的名称。

2. 配置部署  

以管理员模式运行Clash Verge 或其他支持 Mihomo 内核的客户端。

将仓库的配置片段导入进你的 Clash 配置文件中。

打开虚拟网卡（TUN 模式），选择规则代理模式。

3. 测试  

打开 https://ip.skk.moe/ ，当iP138.com与IP.cn 查询网为网线连接的境内ISP，Cloudflare和IPinfo.io为Wi-Fi连接的境外卡漫游运营商，说明功能实现成功。

<img width="1264" height="832" alt="image" src="https://github.com/user-attachments/assets/76572371-7200-4235-b146-c92130164d0c" />
<img width="457" height="400" alt="image" src="https://github.com/user-attachments/assets/c1f6ed83-a849-4c1d-afa1-32d78cc58cfb" />
<img width="1060" height="673" alt="image" src="https://github.com/user-attachments/assets/79046393-c29a-4dd3-b9b5-66483a0643da" />



