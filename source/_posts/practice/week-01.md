---
title: "練習題"
date: 2022-04-21 12:30:00
updated: 2022-04-21 12:30:00
description: "練習題"
keywords: 練習題
swiper_index:
categories:
- [練習題]
tags:
  - Python
  - C#
---

{% folding yellow, 第一題 %}

<body contenteditable="false" class="cke_editable cke_editable_themed cke_contents_ltr cke_show_borders"
    spellcheck="false" style="height: auto; min-height: auto;">
    <p><span style="font-family:Courier New,Courier,monospace">公司每年定期為員工實施健康檢查測量血壓，血壓的值包含收縮壓(較高者)與舒張壓(較低者)。<br>在測量完所有員工的兩項血壓數值後，公司會統計並輸出所有員工之收縮壓與舒張壓的平均值與中位數以資參考。<br><strong>一串數字的中位數</strong>，<strong>是這些數字依序居中的值</strong>，例如：3,7,1,9,5的<strong>中位數是5</strong>；而5,8,2,6的<strong>中位數是5和6的平均</strong>(無條件捨去小數位)。<br><strong>請協助完成函式</strong><em>split
                − range()</em><strong>以完成計算員工兩項血壓的中位數值</strong>。(注意：本程式並未使用排序來找出中位數。)</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸入格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace"><em>n</em>：員工數</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>h<sub>a1</sub></em>, …,<em>
                    h<sub>an</sub></em>：員工的收縮壓</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>h<sub>b1</sub></em>, …,
                <em>h<sub>bn</sub></em>：員工的舒張壓</span></li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸出格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace"><em>ha_avg</em>&nbsp;: 員工收縮壓平均值</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>hb_avg</em>&nbsp;: 員工舒張壓平均值</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>ha_md</em>&nbsp;: 員工收縮壓中位數</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>hb_md</em>&nbsp;: 員工舒張壓中位數</span></li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>需要完成及繳交的函式（擇一程式語言完成作答即可）：</strong></span></p>
    <table border="1" cellpadding="1" cellspacing="1" style="width:1100px">
        <tbody>
            <tr>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png" style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png"
                            style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png" style="height:29px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png" style="height:30px; width:30px"></span></td>
            </tr>
            <tr>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace"><strong>static void Split_Range(int
                                split_pos, int mid, ref int left, ref int right)</strong> 函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">split_pos: 分割點位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">mid: 中位數位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">left: 排序左端</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">right: 排序右端</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">此函式依照呼叫split函數的結果(split_pos)，來逐漸縮小尋找的範圍。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">static void Split_Range(int split_pos,
                            int mid, ref int left, ref int right) {<br>&nbsp; &nbsp; //請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace"><strong>void split_range(int split_pos,
                                int mid, int *left, int *right)</strong> 函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">split_pos: 分割點位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">int mid: 中位數位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">int *lef: 排序左端</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">int *right: 排序右端</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">此函式依照呼叫split函數的結果(split_pos)，來逐漸縮小尋找的範圍。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">void split_range(int split_pos, int mid,
                            int *left, int *right) {<br>&nbsp; &nbsp; // 請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace"><strong>private static int[]
                                splitRange(int splitPos, int mid, int left, int right)</strong> 函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">splitPos: 分割點位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">mid: 中位數位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">left: 排序左端</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">right: 排序右端</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">此函式依照呼叫split函數的結果(splitPos)，來逐漸縮小尋找的範圍。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">private static int[] splitRange(int
                            splitPos, int mid, int left, int right) {<br>&nbsp; &nbsp; //請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace"><strong>def split_range(pivot_position,
                                mid, left, right):</strong> 函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">pivot_position: 分割點位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">mid: 中位數位置</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">left: 排序左端</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">right: 排序右端</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">此函式依照呼叫split函數的結果(pivot_position)，來逐漸縮小尋找的範圍。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">def split_range(pivot_position, mid,
                            left, right):<br>&nbsp; &nbsp; #請完成並繳交本函式</span></p>
                </td>
            </tr>
        </tbody>
    </table>
    <p><br></p>
    {% folding yellow, 測資 %}
    <p><span style="font-family:Courier New,Courier,monospace"><strong>範例測資：<br>測資1<br>輸入</strong><br>5<br>139 93 121
            142 116<br>68 89 58 67 83<br><strong>輸出</strong><br>122<br>73<br>121<br>68</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資2<br>輸入</strong><br>4<br>125 132 130 108<br>96
            67 82 96<br><strong>輸出</strong><br>123<br>85<br>127<br>89</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資3<br>輸入</strong><br>3<br>149 147 119<br>77 68
            70<br><strong>輸出</strong><br>138<br>71<br>147<br>70</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資4<br>輸入</strong><br>10<br>108 140 141 132 140
            100 116 116 94 90<br>89 55 84 77 79 91 74 72 85 99<br><strong>輸出</strong><br>117<br>80<br>116<br>81</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資5<br>輸入</strong><br>1<br>134<br>55<br><strong>輸出</strong><br>134<br>55<br>134<br>55</span>
    </p>
    <p><br></p>
    {% endfolding %}
</body>

```c#
using System;

namespace Q1
{
    class Program
    {
        static int Average(int[] x)
        {
            int sum = 0;
            for (int i = 0; i < x.Length; ++i)
            {
                sum += x[i];
            }
            return sum / x.Length;
        }

        static int Split(int[] x, int left, int right)
        {
            int focus_data = x[left];
            int focus_pos = left, tmp;

            for (int i = left + 1; i <= right; ++i)
            {
                if (x[i] < focus_data)
                {
                    tmp = x[++focus_pos];
                    x[focus_pos] = x[i];
                    x[i] = tmp;
                }
            }

            tmp = x[left];
            x[left] = x[focus_pos];
            x[focus_pos] = tmp;

            return focus_pos;
        }

        static void Split_Range(int split_pos, int mid, ref int left, ref int right)
        {
            // 你的程式碼
        }

        static int half(int[] data)
        {
            int value = data[data.Length / 2];
            for (int i = data.Length / 2; i < data.Length; ++i)
            {
                if (data[i] < value)
                    value = data[i];
            }
            return value;
        }

        static int Midian(int[] x)
        {
            int left = 0, right = x.Length - 1, mid = right / 2, split_pos;
            while (true)
            {
                split_pos = Split(x, left, right);
                if (split_pos == mid) break;
                else Split_Range(split_pos, mid, ref left, ref right);
            }

            if (x.Length % 2 == 1) return x[mid];
            else return (x[mid] + half(x)) / 2;
        }

        static void Main(string[] args)
        {
            //Console.Write("input n: ");
            //int n = 
            Convert.ToInt32(Console.ReadLine());
            int[] ha, hb;
            int ha_avg, hb_avg, ha_md, hb_md;

            ha = Array.ConvertAll(Console.ReadLine().Trim().Split(' '), item => Convert.ToInt32(item));
            hb = Array.ConvertAll(Console.ReadLine().Trim().Split(' '), item => Convert.ToInt32(item));

            ha_avg = Average(ha);
            hb_avg = Average(hb);
            ha_md = Midian(ha);
            hb_md = Midian(hb);
            Console.WriteLine(ha_avg + "\n" + hb_avg + "\n" + ha_md + "\n" + hb_md);
        }
    }
}
```

```python
def average(data, n):
    avg = 0
    for x in data:
        avg += x
    return avg//n

def split(data, left, right):
    pivot = data[left]
    pivot_position = left
    for i in range(left+1,right+1):
        if data[i] < pivot:
            pivot_position += 1
            data[i], data[pivot_position] = data[pivot_position], data[i]
    data[left], data[pivot_position] = data[pivot_position], data[left]
    return pivot_position

def split_range(pivot_position, mid, left, right):
	
# 你的程式碼
	
def half(data, n):
    value = data[n//2]
    for i in range(n//2,n):
        if data[i] < value:
            value = data[i]
    return value

def median(data, n):
    left = 0
    right = n-1
    mid = (left+right)//2

    while(True):
        pivot_position = split(data, left, right)
        if pivot_position == mid:
            break
        else:
            left,right = split_range(pivot_position, mid, left, right)

    if n%2 == 1:
        return data[mid]
    else:
        return (data[mid] + half(data, n))//2

num = int(input())
systolic = list(map(int,input().split()))
diastolic = list(map(int,input().split()))

sy_average = average(systolic, num)
dia_average = average(diastolic, num)
sy_median = median(systolic, num)
dia_median = median(diastolic, num)
print(sy_average, dia_average, sy_median, dia_median,sep='\n')
```

{% endfolding %}

{% folding yellow, 第二題 %}


<body contenteditable="false" class="cke_editable cke_editable_themed cke_contents_ltr cke_show_borders"
    spellcheck="false" style="height: auto; min-height: auto;">
    <p><span
            style="font-family:Courier New,Courier,monospace">台灣兒童保護基金會募集發票後，請志工協助對獎並統計中獎金額製作出公開報表，供捐贈者自由查閱。<br>統一發票獎別及獎金如下：</span>
    </p>
    <p><span style="font-family:Courier New,Courier,monospace"><img alt=""
                data-cke-saved-src="/_other/CK/upload/images/發票兌獎.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/發票兌獎.png"
                style="height:222px; width:659px"></span></p>
    <p><span
            style="font-family:Courier New,Courier,monospace">一張發票若同時符合2個獎項，則獎金以最高獎金為主，例如發票號碼同時符合五獎及六獎，則以五獎判定。<br>對獎主程式將呼叫<em>WinPrize</em>()函式以計算並回傳一張發票的中獎金額，據以統計全部發票的中獎總金額。</span>
    </p>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸入格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace"><em>W</em>：頭獎號碼，其中<em>W</em>為8碼字串</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>N</em>：發票總數，其中<em>N</em>為整數，
                1≤<em>N</em>≤20</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>P<sub>1</sub></em>: 第一張發票</span></li>
        <li><span style="font-family:Courier New,Courier,monospace">...</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>P<sub>N</sub></em>: 第<em>N&nbsp;</em>張發票</span>
        </li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸出格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace"><em>M</em>: 中獎總金額</span></li>
    </ul>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>需要完成及繳交的函式（擇一程式語言完成作答即可）：</strong></span></p>
    <table border="1" cellpadding="1" cellspacing="1" style="width:1000px">
        <tbody>
            <tr>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png" style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png"
                            style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png" style="height:29px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png" style="height:30px; width:30px"></span></td>
            </tr>
            <tr>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">static int WinPrize(string W, string
                            P)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">W頭獎發票號碼，其長度始終為8，內容為0到9</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">P發票號碼，其長度始終為8，內容為0到9</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算並回傳發票中獎金額。</span></li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">static int WinPrize(string W, string P)
                            {<br>&nbsp; &nbsp; // 請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">int WinPrize (char W[], char
                            P[])函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">W頭獎發票號碼，其長度始終為8，內容為0到9</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">P發票號碼，其長度始終為8，內容為0到9</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算並回傳發票中獎金額。</span></li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">int WinPrize (char W[], char P[])
                            {<br>&nbsp; &nbsp; // 請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">private static int WinPrize(String W,
                            String P)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">W頭獎發票號碼，其長度始終為88，內容為00到99</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">P發票號碼，其長度始終為88，內容為00到99</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算並回傳發票中獎金額。</span></li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">private static int WinPrize(String W,
                            String P) {<br>&nbsp; &nbsp; // 請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">def WinPrize(W, P)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">W頭獎發票號碼，其長度始終為8，內容為0到9</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">P發票號碼，其長度始終為8，內容為0到9</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算並回傳發票中獎金額。</span></li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">def WinPrize(W, P):<br>&nbsp; &nbsp; #
                            請完成並繳交本函式</span></p>
                </td>
            </tr>
        </tbody>
    </table>
    <p><br></p>
    {% folding yellow, 測資 %}

    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>範例測資：<br>測資1<br>輸入</strong><br>13859285<br>3<br>38592769<br>42893285<br>32398733<br><strong>輸出</strong><br>200</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資2<br>輸入</strong><br>39384729<br>4<br>93859284<br>38494729<br>39472859<br>39485739<br><strong>輸出</strong><br>1000</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資3<br>輸入</strong><br>22385928<br>3<br>22385927<br>38420848<br>48347982<br><strong>輸出</strong><br>0</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資4<br>輸入</strong><br>00384929<br>3<br>82948372<br>00374872<br>82984929<br><strong>輸出</strong><br>4000</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資5<br>輸入</strong><br>98384928<br>2<br>98384928<br>93849284<br><strong>輸出</strong><br>200000</span>
    </p>
    {% endfolding %}
</body>


```c#
using System;

namespace csharp
{
    class Q2
    {
        static int WinPrize(string W, string P)
        {
            // 你的程式碼
        }

        static void Main()
        {
            string W = Console.ReadLine(); // 頭獎號碼
            string P; // 發票號碼
            int N = Convert.ToInt32(Console.ReadLine()); // 發票總數
            int M = 0; // 中獎總金額

            for (int i = 0; i < N; i += 1)
            {
                P = Console.ReadLine();
                M += WinPrize(W, P);
            }
            Console.WriteLine(M);
        }

    }
}
```

```python
def WinPrize(W, P):
	
# 你的程式碼

if __name__ == '__main__':
    W = input()
    N = int(input())
    M = 0
    
    for i in range(N):
        P = input()
        M += WinPrize(W, P)
    print(M)
```
{% endfolding %}

{% folding yellow, 第三題 %}

<body contenteditable="false" class="cke_editable cke_editable_themed cke_contents_ltr cke_show_borders"
    spellcheck="false" style="height: auto; min-height: auto;">
    <p><span
            style="font-family:Courier New,Courier,monospace">一小時音樂廣播節目中共有4個單元，每單元結束時會進2分鐘的廣告，因此每個單元最多僅能播放13分鐘的歌曲。</span>
    </p>
    <p><span style="font-family:Courier New,Courier,monospace">單元中的音樂由AI程式從DJ準備的音樂歌單中，依下列規則選擇播放：</span></p>
    <ol>
        <li><span style="font-family:Courier New,Courier,monospace">每首歌僅能播放一次，且須完整播完，不能中間卡歌。</span></li>
        <li><span
                style="font-family:Courier New,Courier,monospace">歌曲播放順序以音樂歌單中長度最長且能完整播完的優先。若兩首歌曲長度相同，編號較大者優先選擇播放。</span>
        </li>
        <li><span style="font-family:Courier New,Courier,monospace">若有單元剩餘時間（進廣告前）無法完整播放下一首歌，則由節目DJ串場直至進廣告為止。</span>
        </li>
    </ol>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>範例</strong></span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　DJ音樂歌單共有M=15首音樂，每首音樂的資訊記錄為&lt;音樂編號，音樂長度&gt;，15首音樂分別記錄為<br>　　&lt;1,
            210&gt;,&lt;2, 246&gt;,&lt;3, 252&gt;,&lt;4, 192&gt;,&nbsp;&lt;5, 186&gt;,<br>　　&lt;6, 282&gt;,&lt;7,
            168&gt;,&lt;8, 162&gt;,&lt;9, 90&gt;,&lt;10, 234&gt;,<br>　　&lt;11, 252&gt;,&lt;12, 210&gt;,&lt;13,
            258&gt;,&lt;14, 210&gt;,&lt;15, 204&gt;。</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　我們根據音樂長度將音樂歌單由大到小排序，若音樂長度相同，則以音樂編號大者優先排序，其順序為<br>　　&lt;6,
            282&gt;,&nbsp;&lt;13, 258&gt;,&lt;11, 252&gt;,&nbsp;&lt;3, 252&gt;,&nbsp;&lt;2, 246&gt;,<br>　　&lt;10,
            234&gt;,&nbsp;&lt;14, 210&gt;,&nbsp;&lt;12, 210&gt;,&nbsp;&lt;1, 210&gt;,&nbsp;&lt;15, 204&gt;,<br>　　&lt;4,
            192&gt;,&lt;5, 186&gt;,&nbsp;&lt;7, 168&gt;,&nbsp;&lt;8, 162&gt;,&nbsp;&lt;9, 90&gt;。</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　因此四個單元的歌單為：</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　第一個單元13分鐘，歌曲 6, 13, 10，剩餘6秒；</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　第二個單元13分鐘，歌曲 11, 3, 2，剩餘30秒；</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　第三個單元13分鐘，歌曲 14, 12, 1, 9，剩餘60秒；</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　第四個單元13分鐘，歌曲 15, 4, 5, 7，剩餘30秒。</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">　　請協助完成程式中MusicOrder函式，回傳該單元的音樂播放清單。</span></p>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸入格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace">M：音樂歌單的歌曲數，音樂編號就是1到M。</span></li>
        <li><span style="font-family:Courier New,Courier,monospace">X<sub>1</sub>&nbsp;...
                X<sub>M</sub>：每一首音樂的時間長度(單位：秒)，0 &lt; X<sub>i</sub>&nbsp;≤ 600，其中1 ≤ i ≤ M，兩數之間以一空格分隔。</span></li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸出格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace">Y<sub>1</sub>&nbsp;…
                Y<sub>k</sub>&nbsp;T<sub>1</sub>：第一單元音樂播放清單及剩餘時間，兩數之間以一空格分隔。</span></li>
        <li><span style="font-family:Courier New,Courier,monospace">Y<sub>1</sub>&nbsp;…
                Y<sub>k</sub>&nbsp;T<sub>2</sub>：第二單元音樂播放清單及剩餘時間，兩數之間以一空格分隔。</span></li>
        <li><span style="font-family:Courier New,Courier,monospace">Y<sub>1</sub>&nbsp;…
                Y<sub>k</sub>&nbsp;T<sub>3</sub>：第三單元音樂播放清單及剩餘時間，兩數之間以一空格分隔。</span></li>
        <li><span style="font-family:Courier New,Courier,monospace">Y<sub>1</sub>&nbsp;…
                Y<sub>k</sub>&nbsp;T<sub>4</sub>：第四單元音樂播放清單及剩餘時間，兩數之間以一空格分隔。</span></li>
    </ul>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>需要完成及繳交的函式（擇一程式語言完成作答即可）：</strong></span></p>
    <table border="1" cellpadding="1" cellspacing="1" style="width:800px">
        <tbody>
            <tr>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png"
                            style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png" style="height:29px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png" style="height:30px; width:30px"></span></td>
            </tr>
            <tr>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">int *MusicOrder(int chapter_len, int M,
                            int *X_sorted, int *X_sorted_id, int *music_list)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">整數chapter_len代表每單元所剩時間。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">整數M代表音樂歌單歌曲數。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">陣列X_sorted代表排序後的音樂歌單時長。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">陣列X_sorted_id代表排序後的音樂清單編號。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">陣列music_list代表該單元的音樂播放清單。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算該單元的音樂播放清單與剩下未播放音樂的時間長度。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">int *MusicOrder(int chapter_len, int M,
                            int *X_sorted, int *X_sorted_id, int *music_list) {<br>&nbsp; &nbsp; // 請完成並繳交本函式</span></p>
                    <p><span style="font-family:Courier New,Courier,monospace">&nbsp; &nbsp; return
                            music_list;<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">public static int[] MusicOrder(int
                            chapter_len, int M, int[] X_sorted, int[] X_sorted_id, int[] music_list)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">整數chapter_len代表每單元所剩時間。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">整數M代表音樂歌單歌曲數。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">陣列X_sorted代表排序後的音樂歌單時長。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">陣列X_sorted_id代表排序後的音樂清單編號。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">陣列music_list代表該單元的音樂播放清單。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算該單元的音樂播放清單與剩下未播放音樂的時間長度。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">public static int[] MusicOrder(int
                            chapter_len, int M, int[] X_sorted, int[] X_sorted_id, int[] music_list)<br>{<br>&nbsp;
                            &nbsp; // 請完成並繳交本函式</span></p>
                    <p><span style="font-family:Courier New,Courier,monospace">&nbsp; &nbsp; return
                            music_list;<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">def MusicOrder(chapter_len, X_sorted,
                            X_sorted_id)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">整數chapter_len代表每單元所剩時間。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">串列X_sorted代表排序後的音樂歌單時長。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">串列X_sorted_id代表排序後的音樂清單編號。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函數計算該單元的音樂播放清單與剩下未播放音樂的時間長度。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">def MusicOrder(chapter_len, X_sorted,
                            X_sorted_id): # 回傳該單元的音樂播放清單<br>&nbsp; &nbsp; # 請完成並繳交本函式</span></p>
                </td>
            </tr>
        </tbody>
    </table>
    <p><br></p>
    {% folding yellow, 測資 %}
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>範例測資：<br>測資1<br>輸入</strong><br>1<br>800<br><strong>輸出</strong><br>780<br>780<br>780<br>780</span>
    </p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資2<br>輸入</strong><br>2<br>300
            300<br><strong>輸出</strong><br>2 1 180<br>780<br>780<br>780</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資3<br>輸入</strong><br>5<br>60 100 200 300
            400<br><strong>輸出</strong><br>5 4 1 20<br>3 2 480<br>780<br>780</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資4<br>輸入</strong><br>5<br>638 527 416 354
            223<br><strong>輸出</strong><br>1 142<br>2 5 30<br>3 4 10<br>780</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資5<br>輸入</strong><br>10<br>272 623 226 398 452
            328 705 646 172 763<br><strong>輸出</strong><br>10 17<br>7 75<br>8 134<br>2 157</span></p>
    {% endfolding %}
