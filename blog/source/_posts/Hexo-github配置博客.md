---
title: Hexo+github配置博客
date: 2017-12-20 14:07:33
tags: tools
category: tec
---

### 安装git
### 安装Hexo
```
$ cd d:/hexo
$ npm install hexo-cli -g
$ hexo init blog
$ cd blog
$ npm install
$ hexo g # 或者hexo generate
$ hexo s # 或者hexo server，可以在http://localhost:4000/ 查看
```

这里有必要提下Hexo常用的几个命令：

```
hexo generate (hexo g) 生成静态文件，会在当前目录下生成一个新的叫做public的文件夹

hexo server (hexo s) 启动本地web服务，用于博客的预览

hexo deploy (hexo d) 部署播客到远端（比如github, heroku等平台）
```

另外还有其他几个常用命令：
```
$ hexo new "postName" #新建文章
$ hexo new page "pageName" #新建页面
```
常用简写
```
$ hexo n == hexo new
$ hexo g == hexo generate
$ hexo s == hexo server
$ hexo d == hexo deploy
```
常用组合
```
$ hexo d -g #生成部署
$ hexo s -g #生成预览
```
现在我们打开http://localhost:4000/ 已经可以看到一篇内置的blog了。

### Github Pages设置

[GitHub Pages](https://pages.github.com/) 本用于介绍托管在GitHub的项目，不过，由于他的空间免费稳定，用来做搭建一个博客再好不过了。

每个帐号只能有一个仓库来存放个人主页，而且仓库的名字必须是username/username.github.io，这是特殊的命名约定。你可以通过http://username.github.io 来访问你的个人主页。

这里特别提醒一下，需要注意的个人主页的网站内容是在master分支下的。

### 部署Hexo到Github Pages
### 使用hexo deploy部署发布文章
### Hexo主题配置
#### 添加about页面
