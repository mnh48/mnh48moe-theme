---
title: 試一試MNH48網站的主題包
description: 這是來試試主題包在華文版本中如何表現
lang: zh-Hant
hasENG: true
hasRMI: true
hasJWI: true
hasRJG: true
hasBRG: true
hasSCH: true
hasTCH: true
hasJPN: true
layout: article
needbtt: true
---


- [段落標題](#段落標題)
  - [小標題](#小標題)
    - [另一個較小的標題](#另一個較小的標題)
    - [燈箱畫廊樣本](#燈箱畫廊樣本)
{: .toc id="toc" data-title="內容"}


這只是來試試本主題包如何表現。


&nbsp;


## 段落標題
{: style="clear: none;"}

### 小標題
{: style="clear: none;"}

#### 另一個較小的標題
{: style="clear: none;"}

這是一個繁體版的新馬華文段落。


**這是粗體的文字。**


這是帶下劃線的文字。
{: style="text-decoration:underline;"}


*這是斜體的文字。*


[這段文字有鏈接](#)


這是一個排序列表

1. 第一項
2. 第二項


這是一個未排序的列表

- 某一件事
- 另一件事


這是一個可收起的文本
{% capture markdowntextinbox %}
#### 可收起的文本之中的另一個較小的標題
這是*某個*文本**的**樣本。
{% endcapture -%}
{% include toggletext.html boxid="文本樣本" boxtitle="單擊這裡來看所寫的文本" boxcontent=markdowntextinbox -%}


這是一個可收起的圖盒，圖盒中有YouTube的內嵌視頻
{% capture ytembed %}{% include iframe.html iframeurl="https://www.youtube.com/embed/dQw4w9WgXcQ" iframewidth="600" iframeheight="320" %}{% endcapture -%}
{% include togglefigure.html boxid="圖盒樣本" boxtitle="單擊這裡來看爆雷標籤著的視頻的樣本" boxcontent=ytembed boxcaption="這是一個示例說明" -%}


這是一個按鈕
{: style="text-align:center;" id="按鈕"}

[單擊我](#按鈕)
{: .button .button300}


{% capture gallerythumb_array %}
https://file.mnh48.moe/transit/2022/11/ge15/b_2_kl-sentral-waypoint-signboard-small.jpg
https://file.mnh48.moe/transit/2022/11/ge15/f_2_free-flowing-drink-small.jpg
https://file.mnh48.moe/transit/2022/11/ge15/g_5_sandwich-and-tea-small.jpg
https://file.mnh48.moe/transit/2022/11/ge15/i_2_bistro-onboard-train-small.jpg
{% endcapture -%}
{% assign gallerythumb = gallerythumb_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture galleryimage_array %}
https://file.mnh48.moe/transit/2022/11/ge15/b_2_kl-sentral-waypoint-signboard.jpg
https://file.mnh48.moe/transit/2022/11/ge15/f_2_free-flowing-drink.jpg
https://file.mnh48.moe/transit/2022/11/ge15/g_5_sandwich-and-tea.jpg
https://file.mnh48.moe/transit/2022/11/ge15/i_2_bistro-onboard-train.jpg
{% endcapture -%}
{% assign galleryimage = galleryimage_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture gallerycaption_array %}
樣本圖片
別的樣本圖片
有食物可以吃
電車上有賣食物
{% endcapture -%}
{% assign gallerycaption = gallerycaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture imagecaption_array %}
吉隆坡中央車站的指示牌
持有商務艙電車票的人可以無限飲料
三明治與紅茶
在電車上也有賣食物
{% endcapture -%}
{% assign imagecaption = imagecaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% include imagegallery.html gallerytitle="燈箱畫廊樣本" gallerycount="4" galleryname="sample" gallerythumb=gallerythumb gallerycaption=gallerycaption -%}
{% include imagelightbox.html gallerycount="4" galleryname="sample" galleryimage=galleryimage imagecaption=imagecaption -%}


&nbsp;

