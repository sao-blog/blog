---
title: 第1周 程式練習
cover: /img/cover.jpg
date: 2021/12/25 02:20:00
categories:
- [程式語言, Python, 程式練習]
tags:
 - Pyhon
 - 大一課程
 - 程式語言
 - 程式練習
---

:::info
以下為個人學習筆記和習題整理
課程：程式設計 Python - 德明財經科技大學 - 藍國桐
:::

# 第一題 秒數計算 難度 :star2: :star: :star: :star: :star:
- **題目內容**
  甲乙兩人參加 3000公尺賽跑的成績分別是：A 分 B 秒 與 C 分 D 秒，
  請寫一個程式幫忙計算兩者成績相差幾秒。

  *注意：有可能甲的時間比較短，也有可能乙的時間比較短*

|  輸入範例  | 輸出範例 |
| :--------: | :------: |
| `1 10 1 2` |   `8`    |
| `1 50 2 0` |   `10`   |

- 解題思路：
先把分鐘轉成秒
做相減，若答案是負的
可以用abs()這個函數轉成正數
也可以
轉換成字串用迴圈去除負號
或是用replace()來做字串替換
把負號替換掉

## 解題代碼
```python
import datetime
n = input().split()
n = list(map(int,n))
t1 = datetime.timedelta(0,n[0],n[1])
t2 = datetime.timedelta(0,n[1],n[2])
print(abs(t1-t2).seconds)
```

# 第二題 風速計算 難度 :star2: :star: :star: :star: :star:
- **題目內容**
  蒲福風級是由英國海軍少將法蘭西斯蒲福所提出，主要用來紀錄風力，現分為   0~12共13個級數。蒲福風級表通常可做為國際間的天氣預報使用。
請寫一程式輸入蒲福風級經下列公式換算後輸出其對應實際風速(請計算式小數
點第二位四捨五入)。
目前蒲福風級與對應實際風速的公式為：
$V=0.836 * ( B^{3/2} )$ ```( V = 風速 m/s • B = 風級 • ^ 表示次方)```

  *注意：B的3/2次方二B的三次方之後開根號*

|  輸入範例  | 輸出範例 |
| :--------: | :------: |
| `1 10 1 2` |   `8`    |
| `1 50 2 0` |   `10`   |

- 解題思路：
平方使用\*\*
根號使用\*\*0.5

## 解題代碼
```python
print(round(0.836*((int(input())**3)**0.5),2))
```

# 第三題 運費計算 難度 :star2: :star2: :star: :star: :star:
- **題目內容**
新竹貨運公司處理網路購物的運費如下,基本物流處理費199
元,货品重量前1~5公斤,每公斤50元,超過5公斤部分,每公斤30元,货品
重量含小數點时均無條件進位。請寫一個程式用以計算貨品運費·輸入貨品重
量後,計算所需費用。例如:9.5公斤货品所需運費應為599元。

| 範例輸入 | 範例輸出 |
| :------: | :------: |
|   `10`   |  `599`   |
|  `3.1`   |  `399`   |

- 解題思路：
使用math模組裡的ceil()做無條件進位

## 解題代碼
```python
import math
n = float(input())
n = math.ceil(n)
m = 199
for i in range(1,n+1):
    if i<=5:
        m+=50
    else:
        m+=30
print(m)
```

# 第四題 猜數字遊戲 難度 :star2: :star2: :star: :star: :star:
- **題目內容**
A在手心寫個範圍在1-10的數字,握拳不可以被偷看喔
B開始猜,看看B在第幾次能猜到這個數字
請以A為電腦、B為使用者來設計這個程式
**電腦隨機產生一個1-10的數字,然後玩家開始輸入一個數字。如果相同,程式顯
示玩家猜幾次然後結束;如果不同,程式顯示猜錯了然後繼續猜**

- 解題思路：
使用random模組裡的randint做整數隨機亂數
因為不知道要猜幾次所以用while
條件設直到輸入的數字等於一開始設的亂數就跳出迴圈

## 解題代碼
```python
import random
x = random.randint(1,10)
m = 0
n = 0
while x != n:
    n = int(input())
    if n == x:
        m+=1
        print("你花了幾次",m,"猜中")
    else:
        m+=1
        print("猜錯 已猜了",m,"次")
```

# 第五題 計程車車資計算 難度 :star2: :star2: :star: :star: :star:
- **題目內容**
搭計程車時,前1.25公里是起跳格70元,也就是在1.25公里內,不論距離一律
收70元。過了125里後開始跳,每次5元,每隔200公尺一次。請撰寫一
個計算計程車資的程式。輸入公里數,輸出車資。

| 範例輸入 | 範例輸出 |
| :------: | :------: |
|  `7.5`   |  `230`   |
|  `0.8`   |   `70`   |

