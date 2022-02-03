---
title: Python常用函式
quiz: true
date: 2021/12/25 02:20:00
categories:
- [程式語言, Python]
tags:
 - Pyhon
 - 大一課程
 - 程式語言
---
;;;id1 test
test
;;;

;;;id1 test1
test
;;;
:::info
以下為個人學習筆記和習題整理
課程：程式設計 Python - 德明財經科技大學 - 藍國桐
:::

# 常用輸入函式
- **`字串.split()`**
	`字串.split("要分割的字", 分割的次數)`
	括號裡面不寫東西，預設是分割空字符
    ```python
	txt = "Google#Runoob#Taobao#Facebook"
	# 第二个参数为 1，返回两个参数列表
	x = txt.split("#", 1)
	print(x)
	#實例輸出如下
	#['Google',  'Runoob#Taobao#Facebook']
    ```

1. `print("apple banana".split("a"))`輸的是 []{.gap} 。 {.quiz}
    - `['apple b', '', 'a']`
    - `['apple', 'banana']`
    - `['a', '', 'le banana']`
    - `['', 'pple b', 'n', 'n', '']` {.correct}
{.options}
	> - :x: `print("apple banana".split("an"))`
    > - :x: `print("apple banana".split(" "))`
    > - :x: `print("apple banana".split("p"))`
    > - :heavy_check_mark: `print("apple banana".split("a"))`
    > {.options}

# 型態轉換函式

- **`int()`**
  括號內放入想要轉換成整數的變數`int(x)`
  
- **`str()`**
  括號內放入想要轉換成字串的變數`str(x)`
  
- **`float()`**
  括號內放入想要轉換成浮點數的變數`float`

## 注意事項
`input()`輸入的值是[**字串型態**]{.rainbow}
在[oj | 簡易加法(I)](https://sao.dsmynas.com:1100/problem/0002)中做兩數字相加時，要將`input().split()`分割後的數字轉成**整數型態**，因為`input()`輸入數字串，要每個數字相加必須把每個值做轉換，而不是把相加完的字串轉成整數型態

1. 請問以下程式碼，輸入`1 2`，答案為[12]{.gap}。 {.quiz .fill}
    ```python
    n = input().split()
    print(int(n[0]+n[1]))
    ```
    >這裡是用字串型態做相加
    >所以"1"+"2"="12"
    >然後再把"12"轉換成整數型態變成12 
    >[**3是錯誤的答案喔!!!**]{.mistake}
    
2. 請問以下程式碼，輸入`1 2`，答案為[3]{.gap}。 {.quiz .fill}
    ```python
    n = input().split()
    print(int(n[0])+int(n[1]))
    ```
    >這裡是把每個字串分別轉換成整數型態
    >用整數型態做相加
    >所以1+2=3
    >[**12是錯誤的答案喔!!!**]{.mistake}

+++warning 看得懂就用吧
- **map()**
	`map(function, iterable,  ...)`
	-   function - 函式
	-   iterable - 一個或多個陣列

  使用一個變數要將陣列轉換型態請使用`list()`
  `n = list(map(函式,陣列))`
+++