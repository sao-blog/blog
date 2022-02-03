---
title: 第02章 資料、資料型態與變數
math: true
date: 2022/01/31 01:45:00
categories:
- [程式語言, Golang]
tags:
 - Golang
 - 程式語言
 - 程式學習
---

# 資料型態

| 資料型態 | 語法    |
| -------- | ------- |
| 整數     | int     |
| 浮點數   | float64 |
| 字串     | string  |
| 布林值   | bool    |
| 字元     | rune    |

# 變數的使用流程

## 基本變數宣告

[var]{.red} [變數名稱]{.blue} [資料型態名稱]{.green}

## 指定資料

[變數名稱]{.blue}=[對應型態的資料]{.green}

## 使用變數

使用[變數名稱]{.red}代替資料來做運算

## 宣告變數
```go
var x int = 10

//可以同時建立多個變數並指定初值
var x, y, z int = 10, 20, 30

//如果宣告多個變數時，想要指定不同的型態，可以使用批量宣告
var (
    x int = 10
    y string = "Justin"
    z bool = true
)
```
如果宣告變數時指定了型態，但未指定初值，那麼編輯器會提供預設初值，例如：

```go
var (               // 初始值
    a bool          // false
    b int32         // 0
    c float32       // 0.0
    d string        // ""
    e complex128    // 0 + 0i
)
```

:::danger
在 Go 中，宣告了變數，程式中卻沒有取用的動作，那麼會發生 declared and not used 的編譯錯誤
:::

## 自動推斷型態

在 Go 中宣告變數並指定值時，可以不用提供型態，由編譯器自動推斷型態，例如：

```go
var x = 10 //x 型態會是 int
var x, y, z = 10, 3.14, "only" // x、y、z 的型態分別會是 int、float64 與 string
var (
    x = 10        // int 型態
    y = 3.14      // float64 型態
    z = "Justin"  // string 型態
)
```

## 短變數宣告

```go
x := 10
y := 3.14
z := "Justin"

x, y, z := 10, 3.14, "Justin"
```

## 調換變數值

```go
var x = 10
var y = 20
x, y = y, x
```

# 練習1

```go
package main // 可執行程式必須使用 main 封包
import "fmt" // 載入內建的 fmt 封包，用來做基本輸出輸入
func main(){ // 建立 main 函式，程式的進入點
    // 輸出訊息到終端：fmt.Println(資料,資料,...)
    fmt.Println(3) // 整數 int
    fmt.Println(3.1415) // 浮點數 float64
    fmt.Println("測試中文") // 字串 string
    fmt.Println(true) // 布林值 bool
    fmt.Println('a') // 字符 rune
}
```

# 練習2

```go
package main // 可執行程式必須使用 main 封包
import "fmt" // 載入內建的 fmt 封包，用來做基本輸出輸入
func main(){ // 建立 main 函式，程式的進入點
    var x int // 宣告變數 x
    x = 4 // 指定資料:把資料 4 放進變數裡
    fmt.Println(x) // 使用變數: 用變數的名稱代替資料，做操作
    x = 10
    fmt.Println(x)
    // x = "Hello" 資料型態不正確
    var f float64 = 3.1415 // 宣告變數順便放進資料
    // var 變數名稱 資料型態 = 適當資料
    fmt.Println(f)
    var s string = "only"
    fmt.Println(s)
    var test bool = true
    fmt.Println(test)
    var c rune = 'b'
    fmt.Println(c)
}
```