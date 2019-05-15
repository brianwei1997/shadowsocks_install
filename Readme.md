# Auto install ShadowsocksRR Server

Release 2019-5-15
```
切换SSRR至DEV分支
添加rc4 rc4-md5-6加密支持
添加auth_akarin_rand auth_akarin_spec_a协议支持
添加random_head混淆支持
```

shadowsocksR.sh
===============
- Auto Install ShadowsocksR Server for CentOS/Debian/Ubuntu
- https://web.archive.org/web/20190203064434/https://shadowsocks.be/9.html
- ShadowsocksR一键安装脚本
- 使用root用户登录，运行以下命令：

```
wget --no-check-certificate https://raw.githubusercontent.com/zjl88858/shadowsocks_install/master/shadowsocksR.sh
chmod +x shadowsocksR.sh
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
```
- 安装完成后，脚本提示如下：

```Congratulations, ShadowsocksR server install completed!
Your Server IP        :your_server_ip
Your Server Port      :your_server_port
Your Password         :your_password
Your Protocol         :your_protocol
Your obfs             :your_obfs
Your Encryption Method:your_encryption_method

Welcome to visit:https://shadowsocks.be/9.html
Enjoy it!
```
启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
重启：/etc/init.d/shadowsocks restart
状态：/etc/init.d/shadowsocks status
配置文件路径：/etc/shadowsocks.json
日志文件路径：/var/log/shadowsocks.log
代码安装目录：/usr/local/shadowsocks

Copyright (C) 2014-2019 Teddysun
Remastered (C) 2019 Turmi
