---
title: 2018-9-11-配置小书匠的hexo blog模板
tags: 
 - 新建
categories: 
 - 未分类
comments: true
updated: false
author: 张学志
date: 2018-9-2 20:56:27
grammar_cjkRuby: true
---

> 本文描述了：**如何配置小书匠的模板，适用于hexo blog。**
<!-- more -->



```
---
title: <% print((new Date()).getFullYear().toString()+ '-'+ ((new Date()).getMonth() + 1).toString() + '-'+ (new Date()).getDate().toString()); %>-未命名
tags: 
 - 新建
categories: 
 - 未分类
comments: true
updated: false
author: 张学志
date: <% print((new Date()).getFullYear().toString()+ '-'+ ((new Date()).getMonth() + 1).toString() + '-'+ (new Date()).getDay().toString() + ' ' + (new Date()).getHours().toString() + ':' + (new Date()).getMinutes().toString() + ':' + (new Date()).getSeconds().toString()); %>
grammar_cjkRuby: true
---

> 本文描述了：
<!-- more -->

```