---
title: SSR Node Deployment
description: How to deploy ShadowsocksR node in server
published: true
date: 2022-06-30T09:24:52.117Z
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

3. Running shadowsocks

```
nohup ssserver -m aes-256-cfb -p 15251 -k abc@123 &
```

> aes-256-cfb is the encryption method, 15251 is the port used, abc@123 is the password, do not forget last &
{.is-info}

