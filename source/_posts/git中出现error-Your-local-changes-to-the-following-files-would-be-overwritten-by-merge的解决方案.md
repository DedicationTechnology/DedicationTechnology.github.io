---
top: false
cover: false
toc: true
mathjax: true
date: 2020-07-05 19:58:46
password:
summary: git中出现error Your local changes to the following files would be overwritten by
  merge的解决方案
tags: 
- git
- github
categories: git
---

#### 1.错误说明

> 这句代码的意思是以本地进行的修改会被覆盖，也就是说你本地进行的修改不会生效。

#### 2.错误起因

> 一般是使用了git pull相关的命令同步远程仓库到本地引起的，而本地的修改无法上传到远程仓库，导致两者都不能兼备

#### 3.解决方案

```bash
git stash  # 备份当前的工作区的内容，让工作区保证和上次提交的内容一致。同时，将当前的工作区内容保存到Git栈中
git commit
git stash pop  # 从Git栈中读取最近一次保存的内容，恢复工作区的相关内容
在终端下依次输入上述代码就可以让服务器上的代码更新到了本地，而且你本地修改的代码也没有被覆盖
之后使用add，commit，push命令即可更新本地代码到服务器
```

