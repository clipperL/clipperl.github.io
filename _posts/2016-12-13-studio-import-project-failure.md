---
layout: post
title:  "【Studio】导入其他项目卡死"
date:   2016/12/13 06:03:42
categories: Studio
---


有次换电脑，把之前电脑上的项目拷过来，然后用studio打开其中一个要修改的项目，然后悲剧了。

![这里写图片描述](http://img.blog.csdn.net/20161106211653823)

漫长的等待，然并卵，用任务管理器，杀死studio，再打开studio，再导入那个项目，然后还是一样，看不到尽头的进度条。

<!-- more -->

这不是个办法，得换个路子，去看了下项目的gradle版本，是2.14.1

![这里写图片描述](http://img.blog.csdn.net/20161106212804789)

而studio上的gradle的版本号是2.10

![这里写图片描述](http://img.blog.csdn.net/20161106213225072)

版本对不上嘛，下载这玩意要FQ，还下的死慢，所以那个进度条一直在那走，走不到尽头。

解决办法其实有两种，首先用任务管理器把干掉。

## **第一种方法**

比较简单，手动把项目的Gradle版本改成studio上的，修改项目的gradle地址在这（Demo1对应你的项目名）：

Demo1\gradle\wrapper\gradle-wrapper.properties

![这里写图片描述](http://img.blog.csdn.net/20161106213327674)

## **第二种方法**

稍微有点麻烦，就是去下载项目中对应的gradle，这是网址：

**http://services.gradle.org/distributions**，

下载后把这个zip文件放在：

C:\Users\用户名\\.gradle\wrapper\dists\gradle-2.14.1-all\8bnwg5hd3w55iofp58khbp6yv，

8bnwg5hd3w55iofp58khbp6yv是文件夹，你的和我的名字不一样。

![这里写图片描述](http://img.blog.csdn.net/20161106214024791)

两种方法，任选一个，然后然后再启动studio，就可以解决gradle版本造成的假卡死。

当然，不要高兴的太早，你马上就会掉入下一处坑。

![这里写图片描述](http://img.blog.csdn.net/20161106214356686)

这是要闹啥！
冷静，这是在下jar包，因为别人的项目中会导入了框架什么哒，举个栗子

![这里写图片描述](http://img.blog.csdn.net/20161106214628440)

我CAO，这么多，要下到凌晨几点，骚年，早点洗洗睡吧，这个只能慢慢下，电脑别关。

只把屏幕关了，这样不会影响睡眠，关屏幕的软件我都帮你准备好了，

**[http://download.csdn.net/detail/yingpaixiaochuan/9451359](http://download.csdn.net/detail/yingpaixiaochuan/9451359)**

拿走，不谢。

补充：[【Studio】Android Studio如何最快速、顺利导入其他项目](http://www.jianshu.com/p/8f4c8c3f6a3a)
