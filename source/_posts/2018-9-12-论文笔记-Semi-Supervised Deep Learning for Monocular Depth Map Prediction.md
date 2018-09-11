---
title: 2018-9-12-论文笔记-Semi-Supervised Deep Learning for Monocular Depth Map Prediction
tags: 
 - 论文
categories: 
 - 论文
comments: true
updated: false
author: 张学志
date: 2018-9-3 7:30:39
grammar_cjkRuby: true
---

> 本文分析了论文：Semi-Supervised Deep Learning for Monocular Depth Map Prediction
<!-- more -->。

## 贡献
* 提出了一个半监督的深度估计算法：有监督loss + 无监督loss。

## 分析
* 激光雷达数据的问题：
	* 稀疏
	* 噪声的影响
	* 标定不准确的影响
* 有监督loss 和 无监督loss：
	* 使用激光雷达获取的稀疏的有效点做有监督loss训练。smooth_l1。
	* 使用其它的像素点构建无监督loss。通过左右图像 + warp一致构建loss。
	* 为了保证边缘的锐利度，根据边缘有构建了一个loss。
* 

* 算法框架和无监督的双目算法基本一致，只是加了有监督loss，变成了半监督算法。
![算法框架](https://www.github.com/xuezhisd/xuezhisd.github.io.img/raw/dev/imgs/1536709268593.png)
* 损失函数没有什么新意，在其他论文中都有出现。不管是有监督的smooth_l1，还是无监督loss。
* 评价准则也是常用的评价方法。
* ~~~除了半监督，没啥新奇的地方。~~~