- 解題思路：
for圈用200間格
是因為200公尺跳表一次
太簡單我掰不出來了

## 解題代碼
```python
n =  float(input())
km =  70 m =  1250 
for _ in  range(m,int(n*1000),200):
	km+=5
	print(70  if n <  1.25  else km)
```

# 第六題 大樂透開獎號碼 難度 :star2: :star2: :star2: :star: :star:
- **題目內容**
大樂透開獎時是1-49內數取出6個數字當開獎號碼,同時再取一個特 別號。換句話說,大樂透的開獎號碼一共包含7個數字,這些數字當然 不能重複。請撰寫一個程式,可以隨機產生一組大樂透的開獎號碼,中 獎號碼會由小到大顯示;特別號列在最後一個位置

| 範例輸入 |                範例輸出                |
| :------: | :------------------------------------: |
|   `無`   | `中獎號碼 6 13 17 29 33 40、特別號 21` |
|   `無`   | `中獎號碼 3 9 15 31 38 47、特別號 11`  |

- 解題思路：
使用random模組裡的sample()做隨機產生7個亂數到串列裡  
把串列最後一個數存起來後移除  
把串列做排序

## 解題代碼
```python
import random
list  =  [i for i in  range(1,50)]
x = random.sample(list,7)
z = x[6]
x.remove(x[6])
x.sort() 
print("中獎號碼",x[0],x[1],x[2],x[3],x[4],x[5],end =  '')  print("、特別號",z)
```

# 第七題 抓出遲到鬼 難度 :star2: :star2: :star: :star: :star:
- **題目內容**
班上有座號1-10的10位同學,約好上九點在學校集合後一起出去玩。請寫個程 式,依照同學到達的順序輸入座號,然後依序輸出缺席的同學座號

|     範例輸入     |   範例輸出   |
| :--------------: | :----------: |
| `8 2 3 5 10 4 1` |   `6 7 9`    |
|   `2 8 1 3 7`    | `4 5 6 9 10` |

- 解題思路：
for迴圈1開始要記得11結束  
若迴圈的數字不在串列裡則印出來

## 解題代碼
```python
n =  [eval(i)  for i in  input().split()]
#n = list(map(int,input().split()))
for _ in  range(1,11):
	if _ not  in n:  print(_,end =  ' ')
```

# 第七題 遊覽車座位 難度 :star2: :star2: :star2: :star: :star:
- **題目內容**
程式設計課即將出遊,學生有90人(編號1 90),有5台中型遊覽車 可以搭乘(假設一可搭乘20人)。請將每位同學隨機分配到一台遊覽車 (車號1,··5),列出每輛車所搭乘的學生編號,並輸出每台車的人數。 輸入無 輸出 車號1:共人,xxx 車號2:共X人,xxx 車號3:共X人,xxx 車號4:共人,xxx 車號5:共人,xxx 解題思路: 產生一個存了1~90的串列 使用random模組裡的shuffle(把陣列打亂 剩下的自己想我懶得打字 不然就來問我ク

| 範例輸入 |                                               範例輸出                                                |
| :------: | :---------------------------------------------------------------------------------------------------: |
|   `無`   | `車號1:共x人,xxx`<br>`車號2:共x人,xxx`<br>`車號3:共x人,xxx`<br>`車號4:共x人,xxx`<br>`車號5:共x人,xxx` |

- 解題思路：
產生一個存了1~90的串列  
使用random模組裡的shuffle()把陣列打亂  
剩下的自己想我懶得打字  
不然就來問我ㄅ

## 解題代碼

;;;id1 普通版
```python
import random
bus=[]
people = []
n = 0
m = 20
list = [i for i in range(1,91)]
random.shuffle(list)
for _ in range(5):
    people = [ i for i in list[n:m]]
    n = m
    m+=20
    bus.append(people)
for i in range(5):
    print("車號"+str(i+1)+" : 共"+str(len(bus[i]))+"人",end = "  ")
    for j in range(len(bus[i])):
        print(bus[i][j],end = " ")
    print
```
- - -

;;;

;;;id1 公車隨機人數版
```python 公車隨機人數版
import random
bus=[]
people = []

list = [i for i in range(1,91)]
random.shuffle(list)

import random

def bus_random():
    y = 0
    bus = []
    for i in range(4):
        x = random.randint(10,20)
        bus.append(x)
        y+=bus[i]
    if y >= 70:
        bus.append(90-y)
        return bus
    else:
        return bus_random()
bus_num = bus_random() 

n = 0
m = 0

for _ in range(5):
    m+=bus_num[_]
    people = [ i for i in list[n:m]]
    n = m
    bus.append(people)
    
for i in range(5):
    print("車號"+str(i+1)+" : 共"+str(len(bus[i]))+"人",end = "  ")
    for j in range(len(bus[i])):
        print(bus[i][j],end = " ")
    print()
```
- - -

;;;