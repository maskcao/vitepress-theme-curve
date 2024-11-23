---
title: BurpSuitePro Mac版破解教程
tags: [BurpSuite]
categories: [工具使用]
date: 2024-11-12
description: BurpSuitePro 破解
articleGPT: 本文分享了BurpSuitePro Mac版的破解教程。
---

## 一.安装burp
**访问官网：** https://portswigger.net/burp/releases
点击下载最新版本
![pic1](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F57bfd112-e18f-47bb-96f5-e9209e5f615a%2Fc3e18b61-0336-4b7b-97ac-b72ce5171e81%2Fimage.png?table=block&id=14354df7-de7d-8047-aa86-e750fc6c3c4c&t=14354df7-de7d-8047-aa86-e750fc6c3c4c&width=708.984375&cache=v2)
进行安装，将图标拖入文件夹中即可
## 二.打开burp（一定要打开一下再退出）
双击burp图标打开应用程序，出现以下界面，点击打开。
![prod-files-secure](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F57bfd112-e18f-47bb-96f5-e9209e5f615a%2Fd8e05495-228d-42dd-a2c5-83d256051db2%2Fimage.png?table=block&id=14354df7-de7d-808a-b3c6-dd5f1f2262f4&t=14354df7-de7d-808a-b3c6-dd5f1f2262f4&width=574&cache=v2)
出现以下界面command+q立即退出burp
![prod-files-secure](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F57bfd112-e18f-47bb-96f5-e9209e5f615a%2Fc343c01a-401b-4789-a0de-28f3d551a76a%2Fimage_(1).png?table=block&id=14354df7-de7d-800b-8df5-f71ca0648c82&t=14354df7-de7d-800b-8df5-f71ca0648c82&width=723.9921875&cache=v2)
## 三.开始破解
**破解工具：** https://www.123pan.com/s/dpIYjv-0e8Bh.html提取码:1234
在应用程序文件夹找到burp，右击显示包的内容
![prod-files-secure](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F57bfd112-e18f-47bb-96f5-e9209e5f615a%2Fd82efa4e-5e5d-44c7-b242-9441014b983b%2Fimage.png?table=block&id=14354df7-de7d-80ad-9009-c0211446cc74&t=14354df7-de7d-80ad-9009-c0211446cc74&width=723.9921875&cache=v2)
找到并编辑vmoptions.txt
```bash
-XX:MaxRAMPercentage=50
-include-options user.vmoptions
-javaagent:BurpLoaderKeygen.jar
-javaagent:BurpSuiteChs.jar
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.Opcodes=ALL-UNNAMED
-noverify
```
进入app路径
`/Applications/Burp Suite Professional.app/Contents/Resources/app`
将破解工具中的BurpLoaderKeygen.jar和BurpSuiteChs.jar放入app文件夹中
![prod-files-secure](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F57bfd112-e18f-47bb-96f5-e9209e5f615a%2F1218ca99-ebcc-4c5b-a646-0dfeb57891ca%2Fimage.png?table=block&id=14354df7-de7d-805e-bf17-f12c9036d1df&t=14354df7-de7d-805e-bf17-f12c9036d1df&width=723.9921875&cache=v2)
## 注:
该列为启用中文包，注释可取消中文
![prod-files-secure](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F57bfd112-e18f-47bb-96f5-e9209e5f615a%2F6ac11e6d-d9a4-48f8-a71c-ebfe9919c0f0%2F3020298-20240105135900639-875303953.png?table=block&id=14354df7-de7d-80ce-a7a5-d6cb82a67be9&t=14354df7-de7d-80ce-a7a5-d6cb82a67be9&width=1358&cache=v2)
## 最后打开burp即可正常使用
