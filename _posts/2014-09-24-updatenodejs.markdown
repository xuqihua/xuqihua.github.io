---
layout: post
title:  "更新node.js版本"
date:   2014-09-24 22:00
categories: life
permalink: /20140924-vagrant/
---
使用npm包 n。
{% highlight bash %}
;安装包
npm install -g n
;安装最新的稳定版
n stable
;帮助
n -h
  Usage: n [options] [COMMAND] [args]

  Commands:

    n                            Output versions installed
    n latest                     Install or activate the latest node release
    n stable                     Install or activate the latest stable node release
    n <version>                  Install node <version>
    n use <version> [args ...]   Execute node <version> with [args ...]
    n bin <version>              Output bin path for <version>
    n rm <version ...>           Remove the given version(s)
    n prev                       Revert to the previously activated version
    n --latest                   Output the latest node version available
    n --stable                   Output the latest stable node version available
    n ls                         Output the versions of node available

  Options:

    -V, --version   Output current version of n
    -h, --help      Display help information

  Aliases:

    which   bin
    use     as
    list    ls
    -       rm
{% endhighlight %}

