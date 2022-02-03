---
title: 第01章 基礎語法
math: true
date: 2022/01/31 01:20:00
categories:
- [程式語言, Golang]
tags:
 - Golang
 - 程式語言
 - 程式學習
---

# 注釋

```go
// 單行注釋
/*
Author by 唯一
我是多行注釋
*/
```

# 輸出Hello, World!

```go
package main // 可執行程式必須使用 main 封包
import "fmt" // 載入內建的 fmt 封包，用來做基本輸出輸入
func main(){ // 建立 main 函式，程式的進入點
    // 輸出字串 Hello, World!
    fmt.Println("Hello, World!")
}
```