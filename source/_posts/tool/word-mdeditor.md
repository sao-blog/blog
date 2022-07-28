---
title: "在 Word 插入程式碼區塊"
date: 2022-03-29 03:30:00
updated: 2022-03-29 03:30:00
description: "在 Word 插入程式碼區塊"
keywords: 在 Word 插入程式碼區塊,在Word插入程式碼區塊,插入程式碼
swiper_index: 2
categories:
  - [工具]
tags:
  - 
---

# 前言

因為在寫報告時，需要貼上程式碼，但是直接貼覺得很醜，所以找了一個方法順利複製到word

# 開啟MdEditor

- 開啟 [MdEditor](https://www.mdeditor.tw)
- 貼上下方程式碼餘編輯器左側，其中以golang語言舉例(亦可使用c, cpp, java…等)。
~~~ markdown
#### Code

```golang
// your code here
```
~~~

# 貼上目標程式碼並複製到word
- 將 `# your code here` 替換為你的程式碼，你將會在右半邊看到效果
- 反白整個右半邊並複製，{% span red, 注意：須包含標題字(Code) %}，否則會跑版

# 結束

![](https://cdn.jsdelivr.net/gh/sao-coding/sao-blog-images@main/post/1649061140000.png)