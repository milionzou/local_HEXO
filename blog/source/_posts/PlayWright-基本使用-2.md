---
title: PlayWright-基本使用(2)
date: 2023-03-10 18:24:43
tags: Web自动化测试
categories: Web自动化测试之微软新宠儿--PlayWright
cover: https://cdn.staticaly.com/gh/milionzou/pic_bed@main/img/playwrightLogo.webp
---
# 初期闯关前需要准备(要导入的库)
{% folding blcak, 常用库 %}
playwright.async_api        #异步 
playwright.sync_api         #同步
{% endfolding %}

### 起手式
```commandline
with sync_playwright() as p:  #初始化对象   #异步的话需要特别定义说明 
    browser = p.chromium.launch(headless=False)          # False：正常模式启动 chromium 浏览器   True：无头模式
    #之后 browser相当于一个浏览器对象
    page = 对象.new_page      #创建一个页面  可以创建多个
    页面.goto("URL")      #打开一个页面
    
```

### 异步起手式
```commandline
#异步的话需要特别定义说明
例如 
async def main():
    async with async_playwright() as p
```