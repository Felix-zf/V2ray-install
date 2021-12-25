# Xray-V2ray搭建教程
- 科学上网搭建脚本代码，VPS服务器搭建系统最好选择 Debian9或以上  
- 自备VPS和域名

## VPS测试脚本 
- 检测Vps状态信息(普通)
```
wget -N --no-check-certificate https://raw.githubusercontent.com/91yun/91yuntest/master/test_91yun.sh && bash test_91yun.sh
```

- 检测Vps状态信息(完全)
```
wget -N --no-check-certificate https://raw.githubusercontent.com/91yun/91yuntest/master/test_91yun.sh && bash test_91yun.sh
```

## Curl安装
  ### Debian：
```
apt update -y && apt install -y curl && apt install -y socat
```
  ### CentOS：
```
yum update -y && yum update -y && yum install -y socat
```

## BBR 加速
  ### Google原版BBR
```
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
```

  ### BBR Plus(多合一)
```
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
```

  ### BBR2（限Debian）
```
wget --no-check-certificate -q -O bbr2.sh "https://github.com/yeyingorg/bbr2.sh/raw/master/bbr2.sh" && chmod +x bbr2.sh && bash bbr2.sh auto
```

## 环境搭建
  ### V2ray:
```
bash <(curl -s -L https://git.io/v2ray.sh)
```
  ### Xray:
```
bash <(curl -Ss https://raw.githubusercontent.com/paniy/Xray_bash_onekey/main/install.sh)
```
  ### Trojan:
```
curl -O https://raw.githubusercontent.com/jinwyp/one_click_script/master/trojan_v2ray_install.sh && chmod +x ./trojan_v2ray_install.sh && ./trojan_v2ray_install.sh
```

## Netflix解锁自制剧
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
- 时间设置
```
rm -rf /etc/localtime  /*删除*/
ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime  /*设置*/
```

## 特别感谢 Special Thanks
1. 脚本感谢 https://github.com/233boy/v2ray 
2. 脚本感谢 https://github.com/Jrohy/trojan 
3. 脚本感谢 https://github.com/v2fly/v2ray-core
4. 脚本感谢 https://github.com/XTLS/Xray-core
5. 脚本感谢 https://github.com/trojan-gfw/trojan
6. 脚本感谢 https://github.com/p4gefau1t/trojan-go
7. 脚本感谢 https://github.com/jinwyp/one_click_script
8. 脚本感谢 https://github.com/sjlleo/netflix-verify
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

