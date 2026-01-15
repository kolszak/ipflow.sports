---
title: "Foto"
excerpt: "zdjęcia z imprez sportowych"
layout: splash
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/rizo_www.JPG
  #actions:
  #  - label: "OneDrive"
  #    url: "#test-link"
intro:
    - excerpt: "Ostatnia impreza biegowa na której fotografowałem:"
intro2:
    - excerpt: "***Gdzie mnie spotkasz:"
feature_row:
  - image_path: /assets/images/splash/parkrun-splash.JPG
    alt: "Parkrun"
    title: "Parkrun Toruń"
    excerpt: "Parkrun w **Toruniu**"
    image_caption: "Image courtesy of [Unsplash](https://parkrun.pl/)"
  - image_path: /assets/images/splash/ulica-splash.jpg
    #image_caption: "Image courtesy of [Unsplash](https://run-torun/)"
    alt: "Biegi uliczne"
    title: "Biegi uliczne"
    excerpt: "Biegi **uliczne** w okolicach Torunia."
    url: "/posts/"
    type: "center"
    btn_label: "Zobacz listę zdjęć"
    btn_class: "btn--info"
  - image_path: /assets/images/splash/basen-splash.jpg
    title: "Pływanie"
    excerpt: "Czasem basen"
---
{% include feature_row id="intro" type="center" %}
{% include feature_row_latest.html %}
{% include feature_row id="intro2" type="center" %}
{% include feature_row %}
