---
title: centos7安装Jekyll
layout: post
tag: centos7 jekyll
---

#### 首先安装rvm
```bash
gpg2 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
\curl -sSL https://get.rvm.io | bash -s stable
rvm list            #查看Ruby版本
rvm install 2.6.5  #可以指定版本安装
rvm install 2.7   #可以指定版本安装
rvm use 3.0.0 -default #切换ruby3.0为默认版本
rvm gemset update #更新所有rubygems包
yum install gcc         //gcc -v
yum install gcc-c++      //g++ -v
yum install make        make -v
```
#### 安装Jekyll
`gem install jekyll`
