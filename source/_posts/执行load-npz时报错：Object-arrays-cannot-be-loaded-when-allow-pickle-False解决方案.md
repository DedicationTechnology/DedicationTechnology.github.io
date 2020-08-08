---
title: 执行load npz时报错：Object arrays cannot be loaded when allow_pickle=False解决方案
top: false
cover: false
toc: true
mathjax: true
date: 2020-07-10 20:45:11
password:
summary: 
tags: 
- 大数据
- 数据可视化
- matplotlib
categories: 大数据
---

1. 错误说明：np.load() 缺少allow_pickle的权限
2. 解决途径：在load方法中添加属性(修改allow_pickle为True)；np.load("npz路径", allow_pickle = True) 