---
layout: "../../layouts/MarkdownPost.astro"
title: "一个成熟的Git工作流"
pubDate: 2024-06-27
description: "一个成熟的Git工作流"
author: "Kaemon"
cover:
  url: "https://jsd.cdn.zzko.cn/gh/AEDELSTAN/picx-images-hosting@master/Pictures/Blogs/The-Boy-and-the-Heron-1.7p2jladte.webp"
  square: "https://jsd.cdn.zzko.cn/gh/AEDELSTAN/picx-images-hosting@master/Pictures/Blogs/The-Boy-and-the-Heron-1.7p2jladte.webp"
  alt: "cover"
tags: ["Git", "工作流", "效率"]
theme: "dark"
featured: false
---

### 一个成熟的 Git 工作流

1.```git clone <url>```到本地

2.git checkout -b <xxx> 切换至新分支 xxx

3.修改或者添加本地代码（部署在硬盘的源文件上）

4.git diff 查看自己对代码做出的改变

5.git add 上传更新后的代码至暂存区

6.git commit 可以将暂存区里更新后的代码更新到本地 git

7.git push origin xxx 将本地的 xxxgit 分支上传至 github 上的 git

### 如果在写自己的代码过程中发现远端 GitHub 上代码出现改变）

1.git checkout main 切换回 main 分支

2.git pull origin master(main) 将远端修改过的代码再更新到本地

3.git checkout xxx 回到 xxx 分支

4.git rebase main 我在 xxx 分支上，先把 main 移过来，然后根据我的 commit 来修改成新的内容（中途可能会出现，rebase conflict -> 手动选择保留哪段代码）

5.git push -f origin xxx 把 rebase 后并且更新过的代码再 push 到远端 github 上

6.原项目主人采用 pull request 中的 squash and merge 合并所有不同的 commit

远端完成更新后
1.git branch -d xxx 删除本地的 git 分支

2.git pull origin master 再把远端的最新代码拉至本地

3.git push origin --delete xxx 删除远端的 git 分支

4.git branch -D xxx 强制删除本地的 git 分支

5.git push origin --delete xxx 强制删除远端的 git 分支

6.git gc --aggressive 清理本地仓库垃圾