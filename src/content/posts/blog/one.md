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
