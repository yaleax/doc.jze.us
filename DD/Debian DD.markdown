---
layout: post
title:  "DD debian"
date:   2022-11-17 14:54:09 +0800
categories: jekyll update
---



```bash
apt install -y net-tools
```

```bash
ifconfig
```

```
inet 172.26.15.34  netmask 255.255.240.0  broadcast 172.26.15.255
```

```
route -n
```

```
172.26.0.1
```

```
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && chmod a+x InstallNET.sh && bash InstallNET.sh -d 11 -v 64 -a --ip-addr 172.26.13.208 --ip-gate 172.26.0.1 --ip-mask 255.255.240.0 --mirror 'http://mirror.xtom.com.hk/debian/'
```

```
bash <(wget --no-check-certificate -qO- https://cdn.jsdelivr.net/gh/MoeClub/Note/InstallNET.sh) \
-d 11 -v amd64 -a \
-p admin123 \
-apt "http://cloudfront.debian.net/debian/" \
--ip-dns 1.1.1.1 \
--ip-addr 172.26.15.34 \
--ip-mask 255.255.240.0 \
--ip-gate 172.26.0.1
```

```
bash <(wget --no-check-certificate -qO- 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh') -d 9 -v 64 -a

```