</body>

```python
def MusicOrder(chapter_len, X_sorted, X_sorted_id): # 回傳該單元的音樂播放清單

# 你的程式碼
	
if __name__ == '__main__':
    M = int(input()) # 音樂歌單歌曲數M
    X = [None] * M # 音樂歌單時長
    X_sorted = [None] * M # 排序後的音樂歌單時長
    X_sorted_id = [None] * M #排序後的音樂清單編號

    X_all = input() # 輸入音樂歌單時長
    X = X_all.split(' ')
    X = list(map(int, X))
    
    # 插入排序（由大至小）
    X_sorted[0] = X[0]
    X_sorted_id[0] = 0
    for i in range(1, M):
        key = X[i]
        j = i - 1
        while(j>=0 and X_sorted[j]<=key):
            X_sorted[j+1] = X_sorted[j]
            X_sorted_id[j+1] = X_sorted_id[j]
            j -= 1
        X_sorted[j+1] = key
        X_sorted_id[j+1] = i
    
    # 安排四個單元的歌單
    chapter_len = 13 * 60 # 每個單元時長
    rounds = 4 # 單元數量
    
    for r in range(rounds):
        music_list = MusicOrder(chapter_len, X_sorted, X_sorted_id)
    
        music_list_len = len(music_list)
        remain = chapter_len
        for m in music_list:
            remain -= X[m-1]
            print(m, end=" ") # 印出該單元的音樂播放清單
        print(remain) # 印出該單元剩餘時間
```

