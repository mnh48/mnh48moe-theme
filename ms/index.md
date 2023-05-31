---
title: Cuba Tema MNH48
description: Ini percubaan untuk tengok tema digunakan dalam bahasa Melayu
lang: ms
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


- [Tajuk Perenggan](#tajuk-perenggan)
  - [Tajuk kecil](#tajuk-kecil)
    - [Tajuk kecil yang lain](#tajuk-kecil-yang-lain)
    - [Contoh galeri jenis kotak cahaya](#contoh-galeri-jenis-kotak-cahaya)
{: .toc id="toc" data-title="Kandungan"}


Ini hanyalah percubaan untuk tunjukkan tema itu sendiri.


&nbsp;


## Tajuk Perenggan
{: style="clear: none;"}

### Tajuk kecil
{: style="clear: none;"}

#### Tajuk kecil yang lain
{: style="clear: none;"}

Ini perenggan bahasa Melayu bertulisan rumi.


**Ini tulisan yang ditebalkan.**


Ini tulisan yang digariskan.
{: style="text-decoration:underline;"}


*Ini tulisan yang dicondongkan.*


[Tulisan ini ada pautan](#)


Ini senarai yang bersusun

1. Perkara pertama
2. Perkara kedua


Ini senarai yang tidak bersusun

- Sesuatu
- Benda lain


{% capture ytembed %}{% include iframe.html iframeurl="https://www.youtube.com/embed/dQw4w9WgXcQ" iframewidth="600" iframeheight="320" %}{% endcapture -%}
{% include togglebox.html boxid="contoh" boxtitle="Klik untuk contoh bocoran video" boxcontent=ytembed boxcaption="Ini contoh butiran kecil" -%}


Ini suatu butang
{: style="text-align:center;" id="butang"}

[Tekan saya](#butang)
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
Contoh gambar
Contoh gambar yang lain
Makan dulu
Bistro atas kereta api
{% endcapture -%}
{% assign gallerycaption = gallerycaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% capture imagecaption_array %}
Papan tanda di stesen KL Sentral
Minuman percuma untuk pemegang tiket kelas perniagaan
Sandwic dan teh o
Bistro atas kereta api menjual makanan
{% endcapture -%}
{% assign imagecaption = imagecaption_array | strip | newline_to_br | strip_newlines | split: "<br />" -%}

{% include imagegallery.html gallerytitle="Contoh galeri jenis kotak cahaya" gallerycount="4" galleryname="sample" gallerythumb=gallerythumb gallerycaption=gallerycaption -%}
{% include imagelightbox.html gallerycount="4" galleryname="sample" galleryimage=galleryimage imagecaption=imagecaption -%}


&nbsp;

