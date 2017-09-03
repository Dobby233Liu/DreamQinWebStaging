---
title: Hexo博客搭建傻瓜教程
thumbnail: ''
date: 2017-09-02 09:57:59
tags: Hexo
top: true
---
> 文章思路借鉴了网上文章，如有雷同，十分正常。有问题邮箱联系我，页面左上角点开即可看到邮箱

使用travis CI自动化部署Hexo到github pages ，并使用腾讯云的cdn加速国内的访问

# 建立完成日常操作流程
```
hexo n 建立文件
git add .  
git commit -m "new post" 
git push

```

# Hexo的优点
> 摘自官网
![2017-09-03-16-55-50](http://ovhqars5t.bkt.clouddn.com/2017-09-03-16-55-50.png)
![2017-09-03-16-55-59](http://ovhqars5t.bkt.clouddn.com/2017-09-03-16-55-59.png)
![2017-09-03-16-56-06](http://ovhqars5t.bkt.clouddn.com/2017-09-03-16-56-06.png)
![2017-09-03-16-56-13](http://ovhqars5t.bkt.clouddn.com/2017-09-03-16-56-13.png)


# travis CI优处

1. 换了电脑、换了工作环境、重装系统之后可以迅速恢复状态，发布博客。
2. 备份了博客的源码和网页。
3. 当仓库push后自动部署，不用手动发布。

# 缺点
1. 当然是开始时变得麻烦了，我一开始弄的时候各种错误差点放弃了
2. 博客的源码公开了，当然这也没什么大不了的，我相信没谁愿意去看我的源码。




# 占个坑，有时间补齐详细教程
[ ](http://www.jianshu.com/p/5691815b81b6)
[ ](https://zhuanlan.zhihu.com/p/26625249?utm_source=weibo&utm_medium=social)


