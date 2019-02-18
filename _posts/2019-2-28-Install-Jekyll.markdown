---
layout: post
title: "用Jekyll + Github Pages 搭建博客(1)"
date: "2019-02-18 12:14:15"
categories: "安装"
tags: Jekyll
---

# Ubuntu 18.04 安装Jekyll
一时兴起，想自己搭建个博客，在网上看见好多人用Jekyll+Github Pages, 也手动自己弄了个。看着很简单，没想到都是坑，特别是自己写主题。在此记录，这次建博的心路历程。
在Windows上安装Jekyll出错了，不想纠缠，就直接换成Ubuntu系统了。

<br>
Jekyll是基于ruby来生成静态网页的，所以要先安装ruby。
<br>
1.安装Ruby：
```shell
$ sudo apt-get install ruby-full
```
<br>
2.用gem安装Jekyll

```shell
$ gem install bundler jekyll
```
<br>
查看一下Jekyll的版本
```shell
$ jekyll -v

jekyll 3.8.5
```
<br>
3.安装完毕，可以用jekyll创建博客了。
```shell
$ jekyll new my-site 
```
<br>
创建了新的项目，然后开始生成静态网页。
```shell
$ cd my-site
~/my-site$ bundle exec jekyll serve
```
<br>
然后就可以在浏览器中输入http://localhost:4000；
<br>
看见Jekyll的默认样式网页，代表安装成功了。

