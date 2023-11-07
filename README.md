# Xray-V2ray搭建教程
- 科学上网搭建脚本代码，VPS服务器搭建系统最好选择 Debian9或以上  
- 自备VPS和域名


## VPS测试 
管理员权限sudo -i
- VPS性能测试一键脚本
```
wget -qO- git.io/superbench.sh | bash
```

- 一键检测VPS回程国内三网路由
```
wget -N --no-check-certificate https://raw.githubusercontent.com/91yun/91yuntest/master/test_91yun.sh && bash test_91yun.sh
```

- BlueSkyXN综合工具箱
```
wget -O box.sh https://raw.githubusercontent.com/BlueSkyXN/SKY-BOX/main/box.sh && chmod +x box.sh && clear && ./box.sh
```


## Curl安装
### CentOS：
```
yum update -y && yum update -y && yum install -y socat
```
### Debian：
```
apt update -y && apt install -y curl && apt install -y socat
```


## 环境搭建
  ### V2ray:
```
bash <(curl -s -L https://git.io/v2ray.sh)
```

```
bash <(curl -s -L https://git.io/v2ray-setup.sh)
```

### Xray:
```
bash <(curl -Ss https://raw.githubusercontent.com/paniy/Xray_bash_onekey/main/install.sh)
```
### Trojan:
```
curl -O https://raw.githubusercontent.com/jinwyp/one_click_script/master/trojan_v2ray_install.sh && chmod +x ./trojan_v2ray_install.sh && ./trojan_v2ray_install.sh
```


## BBR加速
- Linuux系统内核版本>4.9,输入uname -r查询
- 安装完毕输入reboot重启
### Google原版BBR
```
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
```

### BBRPlus (多合一)
```
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
```

### BBR2 (Debian)
```
echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
sysctl -p
lsmod | grep bbr
```


## Netflix
- 检测Netflix状态信息
```
wget -O nf https://github.com/sjlleo/netflix-verify/releases/download/2.61/nf_2.61_linux_amd64 && chmod +x nf && clear && ./nf
```

- 解锁Netflix非自制剧
```
bash <(curl -fsSL git.io/warp.sh) menu
```

- 重启 WARP WireGuard
```
systemctl restart wg-quick@wgcf
```

- 关闭 WARP WireGuard
```
systemctl disable wg-quick@wgcf --now
```


## 附加命令
- 校准时间V2ray
```
rm -rf /etc/localtime  /*删除*/
ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime  /*设置*/
```
- 其它命令
```
./tcp.sh   /*重新连接服务器*/
v2ray url  /*获取订阅链接*/
```


## 软路由
- 桥接模式 (旁路由)
```
vi /etc/sysconfig/network  /*Insert输入，Esc退出*/
:wq     /*内网IP段保存，回车键退出*/
reboot  /*重启*/
```

- 固件&写盘
1. 固件系统: https://openwrt.org/     
2. 写盘工具: https://m0n0.ch/wall/physdiskwrite.php  


## 游戏加速器
1. Netch: https://github.com/netchx/netch
2. SSTap: https://github.com/FQrabbit/SSTap-Rule


## Other协议代码
持续更新ing
1. X-ui: https://www.v2rayssr.com/x-ui.html
2. V2Board: https://docs.v2board.com/deploy/aapanel.html
3. 8combine1: https://github.com/mack-a/v2ray-agent
4. Hysteria2: https://blog.misaka.rest/2023/09/02/hysteria2-script
```
wget -N --no-check-certificate https://raw.githubusercontent.com/Misaka-blog/hysteria-install/main/hy2/hysteria.sh && bash hysteria.sh
```

## 特别感谢 Special Thanks
1. 脚本感谢 https://github.com/Jrohy/trojan
2. 脚本感谢 https://github.com/233boy/v2ray
3. 脚本感谢 https://github.com/fscarmen/warp
4. 脚本感谢 https://github.com/XTLS/Xray-core
5. 脚本感谢 https://github.com/v2fly/v2ray-core
6. 脚本感谢 https://github.com/p4gefau1t/trojan-go
7. 脚本感谢 https://github.com/jinwyp/one_click_script
8. 脚本感谢 https://github.com/trojan-gfw/trojan
9. 脚本感谢 JCNF的博客 https://ybfl.xyz/111.html
10. 特别感谢油管博主 [小六教学](https://www.youtube.com/channel/UCE8MoWhC8Fp1L9LbZw0I6kQ)


## Stargazers over time
[![Stargazers over time](https://starchart.cc/jinwyp/one_click_script.svg)](https://starchart.cc/jinwyp/one_click_script)



[better-cloudflare-ip]: https://github.com/badafans/better-cloudflare-ip/releases
[CFIP]: https://github.com/BlueSkyXN/CFIP/releases
[CloudflareScanner]: https://github.com/Spedoske/CloudflareScanner/releases/tag/1.1.2
[CloudflareSpeedTest]: https://github.com/XIU2/CloudflareSpeedTest/releases/tag/v1.4.9

PS: 💖💖💖Have a good time every day!ヾ(≧▽≦*)o🎄🎈🎈

![Saber](https://github.com/Felix-zf/Picture-Store/blob/master/img/R1.jpg?raw=true)

