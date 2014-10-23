---
layout: post
title: "my first octopress blog"
date: 2014-07-12 13:07:39 +0800
comments: true
categories: octopress
share: true
description: 搭建octopress blog
---

这个blog就是基于octopress的，想拥有自己的blog么？一起来吧~
<!--more-->

让我们一起来搭建一个属于自己的blog，step by step~

---

## 环境准备
1.安装ruby，1.9.3以上

``` bash
xiaolongyuan@xiaolongdeMacBook-Air ~$ ruby --version
ruby 2.0.0p451 (2014-02-24 revision 45167) [universal.x86_64-darwin13]
xiaolongyuan@xiaolongdeMacBook-Air ~$
```

2.下载octopress源码

``` bash
git clone git://github.com/imathis/octopress.git octopress
cd octopress  
```

3.安装源码所需的依赖包,编译octopress

``` bash
gem install bundler
bundle install
```

4.安装主题（rake install['themename']）默认主题不加themename

``` bash
rake install
```

5.在你的github中新建一个 yourname.github.io 的仓库（建议不要添加任何文件）

---

## 使用octopress写blog
1.设置目标仓库，以便让octopress知道push代码到哪里

``` bash
rake setup_github_pages
```

2.生成blog、预览blog、新建blog文章、提交代码

``` bash
rake generate
rake preview
rake new_post['article name']  
rake deploy
```

---

## 值得推荐的几个地址
安装类:

[http://blog.devtang.com/blog/2012/02/10/setup-blog-based-on-github/](http://blog.devtang.com/blog/2012/02/10/setup-blog-based-on-github/){:target="_blank"}
[http://justcoding.iteye.com/blog/1957617](http://justcoding.iteye.com/blog/1957617){:target="_blank"}

主题类:

[https://github.com/imathis/octopress/wiki/3rd-Party-Octopress-Themes](https://github.com/imathis/octopress/wiki/3rd-Party-Octopress-Themes){:target="_blank"}

BTW:我用的主题是[HPSTR](https://github.com/Z1MM32M4N/hpstr-theme){:target="_blank"}