{% endfolding %}

{% folding yellow, 第四題 %}
<body contenteditable="false" class="cke_editable cke_editable_themed cke_contents_ltr cke_show_borders"
    spellcheck="false" style="height: auto; min-height: auto;">
    <p><span style="font-family:Courier New,Courier,monospace">剛成為大一新鮮人的王小明要開始選課了，他想把課程全部排在三天內，其他時間去打工與參加社團。因此他先列出三天內可以選的課程清單，決定使用以下規則輕鬆選課：
            &nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;
            &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;</span></p>
    <ol>
        <li><span style="font-family:Courier New,Courier,monospace"><strong>從第一天開始挑選，挑選完後，再挑選下一天的課程。</strong></span>
        </li>
        <li><span style="font-family:Courier New,Courier,monospace"><strong>依照當天課程之下課節次排序，先挑選最早下課者（如有相同下課時間的課程，則選擇英文字母排序較前者，
                    例如：A為2-3節，B為1-3節，會選擇A）。</strong></span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><strong>每日盡可能把課程排滿。</strong></span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><strong>課程時間不可重疊。</strong></span></li>
        <li><span
                style="font-family:Courier New,Courier,monospace"><strong>同一天不會有重複的課程名稱，且相同課程在三天內只能挑選一次。</strong></span>
        </li>
    </ol>
    <p><span style="font-family:Courier New,Courier,monospace">例如王小明挑選的三天課表為下表：</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><img alt=""
                data-cke-saved-src="/_other/CK/upload/images/未命名(1).jpg" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/未命名(1).jpg"
                style="height:226px; width:800px"></span></p>
    <p><span style="font-family:Courier New,Courier,monospace">第一天選的課程是<em>A</em>、<em>C</em>
            (<em>B</em>的時間與<em>A</em>重疊、<em>D</em>的時間與<em>C</em>
            重疊)<br>第二天選的課程是<em>B</em>、<em>D</em>(<em>A</em>選過了，<em>E</em>的時間與<em>D&nbsp;</em>重疊)<br>第三天選的課程是<em>F</em>
            &nbsp; (<em>C</em>選過了，<em>E</em>的時間與<em>F</em> 重疊)</span></p>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸入格式：</strong><br>未排序的課程清單</span></p>
    <ul>
        <li><span
                style="font-family:Courier New,Courier,monospace"><em>N</em>：共有幾筆資料輸入，其中<em>N&nbsp;</em>為整數，3≤<em>N</em>
                ≤36</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>d</em><sub>1</sub>&nbsp;
                <em>c</em><sub>1</sub>&nbsp; <em>s</em><sub>1</sub> &nbsp;<em>e</em><sub>1</sub>：天(1-3) 課程名稱(A-L)
                課程開始節次(1-7) 課程結束節次(2-8)</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>d</em><sub>2</sub> &nbsp;<em>c</em><sub>2</sub>
                &nbsp;<em>s</em><sub>2</sub> &nbsp;<em>e</em><sub>2</sub>：天(1-3) 課程名稱(A-L) 課程開始節次(1-7)
                課程結束節次(2-8)</span></li>
        <li><span style="font-family:Courier New,Courier,monospace">...</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>d</em><sub>n</sub> &nbsp;<em>c</em><sub>n</sub>
                <em>&nbsp;s</em><sub>n</sub> &nbsp;<em>e</em><sub>n</sub>：天(1-3) 課程名稱(A-L) 課程開始節次(1-7)
                課程結束節次(2-8)</span></li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸出格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace"><em>d</em><sub>1</sub>&nbsp;
                <em>c</em><sub>1</sub>&nbsp; <em>s</em><sub>1</sub> &nbsp;<em>e</em><sub>1</sub></span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>d</em><sub>2</sub> &nbsp;<em>c</em><sub>2</sub>
                &nbsp;<em>s</em><sub>2</sub> &nbsp;<em>e</em><sub>2</sub></span></li>
        <li><span style="font-family:Courier New,Courier,monospace">...</span></li>
        <li><span style="font-family:Courier New,Courier,monospace"><em>d</em><sub>n</sub> &nbsp;<em>c</em><sub>n</sub>
                <em>&nbsp;s</em><sub>n</sub> &nbsp;<em>e</em><sub>n</sub></span></li>
    </ul>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>需要完成及繳交的函式（擇一程式語言完成作答即可）：</strong></span></p>
    <table border="1" cellpadding="1" cellspacing="1" style="width:1000px">
        <tbody>
            <tr>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png" style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png"
                            style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png" style="height:29px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Python_3.png" style="height:30px; width:30px"></span></td>
            </tr>
            <tr>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">static void SelectCourse(Course[]
                            results, bool[] selected, Course[] candidates, int cs)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">results選課結果。</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">selected紀錄課程是否被選過，未選過則紀錄false，已選過則紀錄true。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">candidates每日可選課程。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">cs每日可選課程（candidates）數量</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算並回傳每日的選課清單。</span></li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">static void SelectCourse(Course[]
                            results, bool[] selected, Course[] candidates, int cs) {<br>&nbsp; &nbsp; //
                            請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">void SelectCourse(Course results[], int
                            *rs, bool selected[], Course candidates[], int cs)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">results選課結果。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">rs選課結果（results）數量。</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">selected紀錄課程是否被選過，未選過則紀錄false，已選過則紀錄true。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">candidates每日可選課程。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">cs每日可選課程（candidates）數量</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">此函式計算並更新選課結果(results)，同時更新rs及selected。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">void SelectCourse(Course results[], int
                            *rs, bool selected[], Course candidates[], int cs) {<br>&nbsp; &nbsp; //
                            請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">static void SelectCourse(Course
                            results[], boolean selected[], Course candidates[], int cs)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">results選課結果。</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">selected紀錄課程是否被選過，未選過則紀錄false，已選過則紀錄true。</span>
                        </li>
                        <li><span style="font-family:Courier New,Courier,monospace">candidates每日可選課程。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">cs每日可選課程（candidates）數量</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">此函式計算並更新選課結果(results)，同時更新rs及selected。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">static void SelectCourse(Course
                            results[], boolean selected[], Course candidates[], int cs) {<br>&nbsp; &nbsp; //
                            請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">def selectCourse(candidates,
                            selected):函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">candidates為每天可選之課程。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">selected為已經選擇的課程。</span></li>
                        <li><span style="font-family:Courier New,Courier,monospace">此函式計算並回傳每日的選課清單。</span></li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">def selectCourse(candidates,
                            selected):<br>&nbsp; &nbsp; # 請完成並繳交本函式</span></p>
                </td>
            </tr>
        </tbody>
    </table>
    <p><br></p>
    {% folding yellow, 測資 %}
    <p><span style="font-family:Courier New,Courier,monospace"><strong>範例測資：<br>測資1<br>輸入</strong><br>11<br>2 D 5 7<br>3
            C 2 3<br>1 C 5 6<br>2 E 7 8<br>1 B 2 4<br>2 A 5 6<br>3 E 5 7<br>1 D 6 8<br>1 A 1 2<br>3 F 5 6<br>2 B 1
            4<br><strong>輸出</strong><br>1 A 1 2 &nbsp;<br>1 C 5 6 &nbsp;<br>2 B 1 4 &nbsp;<br>2 D 5 7 &nbsp;<br>3 F 5 6
            &nbsp;</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資2<br>輸入</strong><br>10<br>1 A 1 3<br>1 B 3
            6<br>1 C 5 7<br>2 A 2 4<br>2 B 5 7<br>2 E 3 5<br>3 B 6 8<br>3 D 3 5<br>3 C 4 6<br>3 F 5
            7<br><strong>輸出</strong><br>1 A 1 3<br>1 C 5 7<br>2 E 3 5<br>3 D 3 5<br>3 B 6 8</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資3<br>輸入</strong><br>12<br>1 A 1 3<br>2 B 2
            5<br>3 C 3 5<br>1 B 4 6<br>2 E 5 8<br>3 F 3 5<br>2 C 1 3<br>2 D 4 6<br>2 F 3 5<br>1 C 5 8<br>2 G 7 8<br>3 D
            6 8<br><strong>輸出</strong><br>1 A 1 3<br>1 B 4 6<br>2 C 1 3<br>2 D 4 6<br>2 G 7 8<br>3 F 3 5</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資4<br>輸入</strong><br>9<br>1 A 1 3<br>2 B 3
            4<br>3 C 4 6<br>2 C 5 7<br>2 D 6 8<br>3 F 4 6<br>1 B 6 8<br>2 F 3 5<br>3 E 1 3<br><strong>輸出</strong><br>1 A
            1 3<br>1 B 6 8<br>2 F 3 5<br>2 D 6 8<br>3 E 1 3<br>3 C 4 6</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>測資5<br>輸入</strong><br>8<br>1 D 1 3<br>1 E 4
            6<br>2 A 1 3<br>2 B 2 4<br>3 B 5 7<br>3 E 4 6<br>1 C 3 5<br>2 C 6 8<br><strong>輸出</strong><br>1 D 1 3<br>1 E
            4 6<br>2 A 1 3<br>2 C 6 8<br>3 B 5 7</span></p>
    {% endfolding %}
