
## 申请vps

+ vps: (http://www.vultr.com/?ref=7048874)(tokyo, CentOS6)

## 使用xshell配置ssr

xshell连接vps后在终端执行脚本，来部署ssr
<!-- 安装ss -->
```ss
yum -y install wget

wget –no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev.sh

chmod +x shadowsocks-libev.sh

./shadowsocks-libev.sh 2>&1 | tee shadowsocks-libev.log
```
<!-- 卸载命令：./shadowsocks-libev.sh uninstall -->

<!-- 安装ssr -->
```ssr
yum -y install wget

wget –no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh

chmod +x shadowsocksR.sh

./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
```
<!-- 对着ShadowsocksR的配置选择 -->

## 使用ShadowsocksR在客户端连接ssr