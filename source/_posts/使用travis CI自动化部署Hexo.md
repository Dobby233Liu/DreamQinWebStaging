---
title: 使用travis CI自动化部署Hexo
date: 2017-09-02 09:57:59
tags: Hexo
---
> 教程为本人留存，其中有步骤的简化，有问题邮箱联系我 616099456@qq.com

> 文章思路借鉴了网上文章，如有雷同，不要见怪


# 好处

花费这么大精力到底是为了什么呢？

1. 换了电脑、换了工作环境、重装系统之后可以迅速恢复状态，发布博客。
2. 备份了博客的源码和网页。
3. 当仓库push后自动部署，不用手动发布。

# 缺点
1. 当然是开始时变得麻烦了，我一开始弄的时候各种错误差点放弃了
2. 博客的源码公开了，当然这也没什么大不了的，我相信没谁愿意去看我的源码。

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

## 日常操作流程
```
git add .  
git commit -m "new post" 
git push

```

# 先写到这里，占个坑，有时间补齐
[ ](http://www.jianshu.com/p/5691815b81b6)
[ ](https://zhuanlan.zhihu.com/p/26625249?utm_source=weibo&utm_medium=social)