</body>

```c#
using System;
using System.Collections.Generic;
using System.Text;

namespace csharp
{
    public static class Global
    { // 全域變數
        public static int rs = 0; // 紀錄選課數量（results）
    }
    class Q4
    {
        public struct Course
        { // 課程
            public int day;
            public char name;
            public int start;
            public int end;
        }
        static void SelectCourse(Course[] results, bool[] selected, Course[] candidates, int cs)
        {
            // 你的程式碼
        }

        static void Main()
        {
            Course[] allcourse = new Course[36]; // 所有課程
            Course[] results = new Course[36]; // 選課結果
            int n = Convert.ToInt32(Console.ReadLine());  // 所有課程數量

            bool[] selected = new bool[36]; // 紀錄已選過的課
            for (int i = 0; i < 36; i += 1)
            {
                selected[i] = false;
            }

            for (int i = 0; i < n; i += 1)
            { // 輸入課程
                string[] input = Console.ReadLine().Split(' ');
                allcourse[i].day = Convert.ToInt32(input[0]);
                allcourse[i].name = Convert.ToChar(input[1]);
                allcourse[i].start = Convert.ToInt32(input[2]);
                allcourse[i].end = Convert.ToInt32(input[3]);
            }

            for (int days = 1; days <= 3; days += 1)
            {
                Course[] candidates = new Course[12];
                int cs = 0; // 紀錄candidates有多少
                for (int i = 0; i < n; i += 1)
                {
                    if (allcourse[i].day == days)
                    {
                        candidates[cs] = allcourse[i];
                        cs += 1;
                    }
                }
                SelectCourse(results, selected, candidates, cs);
            }
            for (int i = 0; i < Global.rs; i += 1)
            {
                Console.WriteLine("{0} {1} {2} {3}", results[i].day, results[i].name, results[i].start, results[i].end);
            }

        }
    }
}
```

