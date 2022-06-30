---
title: SSR Node Deployment
description: How to deploy ShadowsocksR node in server
published: true
date: 2022-06-30T09:33:41.507Z
tags: server, ssr
editor: markdown
dateCreated: 2022-06-30T09:08:48.125Z
---

# Install

1. Connect to your server (can use ssh)
> My server OS version is CentOS 7.8, if you can't use yum, consider the appropriate command for your OS
{.is-warning}

2. Install python3 and shadowsocks (run the following code line by line)

```
yum install python3
pip3 install https://github.com/shadowsocks/shadowsocks/archive/master.zip -U
```

# Running

```
nohup ssserver -m aes-256-cfb -p 15251 -k 123 &
```

> aes-256-cfb is the encryption method, 15251 is the port you can modify, 123 is the password you can choose, do not forget last &
{.is-info}

After the above command, you can exit the ssh connect if running correctly.

# Using

1. Download the client for your OS, suggest:
	- Windows: [Shadowsocks](http://shadowsocks.org/)
  - Mac: [ShadowsocksX-NG](https://github.com/shadowsocks/ShadowsocksX-NG/releases)
  - Iphone/Ipad: Shadowrocket in AppStore
2. In client, add a new server
	- Address: Your server ip or domain
  - Port: 15251 or what you set
  - Password: 123 or what you set
  - Method/Encryption: aes-256-cfb
3. Click Ok/Donw and open the connection in client, enjoy!
  



