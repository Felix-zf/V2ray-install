# Xray-V2ray
科学上网搭建脚本代码，VPS服务器搭建系统最好选择 Debian9或以上

# 环境搭建
Debian:(Curl安装):
```
apt update -y && apt install -y curl && apt install -y socat
```
CentOS:(Curl安装):
```
yum update -y && yum update -y && yum install -y socat
```
# 开启自带 BBR 加速
DebianBBR2加速：
```
wget --no-check-certificate -q -O bbr2.sh "https://github.com/yeyingorg/bbr2.sh/raw/master/bbr2.sh" && chmod +x bbr2.sh && bash bbr2.sh auto
```
# 脚本搭建
V2ray:
```
bash <(curl -s -L https://git.io/v2ray.sh)
```
Xray:
```
bash <(curl -Ss https://raw.githubusercontent.com/paniy/Xray_bash_onekey/main/install.sh)
```
 
