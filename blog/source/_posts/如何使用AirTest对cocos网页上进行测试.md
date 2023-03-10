---
title: 如何使用AirTest对cocos网页上进行测试
date: 2023-03-01 14:22:02
tags: airtest 自动化测试
categories: App自动化测试之Airtest
---
#前言少述
```
本来想用selenium 但是发现不能节点定位 暂用Airtest
```
# 前置环境准备（我默认使用chrome）
{% folding yellow, 浏览器驱动确认、python %}
1、AirTest有自带chromedriver驱动(确认版本确认、IDE的路径设置正确)   版本错误或者没有   启动程序将会报驱动错误
2、python以及环境配置完成
{% endfolding %}
先上手有需要再安装
##开始上手（进入IDE新建好对应项目或者功能目录）
AirTest用的也是selenium写法所以需要先引入相关 库
```
from selenium import *

```

