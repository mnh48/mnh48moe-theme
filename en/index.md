---
title: MNH48 Theme Test
description: This is a test for how the theme is in English
lang: en
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


- [Paragraph Title](#paragraph-title)
  - [Smaller title](#smaller-title)
    - [Another smaller title](#another-smaller-title)
    - [Sample Lightbox Gallery](#sample-lightbox-gallery)
{: .toc id="toc" data-title="The Content"}


This is just a test to show the theme itself.


&nbsp;


## Paragraph Title
{: style="clear: none;"}

### Smaller title
{: style="clear: none;"}

#### Another smaller title
{: style="clear: none;"}

This is an English paragraph.


**This is bold text.**


This is underlined text.
{: style="text-decoration:underline;"}


*This is italic text.*


[This text has a link](#)


This is a sorted list

1. First item
2. Second item


This is an unsorted list

- Something
- Another thing


This is a collapsible box containing text
{% capture markdowntextinbox %}
#### Another smaller header inside collapsible box
This *is* **sample** text.
{% endcapture -%}
{% include toggletext.html boxid="textexample" boxtitle="Click to open text" boxcontent=markdowntextinbox -%}


This is a collapsible box containing figure (in this case, the figure hold YouTube embed iframe)
{% capture ytembed %}{% include iframe.html iframeurl="https://www.youtube.com/embed/dQw4w9WgXcQ" iframewidth="600" iframeheight="320" %}{% endcapture -%}
{% include togglefigure.html boxid="figexample" boxtitle="Click for example video spoiler" boxcontent=ytembed boxcaption="This is example of a caption" -%}


This is a button
{: style="text-align:center;" id="button"}

[Click me](#button)
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
Some sample image
Another sample image
Grab some food
Bistro on train
{% endcapture -%}
{% assign gallerycaption = gallerycaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture imagecaption_array %}
Signboard at KL Sentral station
Free-flowing drink for business class ticket holder
Sandwich and plain tea
Bistro on train selling food
{% endcapture -%}
{% assign imagecaption = imagecaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% include imagegallery.html gallerytitle="Sample Lightbox Gallery" gallerycount="4" galleryname="sample" gallerythumb=gallerythumb gallerycaption=gallerycaption -%}
{% include imagelightbox.html gallerycount="4" galleryname="sample" galleryimage=galleryimage imagecaption=imagecaption -%}


&nbsp;

