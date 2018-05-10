---
layout: post
title:  "【其他】Hexo框架 Next 主题的一些设置细节"
date:   2018-05-10 20:42:04
categories: Other
---

### 以下设置，主要是在 Hexo\themes\next 的 _config.yml 做修改：

1. 侧边栏头像

   avatar: /images/luFei.jpg

   > 图片路径：Hexo\themes\next\source\images

2. 关闭加载动画

   以前是 use_motion，现在（6.0）改为 motion 了，设置更详细了，true 改为 false；

3. 显示语言

   在 Hexo\themes\next\languages 找到需要的语言，比如 zh-CN.yml（中文简体）；

   在 Hexo\\_config.yml 中设置 language 为 zh-CN；

