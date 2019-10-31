# 利用 Github Pages 创建个人网站

1. 在网站上注册帐号 [https://github.com/](https://github.com/) ；
1. Fork [https://github.com/jerryyum/jerryyum.github.io](https://github.com/jerryyum/jerryyum.github.io)；
1. 修改项目名字，进入 `Settings`，将项目名字修改为：`username.github.io`；
1. 经过上面几个步骤，你的 github pages 已经建好了，等待大约一分钟，在浏览器上输入地址 `username.github.io`，这就是你刚刚建好的个人网站了。


# 如何修改网站信息

使用 github pages 构建自己的个人网站的另外一个好处是：首先将 github上的项目 clone 到本地，我们可以直接修改本地仓库然后通过 git 的一些操作，直接修改网站内容。

在前面已经提过，我使用的是基于Jekyll 的 `Next` 主题，如果要修改主题，建议阅读下面给出的 `Next` 使用文档，修改你电脑里 `username.github.io 文件夹里的 `config.yml` 文件。
Next 的 github 地址：https://github.com/Simpleyyt/jekyll-theme-next
Next 的使用文档：http://theme-next.simpleyyt.com

修改完后，打开命令行，输入 `cd username.github.io` 命令进入文件夹；
输入 `git add .`
再输入 `git commit -m "message"`
最后输入 `git push` 即完成了从本地仓库到远程 github 仓库的推送。

等待几分钟后再次键入 `username.github.io` 网址即可查看已经修改过的主题内容。


# 写博客

如果想要发表一篇博文，直接在 `_post` 文件夹下放置即可，这里对博文的格式有要求：
1. 博文必须为 `md` 格式(`markdown` 语法书写)，博文的文件名必须是`2018-2-12-name.md` 这样的格式；
1. 博文开头也有格式要求，比如像这样：
```
---
published: true
title: Web Scraping With Python Chapter 1 Learning notes
category: Python
tags:
- Web Scraping
layout: post
---
```
`published` 属性是此篇博文的可见性
`title` 是标题
`category` 是目录
`tag` 是标签
读者只需知道每篇博文必须这样开头，然后在下面使用 Markdown 语法书写博文即可。


# 关于 github pages

github pages 的官方文档：https://pages.github.com。
github pages 免费为我们提供了服务器，并提供了300M的免费空间供我们使用，我们可以通过 git 的相关操作。
github pages 使用了 `Jekyll` 服务器，Jekyll的中文官网：http://jekyllcn.com/。
