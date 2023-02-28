---
title: acme对nginx自动续签证书
layout: post
author: y377
---

## 一条命令
```bash
acme.sh --install-cert -d demo.navigation.heyun.vip \
--key-file       /root/.acme.sh/demo.navigation.heyun.vip/demo.navigation.heyun.vip.key  \
--fullchain-file /root/.acme.sh/demo.navigation.heyun.vip/fullchain.cer \
--reloadcmd     "service nginx force-reload"
```
