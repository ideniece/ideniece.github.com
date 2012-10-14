---
layout: post
title: "ubuntu error"
date: 2012-10-09 20:41
comments: true
categories: 
---
Java print:{% codeblock lang:java %}
System.out.println("Hello world!");
{% endcodeblock %}
Java println:{% codeblock lang:java %}
for(int i=1;i<=100;i++){
 System.out.println("i="+i);
}
System.out.println("it's over!!!!");
System.out.println("it's not over..........................................................................................");
{% endcodeblock %}
<!-- more -->
type the command in your terminal:
``` 
sudo apt-get update
sudo apt-get install ruby1.9.3
``` 
t be reported:

You have some obsolete package versions installed. Please upgrade the following packages and check if the problem still occurs:

signon-ui, coreutils, cpio, dbus, dpkg, findutils, gcc-4.7-base, ifupdown, klibc-utils, libacl1, libavahi-client3, libavahi-common-data, libavahi-common3, libc-bin, libc6, libcups2, libdb5.1, libdbus-1-3, libexpat1, libgcc1, libglib2.0-0, libglib2.0-data, libgpg-error0, libklibc, liblocale-gettext-perl, libmng1, libncurses5, libncursesw5, libnih-dbus1, libnih1, libpcre3, libproxy1, libqt4-dbus, libqt4-declarative, libqt4-network, libqt4-script, libqt4-sql, libqt4-xml, libqt4-xmlpatterns, libqtcore4, libqtgui4, libstdc++6, libtext-charwidth-perl, libtext-iconv-perl, libtinfo5, libudev0, libxcb1, libxml2, lsb-base, module-init-tools, mountall, multiarch-support, ncurses-bin, qdbus, sed, shared-mime-info, udev, x11-common

测试下中文是否可以使用？
