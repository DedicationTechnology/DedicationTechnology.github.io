---
title: hexo博客的恢复
top: false
cover: false
toc: true
mathjax: true
date: 2020-08-18 21:00:52
password:
summary:
tags:
- 博客
categories: 博客
---

### 1. 博客恢复

1. 说明：这里博客的恢复是基于你之前备份了博客且每次添加文章之前都备份到GitHub的备份分支中

2. 这里GitHub中有两个分支：backup和master，前者用于备份博客后者用于生成博客静态文件，其中以将backup设置为默认分支

   - 安装好git、nodejs、npm、hexo

     说明：Mac下git安装：http://sourceforge.net/projects/git-osx-installer/

     ​			Mac下nodejs安装：直接去官网下载对应的安装包
   
     ​			Mac下npm默认已经安装，需要安装cnpm，然后用cnpm安装hexo

     ​			Mac下cnpm安装：在root下进行安装，否则会报错

     ​				$ npm install -g cnpm --registry=https://registry.npm.taobao.org
   
     ​			Mac下hexo安装：在root下进行安装，否则会报错
   
     ​				cnpm install -g hexo-cli
   
   - 克隆博客
   
     ```bash
     git clone https://github.com/DedicationTechnology/DedicationTechnology.github.io.git blog
     ```
   
   - 进入本地的博客目录(这里就是上面目录创建的blog目录)然后利用package.json文件安装相关的插件
   
     ```bash
     npm install
     ```

### 2. 正常博客的备份和发表顺序(以下命令都在backup分支下进行)

```bash
hexo n # 生成一个新的博客
git add  # 添加到本地工作台
git commit -m ""  # 添加到本地仓库
git push origin backup  # 上传到github仓库中的备份分支backup中
hexo clean
hexo g  # 生成博客文件
hexo s  # 开启本地博客预览
hexo d  # 上传博客静态文件到GitHub
```

