---
title: PlayWright-开始(1)
date: 2023-03-10 17:35:40
tags: Web自动化测试
categories: Web自动化测试之微软新宠儿--PlayWright
cover: https://cdn.staticaly.com/gh/milionzou/pic_bed@main/img/playwrightLogo.webp
---
为什么要学习
和selenium的区别
# 环境准备
### 安装 playwright：
```
pip install playwright
```
### 安装所需的浏览器 chromium,firefox 和 webkit：
```commandline
playwright install
```
# 简单使用
{% folding green, 启动浏览器并打开百度页面 %}
with sync_playwright() as p:
    browser = p.chromium.launch(headless=False)          # 启动 chromium 浏览器
    page = browser.new_page()              # 打开一个标签页
    page.goto("https://www.baidu.com")     # 打开百度地址
    print(page.title())                    # 打印当前页面title
    browser.close()
{% endfolding %}                           # 关闭浏览器对象