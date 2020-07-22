---
title: 【每日一更】之Hexo配置豆瓣电影
tags:
  - movies
  - music
  - book
categories:
  - HEXO
  - 豆瓣
abbrlink: fd529351
date: 2020-07-20 00:06:29
cover:
top:
top_img:
---

## 第一章

##安装模块依赖

 我们使用时可以先安装依赖模块，在 `GitBash` 中使用以下命令 

```java
//命令行位置：hexo根目录
$ npm install hexo-douban --save
```

## 站点配置文件中添加配置

 然后我们再在 Hexo 站点根目录配置文件 `_config.yml` 中的末尾添加如下配置： 

```yml
douban:
  user: mythsman
  builtin: false
  book:
    title: 'This is my book title'
    quote: 'This is my book quote'
  movie:
    title: 'This is my movie title'
    quote: 'This is my movie quote'
  game:
    title: 'This is my game title'
    quote: 'This is my game quote'
  timeout: 10000
```

# 上面参数说明：

- user: 你的豆瓣 ID。打开豆瓣，登入账户，然后在右上角点击 “个人主页” ，这时候地址栏的 URL 大概是这样：`https://www.douban.com/people/xxxxxx/` ，其中的 `xxxxxx` 就是你的个人ID了。
- builtin: 是否将生成页面的功能嵌入 hexo s 和 hexo g 中，默认是 false,另一可选项为 true(1.x.x版本新增配置项)。
- title: 该页面的标题.
- quote: 写在页面开头的一段话,支持html语法.
- timeout: 爬取数据的超时时间，默认是 10000ms ,如果在使用时发现报了超时的错(ETIMEOUT)可以把这个数据设置的大一点。

由于 `hexo-douban` 是默认抓取豆瓣读书、豆瓣电影以及豆瓣游戏的，如果只想要其中一部分，可以把其它部分在上述配置文件中去掉即可。

## 启动

那么我们如何去使用这个呢？



我们只需要在 `GitBash` 中输入以下命令：`hexo clean && hexo douban -bgm && hexo g && hexo s` 即可，注意其中开启 `hexo-douban` 的命令中，`-bgm` 代表的是 `book、game、movie` 三个参数，如果只需要其中的一部分就只带你想要的那些参数。

- [ ]  **另外注意的是，由于 hexo douban 的简写是 `hexo d`，与 `hexo deploy` 的简写指令 `hexo d` 冲突，因此在进行二者部署的时候，只能都打全名而不能打简写形式。** 

##测试

 部署
如果上述都没有问题，我们就可以在菜单栏中添加按钮了，打开主题配置文件`_config.xml`，找到菜单按钮，可以选择性的添加下面内容： 

```yml
menu:
  home: /
  archives: /archives
  books: /books     # 这是链接到books页面
  movies: /movies   #  这是链接到movies页面
  games: /games   # 这是链接到games页面
```

注意添加完成之后按钮并不是中文的，这是由于在 `languages` 文件夹下面的 `zh-CN`（中文语言配置文件）没有添加上述对应的中文参数信息，所以我们需要主动添加。

语言文件夹在你的主题配置文件夹下面，比如我的是使用的 next 主题，则是在 `E:\blog\hexo\themes\next\languages` 目录下，找到 `zh-CN` 文件，在 `menu` 菜单下添加：

~~~yml
menu:
  books: 阅读
  movies: 电影
  games: 游戏
~~~

