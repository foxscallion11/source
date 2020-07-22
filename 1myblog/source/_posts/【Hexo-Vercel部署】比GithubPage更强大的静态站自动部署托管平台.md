---
title: 【Hexo+Vercel部署】比GithubPage更强大的静态站自动部署托管平台
abbrlink: 2c4e5608
date: 2020-07-22 01:57:00
cover: http://qdraqx6e2.bkt.clouddn.com/blog/20200722/025956171.png
tags: vercel
categories: 
 - HEXO
 - vercel
top: true
top_img:
---

## 前言

{% blockquote Seth Godin http://sethgodin.typepad.com/seths_blog/2009/07/welcome-to-island-marketing.html Welcome to Island Marketing %}
注： 著作权归作者所有。
商业转载请联系作者获得授权，非商业转载请注明出处。

原文地址：  https://foxlemon.vercel.app/posts/2c4e5608.html 原作者：foxscallion 本文没有授权给任何组织、企业和个人转载，未经作者允许禁止转载！ {% endblockquote %}

 <div class='tip font5 fas fa-atom'><p>因为域名的备案申请还没有通过，想着能够通过免费的CDN来加速网站，同时又能够满足免费的域名，偶尔在别人博客网站上看到了<p></div>

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/020224337.png)

<div class="tip wtgo font5 fas fa-bolt"><p>于是我就通过百度发现了这个vercel是真的真的好用，全自动部署，只要你提交GitHub代码到vercel就可以了，几天前我就想注册个vercel，只是一直苦于无法注册，如图</p><p></p></div>

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/020543399.png)

<div class="tip qq font5 fab fa-qq"><p>于是我用谷歌空间注册了foxscallion@gmail.com账号，然后重新注册GitHub，通过这个样子，终于vercel成功登入了。</p><p></p></div>



## 通过邮箱重新注册个GitHub

- GitHub重新注册完，添加token密钥

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/021132801.png)

- 将这些框框全部✔，然后确定

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/021215949.png)

- 然后新建仓库（怎么建就不说了）

- 把密钥token添加到博客根目录_config.yml的repo

* <div class="tip qq font5 fab fa-qq"><p>这里先复制密钥（密钥☞存在一次）先复制出来</p><p></p></div>

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/022233262.png)

* <div class="tip qq font5 fab fa-qq"><p>注意https://密钥@仓库地址</p><p></p></div>

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/022049398.png)

- 复制你的仓库git地址

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/021348689.png)

- 修改博客根目录的_config.yml，将你的地址换过来

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/021525881.png)





![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/021608624.png)

- 然后hexo clean ，hexo g ，hexo deploy，提交到你刚刚建的GitHub仓库

## 注册你的vercel

- 访问[Vercel](https://link.zhihu.com/?target=https%3A//vercel.com/)官网，根据提示注册账号。个人用户可以免费使用。

* <div class="tip qq font5 fab fa-qq"><p>我的是用谷歌的邮箱注册GitHub，然后通过GitHub绑定vercel的</p><p></p></div>

* 我的是用谷歌的邮箱注册GitHub，然后通过GitHub绑定vercel的

* ![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/022926816.png)

* ![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/022946779.png)

### 

- 点击`Import Project` -> `Import Git Repository`，输入git仓库地址，vercel与Github基本上是无缝衔接，绑定过程非常轻松。 

* 点击文件![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/023043263.png)
* 添加项目![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/023116826.png)
* 输入仓库地址
* ![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/023129832.png)

- ### 绑定完成后是项目配置。Vercel会自动识别开发框架，这里可以自定义编译代码和输出文件夹，你可以在编译代码中添加自己的逻辑；**使用内置框架一般不要修改输出文件夹**。 

- 配置完成后点击`Deploy`，耐心等待即可

- 等待一会vercel就部署成功了

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/023312020.png)

- 点击visit通过浏览器访问

![mark](http://qdraqx6e2.bkt.clouddn.com/blog/20200722/023411471.png)





<body oncontextmenu="return false" onselectstart="return false" oncopy = "return false">