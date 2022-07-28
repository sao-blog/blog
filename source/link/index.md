---
title: 友情鏈接
date: 2022-02-03 14:20:03
type: "link"
description: "友情鏈接"
---

{% issues sites | api=https://api.github.com/repos/sao-coding/blog-gitalk/issues/1/comments?sort=updated&state=open&labels=審核通過 | group=group:来自 GitHub 的朋友 %}


## 如何添加自己的博客鏈接


{% timeline %}
<!-- timeline <p style="font-size:15px;line-height:22px;">第一步：在 <span style="font-size:25px;color:red">Gitalk</span> 留言，按照格式填寫並提交</p> -->

~~~json
```json
{
    "title": "站點名稱",
    "screenshot": "站點預覽圖鏈接",
    "url": "站點鏈接",
    "頭像": "標題",
    "description": "站點描述",
    "group": "作為分組名"
}
```
~~~

~~~json
```json
{
    "title": "",
    "screenshot": "",
    "url": "",
    "avatar": "",
    "description": "",
    "group": "来自 GitHub 的朋友"
}
```
~~~

{% span red large, 分組名稱不能改! %}

為了提高圖片加載速度，建議優化圖片尺寸：

打開 壓縮圖 上傳自己的截圖，將圖片的高度調整到 400px 後下載。
將壓縮後的圖片上傳到 ImgURL免費圖床 或 隨便一個圖床 並使用此圖片鏈接作為截圖鏈接。

<!-- endtimeline -->

<!-- timeline 第二步：刷新 -->
刷新頁面即可生效
<!-- endtimeline -->
{% endtimeline %}

## 如何更新自己的博客鏈接

- 如果是自己留言的 Gitalk ，可以自己修改。
- 如果是管理員創建的，請自己重新創建一份，然後讓管理員刪掉舊的