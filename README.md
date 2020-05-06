# v2ray
最好用的 V2Ray 一键安装脚本 &amp; 管理脚本<br>
直接输入安装命令：

```

git clone https://github.com/Pinanchen/V2ray-auto -b master
cd V2ray-auto
chmod +x install.sh
./install.sh local

```

## 脚本说明
[V2Ray 一键安装脚本](https://github.com/233boy/v2ray/wiki/V2Ray%E4%B8%80%E9%94%AE%E5%AE%89%E8%A3%85%E8%84%9A%E6%9C%AC)

## 搭建教程
[V2Ray搭建详细图文教程](https://github.com/233boy/v2ray/wiki/V2Ray%E6%90%AD%E5%BB%BA%E8%AF%A6%E7%BB%86%E5%9B%BE%E6%96%87%E6%95%99%E7%A8%8B)

## 资助 V2Ray
请考虑 [资助 V2Ray 发展](https://www.v2ray.com/chapter_00/02_donate.html)

## 更多 V2Ray 教程文章
https://github.com/233boy/v2ray/wiki

关闭BBR：
nano /etc/sysctl.conf

把下面两句注释掉
# net.core.default_qdisc = fq
# net.ipv4.tcp_congestion_control = bbr

保存更改
sysctl -p

重启系统
reboot

如果没有出现bbr证明停止成功
lsmod | grep bbr

