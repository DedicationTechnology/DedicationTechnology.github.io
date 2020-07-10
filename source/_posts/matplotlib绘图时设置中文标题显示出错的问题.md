---
title: matplotlib绘图时设置中文标题显示出错的问题
top: false
cover: false
toc: true
mathjax: true
date: 2020-07-10 21:17:20
password:
summary: matplotlib绘图时设置中文标题显示出错的问题
tags:
- 大数据
- 数据可视化
- matplotlib
categories: 大数据
---

在代码中输入如下代码即可解决

```python
#解决中文显示问题
plt.rcParams['font.sans-serif']=['SimHei']
plt.rcParams['axes.unicode_minus'] = False
```

