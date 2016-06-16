---
layout: post
title:  "安装electron失败解决方法"
date:   2016-06-16 10:44:00
categories: electron
permalink: /install-electron-in-china/
---

1. npm源过慢的话，可以把源切到国内的淘宝的镜像上。

npm config set registry https://registry.npm.taobao.org

2. 到electron的国内镜像下载最新的安装包，主要看好自己系统对应的版本

https://npm.taobao.org/mirrors/electron

3. 将下载好的包放到当前用户的根目录下的.electron文件夹下，windows一般是C:\Users\YourUserName\.electron

4. 执行安装命令npm install electron-prebuilt -g