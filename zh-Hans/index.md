---
title: 试一试MNH48网站的主题包
description: 这是来试试主题包在华文版本中如何表现
lang: zh-Hans
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


- [段落标题](#段落标题)
  - [小标题](#小标题)
    - [另一个较小的标题](#另一个较小的标题)
    - [灯箱画廊样本](#灯箱画廊样本)
{: .toc id="toc" data-title="内容"}


这只是来试试本主题包如何表现。


&nbsp;


## 段落标题
{: style="clear: none;"}

### 小标题
{: style="clear: none;"}

#### 另一个较小的标题
{: style="clear: none;"}

这是一个简体版的新马华文段落。


**这是粗体的文字。**


这是带下划线的文字。
{: style="text-decoration:underline;"}


*这是斜体的文字。*


[这段文字有链接](#)


这是一个排序列表

1. 第一项
2. 第二项


这是一个未排序的列表

- 某一件事
- 另一件事


这是一个可收起的文本
{% capture markdowntextinbox %}
#### 可收起的文本之中的另一个较小的标题
这是*某个*文本**的**样本。
{% endcapture -%}
{% include toggletext.html boxid="文本样本" boxtitle="单击这里来看所写的文本" boxcontent=markdowntextinbox -%}


这是一个可收起的图盒，图盒中有YouTube的内嵌视频
{% capture ytembed %}{% include iframe.html iframeurl="https://www.youtube.com/embed/dQw4w9WgXcQ" iframewidth="600" iframeheight="320" %}{% endcapture -%}
{% include togglefigure.html boxid="图盒样本" boxtitle="单击这里来看爆雷标签着的视频的样本" boxcontent=ytembed boxcaption="这是一个示例说明" -%}


这是一个按钮
{: style="text-align:center;" id="按钮"}

[单击我](#按钮)
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
样本图片
别的样本图片
有食物可以吃
电车上有卖食物
{% endcapture -%}
{% assign gallerycaption = gallerycaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture imagecaption_array %}
吉隆坡中央车站的指示牌
持有商务舱电车票的人可以无限饮料
三明治与红茶
在电车上也有卖食物
{% endcapture -%}
{% assign imagecaption = imagecaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% include imagegallery.html gallerytitle="灯箱画廊样本" gallerycount="4" galleryname="sample" gallerythumb=gallerythumb gallerycaption=gallerycaption -%}
{% include imagelightbox.html gallerycount="4" galleryname="sample" galleryimage=galleryimage imagecaption=imagecaption -%}


&nbsp;