```python
def selectCourse(candidates, selected):

# 你的程式碼

if __name__ == '__main__':
    n = int(input()) # 所有課程數量

    allcourse = [] # 所有的課程
    candidates = []
    selected = []

    for i in range(n): # 輸入課程資料 將輸入的課程資料全部加在allcourse
        courses = input()
        dataSplit = courses.split(' ')
        allcourse.append([int(dataSplit[0]),dataSplit[1],int(dataSplit[2]),int(dataSplit[3])])

    for i in range(3): # 有三天 所以for 跑三次
        for j in range(n):
            if(allcourse[j][0] == i+1):
                candidates.append(allcourse[j])
        result = selectCourse(candidates, selected)
        candidates = []
        for x in result:
            selected.append(x[1]) # 把選好的課 加入到selected裡
            for z in x: #印出答案
                print( str(z), end = ' ')
            print("")
```
{% endfolding %}

{% folding yellow, 第五題 %}

<body contenteditable="false" class="cke_editable cke_editable_themed cke_contents_ltr cke_show_borders"
    spellcheck="false" style="height: auto; min-height: auto;">
    <p><span style="font-family:Courier New,Courier,monospace">佇列(Queue)具備先進先出(first in first out,
            FIFO)的特性，廣泛的使用於需要排隊機制的應用中。請完成環形佇列函式circular_queue ( )來輔助進行廣度優先搜尋的功能。</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">本題主程式將透過廣度優先搜尋(Breadth First Search,
            BFS)法，從下圖中某一節點開始搜尋，搜尋過程中每一節點會依序透過&nbsp;circular_queue( )函式放入佇列或自佇列中取出。</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><img alt=""
                data-cke-saved-src="/_other/CK/upload/images/1082-Q5-1.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/1082-Q5-1.png"
                style="height:205px; width:400px"></span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸入格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace">P：廣度優先搜尋的起點節點 (0-9)</span></li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸出格式：</strong></span></p>
    <ul>
        <li><span style="font-family:Courier New,Courier,monospace">p1 p2 … p9：廣度優先搜尋依序輸出節點</span></li>
    </ul>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>例如</strong></span></p>
    <p><span style="font-family:Courier New,Courier,monospace">若從節點4開始搜尋，<strong>環狀佇列的變化</strong>如下所示：</span></p>
    <p><span style="font-family:Courier New,Courier,monospace">[0] [1] [2] [3] [4] [5]<br>&nbsp;4 &nbsp; &nbsp; &nbsp;
            &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;<br>&nbsp; &nbsp; &nbsp;1 &nbsp; 3 &nbsp; 5 &nbsp; 6
            &nbsp;&nbsp;<br>&nbsp;2 &nbsp; &nbsp; &nbsp; 3 &nbsp; 5 &nbsp; 6 &nbsp; 0<br>&nbsp;2 &nbsp; &nbsp; &nbsp;
            &nbsp; &nbsp; 5 &nbsp; 6 &nbsp; 0<br>&nbsp;2 &nbsp; 7 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 6 &nbsp;
            0<br>&nbsp;2 &nbsp; 7 &nbsp; 8 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 0<br>&nbsp;2 &nbsp; 7 &nbsp; 8 &nbsp;
            &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;<br>&nbsp; &nbsp; &nbsp;7 &nbsp; 8 &nbsp; &nbsp; &nbsp; &nbsp;
            &nbsp;&nbsp;<br>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;8 &nbsp; 9 &nbsp; &nbsp; &nbsp;&nbsp;<br>&nbsp; &nbsp;
            &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;9</span></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>輸出</strong></span></p>
    <p><span style="font-family:Courier New,Courier,monospace">4 1 3 5 6 0 2 7 8 9</span></p>
    <p><br></p>
    <p><span style="font-family:Courier New,Courier,monospace"><strong>需要完成及繳交的函式（擇一程式語言完成作答即可）：</strong></span></p>
    <table border="1" cellpadding="1" cellspacing="1" style="width:800px">
        <tbody>
            <tr>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C_sharp.png" style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png" src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/C++.png"
                            style="height:25px; width:30px"></span></td>
                <td style="text-align:center"><span style="font-family:Courier New,Courier,monospace"><img alt=""
                            data-cke-saved-src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png"
                            src="https://judge.csie.ntnu.edu.tw/_other/CK/upload/images/Java.png" style="height:29px; width:30px"></span></td>
            </tr>
            <tr>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace"><strong>public static void
                                circular_queue(char c, int y)</strong>函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">其中參數字元c控制此函數執行新增或刪除動作。</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">當新增資料時，整數x為新增的資料內容；當刪除資料時，整數x為傳回的刪除資料項。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">public static void circular_queue(char c,
                            int y) {<br>&nbsp; &nbsp; &nbsp; &nbsp; // 請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">void circular_queue (char c, int* x
                            )函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">其中參數字元c控制此函數執行新增或刪除動作。</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">當新增資料時，整數x為新增的資料內容；當刪除資料時，整數x為傳回的刪除資料項。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">void circular_queue (char c, int* x
                            ){<br>&nbsp; &nbsp; &nbsp; &nbsp; // 請完成並繳交本函式<br>}</span></p>
                </td>
                <td>
                    <p><span style="font-family:Courier New,Courier,monospace">public static void circular_queue(char c,
                            int y)函式</span></p>
                    <ul>
                        <li><span style="font-family:Courier New,Courier,monospace">其中參數字元c控制此函數執行新增或刪除動作。</span></li>
                        <li><span
                                style="font-family:Courier New,Courier,monospace">當新增資料時，整數x為新增的資料內容；當刪除資料時，整數x為傳回的刪除資料項。</span>
                        </li>
                    </ul>
                    <p><span style="font-family:Courier New,Courier,monospace">public static void circular_queue(char c,
                            int y) {<br>&nbsp; &nbsp; &nbsp; &nbsp; // 你的程式碼<br>}</span></p>
                </td>
            </tr>
        </tbody>
    </table>
    <p><br></p>
    {% folding yellow, 測資 %}
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>範例測資：<br>測資1<br>輸入</strong><br>1<br><strong>輸出</strong><br>1<br>0<br>2<br>4<br>3<br>8<br>5<br>6<br>9<br>7</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資2<br>輸入</strong><br>3<br><strong>輸出</strong><br>3<br>0<br>4<br>5<br>1<br>6<br>7<br>2<br>8<br>9</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資3<br>輸入</strong><br>5<br><strong>輸出</strong><br>5<br>3<br>4<br>6<br>7<br>0<br>1<br>8<br>9<br>2</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資4<br>輸入</strong><br>7<br><strong>輸出</strong><br>7<br>5<br>6<br>9<br>3<br>4<br>8<br>0<br>1<br>2</span>
    </p>
    <p><span
            style="font-family:Courier New,Courier,monospace"><strong>測資5<br>輸入</strong><br>9<br><strong>輸出</strong><br>9<br>7<br>8<br>5<br>6<br>2<br>3<br>4<br>1<br>0</span>
    </p>
    {% endfolding %}
</body>

```c#
using System;

namespace csharp
{
    class Program
    {
        public static int N = 10;
        public static int x = 0;
        public static int rear, front;
        public static int[] queue = new int[N];
        public static int[] visited = new int[N];

        static void Main(string[] args)
        {
            int[,] src = new int[,]{
            {0, 1, 0, 1, 0, 0, 0, 0, 0, 0},
            {1, 0, 1, 0, 1, 0, 0, 0, 0, 0},
            {0, 1, 0, 0, 0, 0, 0, 0, 1, 0},
            {1, 0, 0, 0, 1, 1, 0, 0, 0, 0},
            {0, 1, 0, 1, 0, 1, 1, 0, 0, 0},
            {0, 0, 0, 1, 1, 0, 1, 1, 0, 0},
            {0, 0, 0, 0, 1, 1, 0, 1, 1, 0},
            {0, 0, 0, 0, 0, 1, 1, 0, 0, 1},
            {0, 0, 1, 0, 0, 0, 1, 0, 0, 1},
            {0, 0, 0, 0, 0, 0, 0, 1, 1, 0}};
            //Console.WriteLine("請輸入廣度優先走訪的起點位置: ");
            int p = Convert.ToInt16(Console.ReadLine());
            // for (int i = 0 ; i < N ; i++){
            //     visited[i] = 0;
            //     queue[i]=0;
            // } 
            BFS(src, p);

        }
        public static void circular_queue(char c, int y)
        {

            //你的程式碼
        }
        public static void BFS(int[,] src, int p)
        {

            //Console.WriteLine("走訪節點: "+p+"\n");
            Console.WriteLine(p);
            visited[p] = 1;

            for (int i = 0; i < N; i++)
                if (src[p, i] == 1)
                    if (visited[i] != 1)
                    {
                        circular_queue('i', i);

                    }



            while (front != rear)
            {
                circular_queue('d', x);
                if (visited[x] != 1)
                    BFS(src, x);
            }

        }
    }
}
```
{% endfolding %}