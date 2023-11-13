---
title: git命令
date: 2023-11-11 22:09:49
tags:
  - 博客
  - git
category: git
cover: /images/backgroundFriend.png
ai:
  - 本教程介绍了如何在博客中安装基于Hexo主题的安知鱼主题，并提供了安装、应用主题、修改配置文件、本地启动等详细步骤及技术支持方式。教程的内容针对最新的主题版本进行更新，如果你是旧版本教程会有出入。
  - 本文真不错
---
# git命令

## 1.提交代码时提交者的名字查看与更改

查看名字：git config user.name

更改名字：git config --globle user.name“ xxxxx”

## 2.提交代码的顺序

1.同步远程仓库代码：git pull

2.查看当前状态（就是看你修改了哪些文件）：git status

3.提交代码到本地git缓存区：git  add.

4.推送代码到本地git库： git  commit -m “提交代码的名字”

5.提交本地代码到远程仓库：git push

```javascript
1.git stash //隐藏当前工作的修改,如果不隐藏自己修改的半成品代码，就会发生切换到别的分支后，将然后自己的半成品代码带入其他分支，这样就发生很多不必要的麻烦。
2.git pull
3.git stash pop //恢复隐藏的工作信息，同时删除隐藏的工作信息
4.解决冲突
5.git add . 将修改后的冲突文件再加入暂存区
6.git commit
7.git push
```



## 3.代码回滚（当你的提交出现错误时）

1.

```javascript
.git reset --hard HEAD^ //撤回到上上级
```

2.

```javascript
.git reset --hard HEAD //撤回到上级
```

3.

```javascript
git reset --hard HEAD~3//撤回到第三级
```

## 4.常见的一些指令

- git ls-files -----查看缓存区缓存了哪些文件
- git status -s -----查看文件的状态
- git rm --cached 文件名 -----将某个文件移除缓存区
- git add 文件名 -----将某个文件存入缓存区
- git add . -----将所有文件存入缓存区
- git log --oneline -----查看当前提交了多少次记录
- git reflog --oneline -----查看所有的日志
- git reset --hard 版本号 -----强制覆盖暂存区和工作区的命令
- git branch 分支名 ----创建分支命令
- git checkout 分支名 ----切换分支命令
