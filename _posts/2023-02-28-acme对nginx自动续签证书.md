---
title: 使用acme为nginx自动续签证书
layout: post
author: y377
---

##### 1. 先签发/获取证书

`acme.sh --issue --dns dns_ali -d 你的域名 --keylength ec-256 --server letsencrypt`

###### 2. 将获取到的证书和私钥拷贝到nginx的相应目录

```bash
cp /root/.acme.sh/你的证书路径/Private.key /etc/nginx/ssl/你的nginx证书路径/
cp /root/.acme.sh/你的证书路径/fullchain.cer /etc/nginx/ssl/你的nginx证书路径/
```

###### 3. 安装自动续签（这是一条命令，尾部 “\” 表示：自动换行）

```bash
acme.sh --install-cert -d demo.navigation.heyun.vip \
--key-file       /root/.acme.sh/demo.sample.vip/sample.vip.key  \
--fullchain-file /root/.acme.sh/demo.sample.vip/fullchain.cer \
--reloadcmd     "service nginx force-reload"
```

###### 4. 如果`service nginx force-reload`没效果，执行下面命令：
 > 先`nginx -t`，再`systemctl restart nginx`

**另请注意ECC加密的使用方法，加上**`--ecc`(前提是如果你申请的ECC加密)

```bash
acme.sh --install-cert -d www.heyun.vip \
--ecc --key-file /etc/nginx/ssl/www.heyun.vip/www.heyun.vip.key \
--fullchain-file /etc/nginx/ssl/www.heyun.vip/fullchain.cer \
--reloadcmd "service nginx force-reload"
```
