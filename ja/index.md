---
title: MNH48サイトテーマ試用
description: ウェブサイトテーマが日本語でどのように見えるかのテストです。
lang: ja
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


- [段落名](#段落名)
  - [小題](#小題)
    - [小さなサブトピック](#小さなサブトピック)
    - [ライトボックスギャラリーのサンプル](#ライトボックスギャラリーのサンプル)
{: .toc id="toc" data-title="内容"}


これはウェブサイトのテーマそのものを見せるためのテストです。


&nbsp;


## 段落名
{: style="clear: none;"}

### 小題
{: style="clear: none;"}

#### 小さなサブトピック
{: style="clear: none;"}

これは日本語の段落です。


**これは太字です。**


これは下線付きの文字です。
{: style="text-decoration:underline;"}


*これは斜体の文字です。*


[この文章にはリンクがあります。](#)


これはソートされた一覧表です。

1. 第一項目
2. 第二項目


これはソートされていない一覧表です。

- 何か
- もうひとつ


これは折りたたみ可能テキストです。
{% capture markdowntextinbox %}
#### 折りたたみ可能テキストでの小さなサブトピック
これ*は*サンプルの**テキスト**です。
{% endcapture -%}
{% include toggletext.html boxid="テキストの例" boxtitle="テキストの例はクリックしてください" boxcontent=markdowntextinbox -%}


これは折りたたみ可能フィギュアです。フィギュアはユーチューブ動画の埋め込みです。
{% capture ytembed %}{% include iframe.html iframeurl="https://www.youtube.com/embed/dQw4w9WgXcQ" iframewidth="600" iframeheight="320" %}{% endcapture -%}
{% include togglefigure.html boxid="フィギュアの例" boxtitle="ビデオスポイラーの例はクリックしてください" boxcontent=ytembed boxcaption="これはキャプションの例です" -%}


これはボタンです。
{: style="text-align:center;" id="ボタン"}

[クリックしてください](#ボタン)
{: .button .button300}


{% capture gallerythumb_array %}
https://file.mnh48.com/transit/2022/11/ge15/b_2_kl-sentral-waypoint-signboard-small.jpg
https://file.mnh48.com/transit/2022/11/ge15/f_2_free-flowing-drink-small.jpg
https://file.mnh48.com/transit/2022/11/ge15/g_5_sandwich-and-tea-small.jpg
https://file.mnh48.com/transit/2022/11/ge15/i_2_bistro-onboard-train-small.jpg
{% endcapture -%}
{% assign gallerythumb = gallerythumb_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture galleryimage_array %}
https://file.mnh48.com/transit/2022/11/ge15/b_2_kl-sentral-waypoint-signboard.jpg
https://file.mnh48.com/transit/2022/11/ge15/f_2_free-flowing-drink.jpg
https://file.mnh48.com/transit/2022/11/ge15/g_5_sandwich-and-tea.jpg
https://file.mnh48.com/transit/2022/11/ge15/i_2_bistro-onboard-train.jpg
{% endcapture -%}
{% assign galleryimage = galleryimage_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture gallerycaption_array %}
サンプル画像
別のサンプル画像
食べ物だぞ
電車でカフェ
{% endcapture -%}
{% assign gallerycaption = gallerycaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture imagecaption_array %}
ＫＬセントラルの看板
ビジネスクラスチケットをお持ちの方限定の飲み放題
サンドイッチとプレーンティー
電車でも食べ物が売る
{% endcapture -%}
{% assign imagecaption = imagecaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% include imagegallery.html gallerytitle="ライトボックスギャラリーのサンプル" gallerycount="4" galleryname="sample" gallerythumb=gallerythumb gallerycaption=gallerycaption -%}
{% include imagelightbox.html gallerycount="4" galleryname="sample" galleryimage=galleryimage imagecaption=imagecaption -%}


&nbsp;

