---
title: 【Hexo搭建集合】之快速免费搭建个人博客
tags: HEXO
categories:
  - HEXO
  - GitHub
abbrlink: 14d47894
date: 2020-07-20 17:09:49
cover:
top: true
top_img:
---

{% blockquote Seth Godin http://sethgodin.typepad.com/seths_blog/2009/07/welcome-to-island-marketing.html Welcome to Island Marketing %}
Every interaction is both precious and an opportunity to delight.
{% endblockquote %}
{% blockquote @DevDocs https://twitter.com/devdocs/status/356095192085962752 %}
NEW: DevDocs now comes with syntax highlighting. http://devdocs.io
{% endblockquote %}
{% blockquote David Levithan, Wide Awake %}
Do not just seek happiness for yourself. Seek happiness for all. Through kindness. Through mercy.
{% endblockquote %}
{% codeblock [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcodeblock %}
{% codeblock lang:objc %}
[rectangle setX: 10 y: 10 width: 20 height: 20];
{% endcodeblock %}
<% for (var link in site.data.menu) { %>
  <a href="<%= site.data.menu[link] %>"> <%= link %> </a>
<% } %>

<ol>
<li>你好！</li>
<li>看什么看</li>
<li>我很帅吗！！！</li>
</ol>
使用方法一：
<div class='tip' ><p>默认情况<p></div>
<div class='tip success'><p>success<p></div>
<div class='tip error'><p>error<p></div>
<div class='tip warning'><p>warning<p></div>
使用方法二：
<div class='tip font5 fas fa-atom'><p>自定义font5图标<p></div>
<div class="tip wtgo font5 fas fa-bolt"><p>魔改标签1</p><p></p></div>
<div class="tip ban font5 fas fa-ban"><p>魔改标签2</p><p></p></div>
<div class="tip home font5 fas fa-home"><p>魔改标签3</p><p></p></div>
<div class="tip important font5 fas fa-home"><p>魔改标签4</p><p></p></div>
<div class="tip ref font5 fas fa-sync"><p>魔改标签5</p><p></p></div>
<div class="tip ffa font5 fas fa-cogs"><p>魔改标签6</p><p></p></div>
<div class="tip key font5 fas fa-key"><p>魔改标签7</p><p></p></div>
<div class="tip socd font5 fas fa-bell"><p>魔改标签8</p><p></p></div>
<div class="tip qq font5 fab fa-qq"><p></p><p></p></div>

使用方法三：
<div class="tip wtgo"><p>文字</p><p></p></div>
<div class="tip ban"><p>文字</p><p></p></div>
<div class="tip home"><p>文字</p><p></p></div>
<div class="tip important"><p>魔改标签4</p><p></p></div>
<div class="tip ref"><p>魔改标签5</p><p></p></div>
<div class="tip ffa"><p>魔改标签6</p><p></p></div>
<div class="tip key"><p>魔改标签7</p><p></p></div>
<div class="tip socd"><p>魔改标签8</p><p></p></div>
<div class="tip qq"><p>魔改标签9</p><p></p></div>
