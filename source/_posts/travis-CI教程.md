---
title: travis CI教程
thumbnail: ''
top: false
date: 2017-09-03 16:51:24
tags:
categories:
description:
---
# 思路
将Hexo源码和发布代码放到一个仓库的不同分支：
- 一个分支存放部署后的网页（master）
- 一个分支存放博客的源码（blog-source）

# 具体操作
## 整体流程
1. 新建仓库，为了方便我们可以将仓库名命名为 username.github.io，其中username是你的github的id
1. 创建一个新分支：blog-source
1. 将blog-source设置为默认分支。在仓库的 settings->Branches->Default branch中设置。
1. 将仓库clone到本地
1. 在本地安装Hexo
