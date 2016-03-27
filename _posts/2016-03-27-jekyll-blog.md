---
layout: post
title: "github+jekyll 搭建静态博客"
categories: jekyll
comments: true
---
为了提升一下level以及管理好自己的技术文章，学习使用了jekyll搭建自己的博客并将其托管到github上。

在网上搜了好多文档，但是大多数都不是完全正确而且是关于jekyll老版本的，于是决定自己写一篇博客简介一下。

将整个blog的搭建概括为以下几个步骤：

- 安装（Ruby，RubyGems，jekyll）

- jekyll new myblog，会生成jekyll自带的一些文件

- jekyll build; jekyll serve; 编译文件并开启jekyll服务

  可通过[http://localhost:4000/](http://localhost:4000/)访问默认博客
  
- 查找自己喜欢的jekyll模板样式进行替换

以上完成了在本地博客的搭建，接下来就是将其托管到github上，实现远程的同步。因为github提供了这个功能，username.github.io就是自己的博客地址。

- 本地git init, git add, git commit, 在github上创建一个名为panhe.github.io的仓库（注意要在master分支上）

- git remote add origin git@github.com:panhe/panhe.github.io.git

  git push origin master 实现数据的远程同步
  
- [http://panhe.github.io](http://panhe.github.io)访问到博客


jekyll具备文本格式转换的功能，我们编辑的都是markdown，textile等的格式，它可以转换成HTML格式。

我们编写的文章都存储在_posts文件夹中，按照年-月-日-标题.md的格式，头信息中的category字段表明了该文章所属的分类。



下面列出几个不错的链接：

- jekyll官网：[http://jekyll.bootcss.com/](http://jekyll.bootcss.com/)

- jekyll模板：[http://jekyllthemes.org/](http://jekyllthemes.org/)


