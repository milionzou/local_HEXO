---
title: PlayWright-录制生成脚本(3)
date: 2023-03-14 11:57:30
tags: Web自动化测试
categories: Web自动化测试之微软新宠儿--PlayWright
cover: https://cdn.staticaly.com/gh/milionzou/pic_bed@main/img/playwrightLogo.webp
---

{% folding cyan close,运行 %}
- 在终端输入
- playwright codegen http://网站地址
- 正常打开之后会出现 一个浏览器窗口 一个是playwright inspector窗口
- 可以进行 记录测试、复制测试、清楚测试
- 可以更改测试语言
{% endfolding %}

{% folding cyan close, 运用 %}
- 一般选择 pytest代码 然后录制完成之后 复制代码
- test用例就需要在 test_开头的文件运行
- 在test_文件里粘贴后
- 安装插件： pip install pytest-playwright

{% endfolding %}