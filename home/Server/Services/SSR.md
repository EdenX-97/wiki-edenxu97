---
title: SSR Node Deployment
description: How to deploy ShadowsocksR node in server
published: true
date: 2022-06-30T09:22:25.300Z
tags: server, ssr
editor: markdown
dateCreated: 2022-06-30T09:08:48.125Z
---

# Install

1. Connect to your server (can use ssh)
> My server OS version is CentOS 7.8, if you can't use yum, consider the appropriate command
{.is-warning}

2. Install python3 and shadowsocks (run the following code line by line)

```
yum install python3
pip3 install https://github.com/shadowsocks/shadowsocks/archive/master.zip -U
```
