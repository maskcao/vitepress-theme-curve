---
title: 使用 wxappUnpacker 工具进行 MAC 微信小程序反编译
tags: [小程序反编译]
categories: [工具使用]
date: 2024-07-26
description: mac 上对小程序进行反编译。
articleGPT: 本文分享了在 mac 上利用 wxappUnpacker 对小程序进行反编译的方法！
---
😀记录下mac上面小程序反编译的方法

## 配置反编译环境
首先需要配置好你的 node 环境：官网下载或者 brew 安装都行。
然后下载 wxappUnpacker 工具：[github.com/system-cpu/…](https://github.com/system-cpu/wxappUnpacker)

cd 进入下载的文件夹，安装必须的模块
```
npm install
npm install esprima
npm install css-tree
npm install cssbeautify
npm install vm2
npm install uglify-es
npm install js-beautify
```
寻找小程序代码
在 MAC 系统，可以进入到
`/Users/你的用户名/Library/Containers/com.tencent.xinWeChat/Data/.wxapplet/packages/`

​这个文件夹下面，这里面就是存放的你的电脑近期已经打开过的小程序了。你需要提前打开小程序，并且最好把大多数功能都打开一遍，这样不至于漏掉一些资源没有下载下来。

​那具体是哪一个呢？这个时候就需要掏出手机了，在手机上打开你需要反编译的小程序，然后点击右上角的三个点，然后点击小程序名，然后点击更多资料，然后就可以看到小程序的详细信息了，这里就能看到小程序的 APPID 了。

​这样我们就可以进入到 APPID 对应的文件夹，看到一个名为 APP.wxapkg 的文件了，这里就是微信小程序的代码。

## 反编译
直接一行命令就行了，bash 代码解读复制代码：`node wuWxapkg.js __APP__.wxapkg`

这个时候你就能在 APP.wxapkg 这个文件所在的文件夹生成反编译后的小程序的代码了。

## 审计
接下来使用你熟悉的 JS IDE 审计代码就行了，我这里使用微信开发者工具，官网下载即可。
