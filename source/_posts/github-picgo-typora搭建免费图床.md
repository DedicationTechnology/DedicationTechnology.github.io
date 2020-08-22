---
title: github+picgo+typora搭建免费图床
top: true
cover: false
toc: true
mathjax: true
date: 2020-07-05 20:07:50
password:
summary:
tags: 
- github
- typora
- picgo
categories: 图床
---

#### 1.搭建目的

> 由于typora是一款备受好评的markdown编辑器，大多数人选择在typora上编写markdown然后直接复制到其他的平台进行发布：例如CSDN这类博客又或者是自己搭建的博客(比如用hexo框架搭建的)，又或者是直接上传到GitHub中作为笔记。但这些方式都有一个非常大的弊端，那就是在typora上插入的本地图片一旦上传到其他的平台就无法显示，这里搭建github+picgo+typora的目的就是为了解决这些问题。

#### 2.尚未解决的问题

> 这种github+picgo+typora搭建方法最终得到的图片还无法在CSDN上直接显示，会有防外链的提示，所以在CSDN上发布博客的话目前还是建议直接本地图片上传，在自己搭建的博客或者上传到GitHub上这种方法是可以完美显示图片的。

#### 3.其他方法推荐

> 如果你不想用这种方法来搭建的话，也可以直接用在线免费的图床上传图片，不过会有一些相关限制，这里推荐一个图床：https://imgchr.com/ ，具体操作方法请自行谷歌。

#### 4.搭建步骤

1. 下载picgo：https://github.com/Molunerfinn/picgo/releases ，（请下载2.2.2及以上版本），然后傻瓜式安装即可。

2. 配置github仓库

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/4.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/3.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/6.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/5.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/7.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/9.jpg)

3. 配置picgo

   ![8](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/8.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/10.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/11.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/12.jpg)

4. 配置typora

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/13.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/14.jpg)

   最后如果验证成功就表示可以成功上床图片，到这里搭建就全部完成了

5. 实操

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/15.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/16.jpg)

   ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/17.jpg)

   到这里，搭建的功能就完成了，现在直接将typora的内容上传到自己搭建的博客或者github上就会显示图片

   #### 5.踩过的坑

   1. 你保存的图片不能同名，也就是说github中不能有和你即将在typora粘贴的图片同名的图片，同名会导致上传失败。

   2. 由于github的不稳定，毕竟服务器在国外，偶尔会出现上传失败的问题，如果经过检查发现不是图片同名的问题可以考虑刷新github，然后重新上传图片，或者过一会在上传

      ![](https://raw.githubusercontent.com/DedicationTechnology/picgo/master/img/18.jpg)