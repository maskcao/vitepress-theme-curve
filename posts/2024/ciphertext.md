---
title: 基本密码及密文特点
tags: [密文特点]
categories: [基础知识]
date: 2023-09-05
description: 基本密码及密文特点
articleGPT: 本文分享了一些常见的密码的密文特点
---
总结了一些基本密码的密文特征👇
### base16
特征:base16就是16进制转ASCII问题，base16中只有数字0-9以及大写字母ABCDEF

### base32
特征:base32编码是由大写字母（A-Z）和数字234567组成与base64类似
转化密文：MZWGCZZRGIZQ====

### base64
特征：base64是由大写字母（A-Z），小写字母（a-z），数字（0-9）以及+/组成
如果字符不足则会用“=”补齐，特征很明显。
转化密文：ZmxhZzEyMw==

### base36
特征：密文由36个字符（0-9，a-z）组成加密仅支持整数数字，解密仅支持字符串，不支持中文。

### base58
特征：base58是用于Bitcoin中使用的一种独特的编码方式。主要用于产生Bitcoin的钱包地址，bsae58不使用数字0,大写字母O，大写字母I,小写字母l,已及'+'，'/'。

### base62
特征：密文由62字符（0-9，a-z,A-Z)组成

### base91
特征：密文由91个字符（0-9，a-z，A-Z，!#$%& ()*+,./:;<=>?@ []^_` {|}”）

### base92
特征：密文由91个字符（0-9，a-z，A-Z，!#$%& ()*+,./:;<=>?@ []^_` {|}~”） 比base91多了一个"~"

### 凯撒密码
特征：它是一种替换加密的技术，明文中的所有字母都在字母表上向后（或向前）按照一个固定数目进行偏移后被替换成密文。只位移字母。

### 维吉尼亚密码
维吉尼亚密码是一种简单的多表代换密码(由26个类似的Caesar密码的代换表组成)，即由一些偏移量不同的恺撒密码组成，这些代换在一起组成了密钥。

### ROT5
特征：只对数字进行编码，用当前数字往前数的第5个数字替换当前数字。

### ROT13
特征：只对字母进行编码，用当前字母往前数的第13个字母替换当前字母。

### ROT18
特征：这是一个异类，本来没有，它是将ROT5和ROT13组合在一起，为了好称呼，将其命名为ROT18。

### ROT47
特征：对数字、字母、常用符号进行编码，按照它们的ASCII值进行位置替换，用当前字符ASCII值往前数的第47位对应字符替换当前字符。

### 摩斯密码
特征：一般出现形式为“.”和“-”或者为0和1
转化密文：…-. .-… .- --. .---- …—…–

### URL转码
特征：常出现%

### 栅栏密码
特征：题目会给你特别明显的提示如：栅栏，几(明确的数字)只等

### 培根加密
特征：一串字符里全是A和B，并且5个一组。培根加密只能加密字母。
转化密文：flag ==>AABAB ABABB AAAAA AABBA

### jother编码
特征：在javascript语言中，利用少量特定字符构造精简的匿名函数对与字符串的编码方式.代码中大量出现“+”、“！”、“（”、“）”、“[”、“]”、“{”、“}"字符。
转化密文:!![]+!![]+!![]+!![]+!![]+!![]
（用控制台，enter解密）

### unicode编码
特征：Unicode码扩展自ASCII字元集,使用全16位元字元集。Unicode目前普遍采用的是UCS-2,它用两个字节来编码一个字符,字符编码一般用十六进制来表示。
转化密文:\u4e16\u754c\u4f60\u597d
转换明文：hello world

### HTML编码
特征：HTML代表超文本标记语言

### ook编码
特征：ook密码中有大量ook，加上一些符号

### Aes加密
特征： 一般AES的密钥长度是128bit 或 256bit，加密出来的数据是128或256的整倍数。 一般情况下密钥都是16字节

### brianfuck
特征：
转化密文：+++++ +++++ [->++ +++++ +++<] >++.+ +++++ .<+++ [->-- -<]>- -.+++ +++.<

### Rabbit加密
特征：26个大小写英文字母，+，/，=组成。以U2FsdGVkX1开头。可能以=结尾。

### QWE加密
特征： 从电脑键盘上的字母从Q开始数，顺序是Q W E R T Y U I。。。对应的字母顺序依次是A B C D E F G H 也就是说Q=A,W=B,E=C，依次类推。

### 核心价值观编码
特征：富强民主文明和谐自由平等公正法治爱国敬业诚信友善
转化密文：公正公正公正诚信文明公正民主公正法治法治友善平等和谐敬业和谐富强和谐富强和谐文

### RSA 加解密
特征：给一些 RSA 算法的参数，然后加密\解密消息获取 flag。

### 仿射密码 affine cipher
特征：可能会提示你是放射密码 affine，公式： y = k * x + b mod 26 （跟一元一次函数似的）
后面的取模，如果都是英文字母的话是26，不排除有其他形式，比如ASC II 什么的，取模可能会换。

### 进制转换
特征：二进制 b开头，八进制 o开头，十进制 d开头，十六进制 x开头

### xxencode编码
特征：原理与base64大致相同。组成与base64相比多了'+'，少了'/'，而且补全符号为'+'

### uuendode编码
特征：特殊符号很多。

### jjencode
特征：将JS代码转换成只有符号的字符串。（可能有💲，￥）

### aaencode
特征：将JS代码转换成常用的网络表情
