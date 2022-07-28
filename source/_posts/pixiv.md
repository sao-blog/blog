---
title: Pixiv 日榜小工具
date: 2022-01-30 21:33:31
updated: 2022-01-30 21:33:31
description: Pixiv 日榜
keywords: hexo,butterfly,pixiv
swiper_index: 102
sticky: 1
katex:
categories:
  - HEXO
tags:
  -  HEXO
  - "\U0001F98B Butterfly"
---

# Butterfly 主题

1. 在`themes\Butterfly\layout\includes\widget`文件夾新建`card_pixiv.pug`文件，文件內容如下：

{% codeblock lang:pug mark:6 %}
.card-widget.card-pixiv
  .card-content
    .item-headline
      i.fa.fa-image(aria-hidden="true")
      span= _p('aside.card_pixiv')
    iframe(src="https://cloud.mokeyjay.com/pixiv" frameborder="0" style="width:99%;height:380px;margin:0;")
{% endcodeblock %}

{% note warning flat %}
`https://cloud.mokeyjay.com/pixiv`
使用的是超能小紫提供的服務，也可以自行搭建，搭建方式請看這裡
{% link Pixiv 每日排行榜小部件 v4.4.1,https://www.mokeyjay.com/archives/1063, https://www.mokeyjay.com/headimg.png %}
{% endnote %}

{% note info flat %}
`https://sao.dsmynas.com/pixiv`
我自己也有架設一個也可以用我的

如果自己架設的，想跟換點擊圖片後的連接可以改這[部分](https://github.com/sao-coding/Pixiv-daily-ranking-widget/blob/9d26e568ef1b12eaa510f56c8632c4feb6b241d4/app/Views/index.php#L40)

- 可使用`str_replace()`這個函數
`str_replace( search , replace , subject , count )`
參數說明：search 是要被替換的字串 , replace 是要替換上去的新字串 , subject 是原始字串 , count 是來統計更換數量的參數，選用。
{% endnote %}

2. 編輯`themes\Butterfly\layout\includes\widget\index.pug`文件，在你想要顯示的位置插入以下代碼：
```pug
if theme.aside.card_pixiv
  include ./card_pixiv.pug
```

3. 編輯`butterfly.yml`文件，在`card_webinfo`下面添加一行`card_pixiv: true`

4. 編輯`themes\Butterfly\languages\zh-TW.yml`文件(請根據你的網站語言選擇)，找到`card_announcement: 公告`, 在下面添加一行`card_pixiv: Pixiv日榜Top50`(後面的文本可自定義)

5. 如果不想顯示，直接把`butterfly.yml`文件的`card_pixiv: true`改為`card_pixiv: false`即可

# 其他主题

將以下內容插入到需要顯示的地方:
```html
<iframe src="https://cloud.mokeyjay.com/pixiv" frameborder="0" style="width:100%;height:380px;margin:0;"></iframe>
```