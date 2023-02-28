---
title: centos7 Install Jekyll
layout: post
---

### 安装步骤
 > 参照[Jekyll官网](https://jekyllrb.com/docs/)

1. 安装**rvm**前需要先导入官网密钥，才能下载安装

```
gpg2 --keyserver hkp://keyserver.ubuntu.com --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
```

2. 开始安装

`\curl -sSL https://get.rvm.io | bash -s stable`

3. 如果出现下图 表示成功了（需要你退出当前shell，再此登录；如果你有钱，也可以给该开发团队捐赠）

```shell
[root@node1 ~]# \curl -sSL https://get.rvm.io | bash -s stable
Downloading https://github.com/rvm/rvm/archive/1.29.12.tar.gz
Downloading https://github.com/rvm/rvm/releases/download/1.29.12/1.29.12.tar.gz.asc
gpg2 --keyserver hkp://keyserver.ubuntu.com --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDBcurl: (28) Connection timed out after 30001 milliseconds

Could not download 'https://github.com/rvm/rvm/releases/download/1.29.12/1.29.12.tar.gz.asc'.
  curl returned status '28'.

Creating group 'rvm'
Installing RVM to /usr/local/rvm/
Installation of RVM in /usr/local/rvm/ is almost complete:

  * First you need to add all users that will be using rvm to 'rvm' group,
    and logout - login again, anyone using rvm will be operating with `umask u=rwx,g=rwx,o=rx`.

  * To start using RVM you need to run `source /etc/profile.d/rvm.sh`
    in all your open shell windows, in rare cases you need to reopen all shell windows.
  * Please do NOT forget to add your users to the rvm group.
     The installer no longer auto-adds root or users to the rvm group. Admins must do this.
     Also, please note that group memberships are ONLY evaluated at login time.
     This means that users must log out then back in before group membership takes effect!
Thanks for installing RVM 🙏
Please consider donating to our open collective to help us maintain RVM.

👉  Donate: https://opencollective.com/rvm/donate
```

4. 使用`rvm -v`验证一下，得到下图（表示成功安装了rvm）

```shell
[root@node1 ~]# rvm -v
rvm 1.29.12 (latest) by Michal Papis, Piotr Kuczynski, Wayne E. Seguin [https://rvm.io]
[root@node1 ~]#
```

5. 开始安装**ruby**
 - 可以使用`rvm list known`查看当前**稳定版**的_ruby版本_ 
 - 我是选择了*ruby3.0*，`rvm install ruby-3`

6. 占位符/正在编辑
