---
title: 浅谈集成部署博客
date: 2021.4.17
tags: happy
mathjax: true
---
## 前置准备
+ 拥有良好的网络·
+ 可以「红楼别夜堪惆怅」3jONKj/3io1q7。（非必须
+ 在github有账号
+ 已下载git
+ 拥有一个hexo博客

好了，就这么多。


## 开始
  + 已经有现成的项目

         那就简单了，用git首先push到github，这里我以我的hexo项目为例：
        注意，请上传你的hexo在本地的内容（用git），而不是上传public下的文件）

      ![](https://i.loli.net/2021/04/17/LEs9e64hvdctNjI.png)

   （由于我安装了一些插件所以可能会和你的不太一样，不要在意）

     好，显而易见这个项目是不能部署到github pages上的，因为没有index.html，那怎么办呢？~~是时候召唤超级飞侠了~~这时候集成部署就出来了，我们选择<https://vercle.com>来部署我们的项目。

    进入这个网站之后，选择用github登录。
应该是这个样子的。

   ![](https://i.loli.net/2021/04/17/SsA5exrcaiwgDZR.png)

 点击New Project，看Import Git Repository那一栏，找到你的hexo仓库，点击import，。接下来到
  这一步

  ![](https://i.loli.net/2021/04/17/V3n8OLChWjEt7aR.png)

 应该会检测到你是hexo框架，所以默认了hexo部署。如果没有的话请检查你的前期准备。确认无误后点击Deploy。部署成功的话会是这样的：
 
![](https://i.loli.net/2021/04/17/TgohVKOEYwepsmk.png)

   + 无本地项目

      这样的话相对简单一些，还是会用到vercel。在New Project中看Clone Template这一栏，找到hexo，选择后配置github仓库什么的，就可以了。之后更改操作直接在github上改，下载主题到本地然后push上去就好了
 
## 为什么要用集成部署
   ### 优点

    1. 修改博客方便，如果你在电脑上本地安装hexo，换一台电脑就要装一遍，更别提手机了。用了集成部署，直接在github上操作，对于本地环境难配置的有很大的友好度
    2. 可以使用[hexoplusplus](hexoplusplus.js.org)，这是一个相当于有后端的hexo
    3. 修改更简洁，避免本地上传一些奇奇怪怪的错误

   ### 缺点

    1. 下载插件，主题比较麻烦，须重新push
    2. 对于新手不太友好
   
