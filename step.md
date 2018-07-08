
1. vps: (http://www.vultr.com/?ref=7048874)(tokyo, CentOS6)
2. xshell

 连接vps后在终端执行脚本，来部署ssr

```ss
yum -y install wget

wget –no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev.sh

chmod +x shadowsocks-libev.sh

./shadowsocks-libev.sh 2>&1 | tee shadowsocks-libev.log

卸载命令：./shadowsocks-libev.sh uninstall
```


```ssr
yum -y install wget

wget –no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh

chmod +x shadowsocksR.sh

./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
```

3. ShadowsocksR