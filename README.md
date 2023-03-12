# btpanel
btpanel7.7开心版
（1）安装时如果报错，请先部署环境后再重新安装（此处以Debian系统为例，其他系统参照）
```
apt update -y && apt dist-upgrade -y && apt install -y curl && apt install -y socat 
apt-get install -y xz-utils openssl gawk file wget screen && screen -S os
```

宝塔面板自7.8开始，违背了宝塔开源协议，竟然在免费版的源码里面加入了加密的授权验证模块。除此之外，7.8版本使用各种方法均无法绕过面板强制绑定账号，如果不绑定账号插件就无法下载。因此这里分享一下7.7版本的安装脚本，以及开心方法。
```
纯原版1：
curl -sSO https://raw.githubusercontent.com/shidahuilang/btpanel/main/install_panel.sh && bash install_panel.sh 

纯原版2： 
wget -O install.sh https://raw.githubusercontent.com/shidahuilang/btpanel/main/install_6.0.sh && bash install.sh 

升/降级到7.7命令： 
curl https://raw.githubusercontent.com/shidahuilang/btpanel/main/update6.sh|bash
```
2、宝塔7.7原版一键开心脚本
```
curl -sSO https://raw.githubusercontent.com/shidahuilang/btpanel/main/one_key_happy.sh && bash one_key_happy.sh
```
更改SSH终端中文语言
```
wget -N --no-check-certificate https://raw.githubusercontent.com/shidahuilang/btpanel/main/LocaleCN.sh && bash LocaleCN.sh
```
开心版安装完成后使用 bt 命令可能出现报错，只需要将终端设置为中文语言即可。（可以查阅LocaleCN.sh文件中对应系统的修改命令，先备份好原始文件，然后使用该命令修改语言并重启，尝试 bt 命令正常后，再恢复原有语言文件。这样做的目的是因为在后期使用时个别程序会因为语言不一致，而导致程序无法正常运行。）
