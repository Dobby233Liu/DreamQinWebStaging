---
title: mcmod开发教程
thumbnail: ''
comment: true
date: 2017-09-17 19:00:50
tags:
categories:
description:
---

1. 打开命令行并cd到解压zip文件的文件夹。
2. 在下载的材料文件夹中有一个命令窗口之后，键入：
`gradlew setupDecompWorkspace`
3. 打开IDEA，并导入项目。
4. 选择您的build.gradle文件并将其导入。
5. 完成之后，关闭IntelliJ并运行以下命令：
`gradlew genIntellijRuns`
6. 打开IDEA并导入项目
如果在在IDE中缺少库，或者遇到问题，可以运行
`gradlew  -  refresh-dependencies`
来刷新本地缓存。 

