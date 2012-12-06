---
layout: post
title: "关于在IE下超链接传递参数的问题"
date: 2012-10-15 22:54
comments: true
categories: 
---
最近同事在开发过程中，发现一个很奇怪的问题，在`Internet explorer`上出现的，而在`Google Chrome` 和`Firefox`上都没有出现。

首先，请求是这样的：
{% include_code httphyperlink.html %}
当我打开上面那个超链接的时候，发现我没能拿到` para ` 这个参数的值，貌似直接就没有传到后台，
然后当我把鼠标移动到那个链接上的时候，我发现原来我的超链接变成了这样：
{% include_code httphyperlinkerror.html %}
<!--more-->
{% img /images/httpproblem.png %}
<br/>这个时候，原来的`&amp;para`变成了`¶`符号。原来，这里的`&amp;para`被当成了特殊字符，而被转义了。  
当然，解决的办法有很多，比如 

- 1、可以交换下参数的位置，把`para`放最前面，而其他参数放后面.
- 2、还可以把参数名改成别的，比如`para`改成`param`. 
- 3、也把请求改成POST方式的表单提交.  
- 4、还可以把参数名&amp;amp改成为`&amp;para`. 

总之，这种问题应该避免，应该在开发的过程中，尽量使用有意义的参数名，可以防止随意使用名称，导致的此类问题。

这里附上一篇常用的一些HTML特殊字符的转义，来源于[网络](http://114.xixik.com/character/)