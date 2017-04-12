---
layout: post
title:  "【Android】修改TabLayout中标签文字的样式"
date:   2016/12/10 13:03:42
categories: Android
---


![这里写图片描述](http://img.blog.csdn.net/20161114171301525)

我们在用TabLayout和ViewPager做可以滑动的标签和碎片时，标签的样式一般只能设置文字颜色、滑块的颜色和厚度值

<!-- more -->

![这里写图片描述](http://img.blog.csdn.net/20161114105224937)

如果我想设置文字的大小和加粗，在这必须用到

```
app:tabTextAppearance="@style/CustomTabLayoutTextAppearance"
```
完整代码就是这样：

![这里写图片描述](http://img.blog.csdn.net/20161114105246222)

这个style需要自己在styles.xml中自己定义，我在里边写了字体的大小、加粗、黑色（刚开始没写颜色直接给我展示了白色，尴尬）

![这里写图片描述](http://img.blog.csdn.net/20161114105258035)