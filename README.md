# mup-aliyun

在阿里云的ubuntu 14.04 上用mup，自动安装phantomjs装不上，这个script试图解决这个问题。目前只支持安装 x86_64 版phantomjs 1.9.8.

1. 在云主机上用root或者可以sudo（无密码）的用户登录
2. 运行以下script
```
git clone https://github.com/xigua/mup-aliyun
cd mup-aliyun
./install-phantomjs.sh```
3. 如顺利安装成功，再使用mup来远程或者本地deploy meteor app，注意在mup.json里将setupPhantom设为false。

亦可参考 https://github.com/wmzhai/setup-meteor-machine/blob/master/README.md 中文安装指南。
