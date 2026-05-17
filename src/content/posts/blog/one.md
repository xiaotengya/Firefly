---
title: one
published: 2026-05-03
updated: 2026-05-03
description: 这是第一篇文章
image: ./cover.jpg
tags:
  - one
category: one
draft: false
author: jyzft
---


####  **如何更优雅的用obsidian写博客，图床在obsidian怎么使用，以及个人心得**



## Obsidian Git 插件 说明

|图标|功能名称|对应 Git 操作|作用说明|
|:--|:--|:--|:--|
|⬆️（圆圈内上箭头）|提交并同步|`git commit + git push`|一键提交并推送，适合快速备份笔记|
|✔️|提交变更|`git commit`|仅提交暂存区的修改，不推送到远程|
|➕|暂存所有|`git add .`|把所有修改文件加入暂存区|
|➖|取消暂存所有|`git reset HEAD`|把暂存区的文件恢复到未暂存状态|
|📤（方框内上箭头）|推送|`git push`|把本地提交推送到远程仓库|
|📥（方框内下箭头）|拉取|`git pull`|从远程仓库拉取最新内容|
|📁|打开仓库目录|-|在文件管理器中打开 Obsidian 库的 Git 根目录|
|🔄|刷新状态|`git status`|刷新界面，重新检测文件变更|

- 中间的 `vault backup: {{date}}` 是**提交信息模板**，`{{date}}` 会自动替换成当前日期 / 时间，你可以改成自己习惯的格式（比如 `backup: {{date:YYYY-MM-DD HH:mm}}`）。
- 下方的 `Staged Changes` 是「已暂存的修改」，`Changes` 是「未暂存的修改」，文件后面的 `+M` 表示文件是**新增 / 修改状态**。


## cf imagebed 插件说明


## Q: 如何通过PicGo上传？

- PicGo插件设置中搜索`web-uploader`，安装可自定义前缀的版本，如图：
    
    ![PicGo插件设置](https://cfbed.sanyue.de/images/qa/picgo-plugin.png)
    
- 打开`图床设置`->`自定义Web图床`->`Default`，然后按照下图方式配置，注意API地址和自定义图片URL前缀按照自己的域名进行修改。（**如果设置了`AUTH_CODE`，一定以`?authCode=your_authCode`的方式添加到API地址后面**）：
    
    ![图床设置](https://cfbed.sanyue.de/images/qa/picgo-config.png)
    
- 设置完成，确定即可使用PicGo上传到自建的图床。


图床随机图的使用

https://tu.fqzlr.com/random?type=img&dir=beijing&orientation=auto

curl --location --request GET 'https://tu.fqzlr.com/random'

curl --location --request GET 'https://tu.fqzlr.com/random?orientation=landscape'

curl --location --request GET 'https://tu.fqzlr.com/random?dir=beijing&orientation=portrait'

curl --location --request GET 'https://tu.fqzlr.com/random?type=img&orientation=landscape'

<img src="https://tu.fqzlr.com/random?type=img&orientation=landscape" alt="随机背景">

.hero {
  background-image: url('tu.fqzlr.com/random?type=img&orientation=landscape');
  background-size: cover;
}

https://your.domain/random?type=img&dir=mobile&orientation=portrait