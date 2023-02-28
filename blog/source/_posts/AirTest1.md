---
title: AirTest（一）：了解、安装
date: 2023-02-27 20:32:19
tags: airtest
categories: App自动化测试之Airtest
---
#什么是Airtest
由 Airtest框架、poco框架、airtestIDE组成的测试套件
```  
Airtest是网易出品的一款基于图像识别和poco控件识别的一款跨平台的UI自动化测试工具。
适用于游戏和App(本质上就是网易自己为了给游戏做自动化测试开发出来的一套框架)。
后期又渐渐支持Windows和Android平台，iOS平台。 
Airtest提供了跨平台的AP1，包括安装应用、模拟输入、断言等。
甚于图像识别技术定位UI元素，你无需嵌入任何代码即可进行自动化测试。
测试脚本运行后可以自动生成详细的HTML测试报告，让你迅速定位失败的测试点。
AirtestIDE 是一个强大的GUI工具，可以帮助你录制和调试测试脚本"
```
##appium和 airtest的区别
| <font color="red">**工具**</font> | Appium  | Airtest                 |
|---------------------------| -------- |-------------------------|
| **安装** | 中等 | 简单                      |
| **支持**                    | Android、IOS、H5 | Android、IOS（需要MAC🙂）、H5 |
| **公司使用率**                 | TOP1 | 逐步在增加？                  |
| **相关资料**                  | 多 | 少                       |
| **上手难度**                  | 中等 | 一般但是没资料烦人               |
| **测试报告**                  | 有 | 有                       |
| **CI支持**                  | 支持 | 支持                      |
| **Web支持**                 | 支持 | 支持                      |

## airtest的优缺点
{% folding yellow, 优点 %}
1.Airtest操作比较简单，甚本上不涉及到代码，所以非常适合刚入门没什么测试经验的人利用这个工具做UI自动化测试，同时Airetest又提供了开源的API，让资深测试工程师可以基于Airtest的框架上再做高级的定制化扩展功能,
2.甚于图像识别和UI控件识别功能简单
3.支持python进行个性化脚本编程
4.可录制脚本一键生成报告
{% endfolding %}
{% folding red, 缺点 %}
1.如果经常使用图像识别脚本会产生大量的图片，会让脚本整体观感不太好(个人意见)
2.目前相关技术文档不多，需要自己去官网或社区探索
3.有时元素无法定位或者会产生未期待的错误
{% endfolding %}





# Airtest安裝
[官網地址](https://airtest.netease.com/) {% tip warning faa-horizontal animated %}下載後壓縮的路徑不要含有中文{% endtip %}
# 啓動
找到解壓的 AirTest目錄 雙擊 AirtestIDE.exe 虽然现在启动了意义不大
{% tip warning faa-horizontal animated %}！！如果启动后黑屏或者闪退可以 更改兼容模式        选项 》  setting    》兼容模式   》 更改选项进行尝试
选择OK之后 需要重启{% endtip %}
#安卓连接
##连接步骤
<img src="/img/airtest/9acf8ca0-d1d1-4153-981a-0b9e46123afe-14592612.jpg" alt="示例图片" style="zoom:50%;" />
连接之后可操作可通过Android Assistant进行快速的apk安装卸载   以及  更换输入法
用法参考： https://mp.weixin.qq.com/s/EH0aQnr2AwG0MmFdgoE7mw
{% tip info %}！！连接不上  需要检查 1：IDE是否为最新版本    2：核对是否有设置没开启    3：确认ADB是否正常连接设备     4：检查手机是否安装上Yosemite 并设置为当前输入法
输入法apk以及adb   路径：Airtest\AirtestIDE\airtest\core\android\static
Android连接常见问题官方文档👇
 https://airtest.doc.io.netease.com/IDEdocs/device_connection/2_android_faq/{% endtip %}

#安卓模拟器的连接
<img src="/img/airtest/ad63337a-ccb9-4cb1-873a-308970d06889-14592612.jpg" alt="示例图片" style="zoom:50%;" />
##常见模拟器连接参数及问题
{% folding cyan close, 点击查看详情 %}
遇到黑屏报错首先尝试选择其他的连接参数
<img src="/img/airtest/afa0b757-ff80-49a1-a410-b074777c2a10-14592612.jpg" alt="示例图片" style="zoom:50%;" />
<img src="/img/airtest/d53ea7df-9ad5-4792-982b-64a981a54c65-14592612.jpg" alt="示例图片" style="zoom:50%;" />
{% endfolding %}

#使用脚本的形式连接真机
{% folding cyan close, 点击查看详情 %}
<img src="/img/airtest/47f68b75-7051-4f97-924a-18f302b2acc4-14592612.jpg" alt="示例图片" style="zoom:50%;" />
<img src="/img/airtest/8448d352-c0bd-4cb2-bade-c855790a4e4f-14592612.jpg" alt="示例图片" style="zoom:50%;" />
{% endfolding %}

#连接Windows窗口（待补充）
