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
    - excerpt: "Tutaj znajdziesz linki do zdjęć z imprez sportowych na których fotografowałem.<br/>
                Gdzie mnie znajdziesz:"
feature_row:
  - image_path: /assets/images/parkrun.jpg
    alt: "Parkrun"
    title: "Parkrun Toruń"
    excerpt: "Parkrun w **Toruniu**"
  - image_path: /assets/images/parkrun.jpg
    #image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Biegi uliczne"
    title: "Biegi uliczne"
    excerpt: "Biegi **uliczne** w okolicach Torunia."
    url: "/posts/"
    type: "center"
    btn_label: "Zobacz listę zdjęć"
    btn_class: "btn--info"
  - image_path: /assets/images/parkrun.jpg
    title: "Pływanie"
    excerpt: "Czasem basen"
---

{% include feature_row id="intro" type="center" %}

{% assign latest = site.posts.first %}

<div class="feature__wrapper">
  <div class="feature__item">
    {% if latest.header.teaser %}
      <img src="{{ latest.header.teaser | relative_url }}" alt="{{ latest.title }}">
    {% endif %}

    <h2 class="archive__item-title">
      <a href="{{ latest.url | relative_url }}">{{ latest.title }}</a>
    </h2>

    <p class="archive__item-excerpt">
      {{ latest.excerpt | strip_html | truncate: 160 }}
    </p>

    <a href="{{ latest.url | relative_url }}" class="btn btn--primary">
      Czytaj najnowszy wpis
    </a>
  </div>
</div>

{% include feature_row %}
