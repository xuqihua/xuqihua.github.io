---
layout: post
title:  "更新mac下的pear和pecl并且安装php-intl拓展"
date:   2015-04-10 14:45:00
categories: uncategory
permalink: /update-mac-pecl/
---

##安装pear&pecl并更新
{% highlight bash %}
cd /usr/lib/php 
sudo php install-pear-nozlib.phar 
Edit:
/etc/php.ini and find the line: ; 
include_path = ".:/php/includes" 
修改为: 
include_path = ".:/usr/lib/php/pear" 
sudo pear channel-update pear.php.net 
sudo pecl channel-update pecl.php.net 
sudo pear upgrade-all
{% endhighlight %}
##安装依赖icu
{% highlight bash %}
wget http://download.icu-project.org/files/icu4c/55.1/icu4c-55_1-src.tgz
tar xvzf icu4c-55_1-src.tgz
cd icu4c-55_1-src
./configure
make
make install
{% endhighlight %}
##安装
{% highlight bash %}
sudo pecl install intl
{% endhighlight %}







