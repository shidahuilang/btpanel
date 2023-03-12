# btpanel
btpanel7.7开心版
宝塔面板自7.8开始，违背了宝塔开源协议，竟然在免费版的源码里面加入了加密的授权验证模块。除此之外，7.8版本使用各种方法均无法绕过面板强制绑定账号，如果不绑定账号插件就无法下载。因此这里分享一下7.7版本的安装脚本，以及开心方法。
```
纯原版1：
curl -sSO https://raw.githubusercontent.com/zhucaidan/btpanel-v7.7.0/main/install/install_panel.sh && bash install_panel.sh 

纯原版2： 
wget -O install.sh http://f.cccyun.cc/bt/install_6.0.sh && bash install.sh 

升/降级到7.7命令： 
curl http://f.cccyun.cc/bt/update6.sh|bash
```
2、宝塔7.7原版一键开心脚本
```
curl -sSO https://raw.githubusercontent.com/ztkink/bthappy/main/one_key_happy.sh && bash one_key_happy.sh
```
