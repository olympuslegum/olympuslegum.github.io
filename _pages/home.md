---
title: "Olympus Legum"
layout: splash
permalink: /
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_image: splash.jpg
  caption: "Photo credit: [**Wallpaper Abyss**](https://wall.alphacoders.com/big.php?i=26102)"
excerpt: "Digital Legal Coverage Worldwide"
intro: 
  - excerpt: 'Dedicated to bringing the best analysis of current news and how it relates to the Law in India and the world' 
feature_row:
  - image_path: law.jpg
    alt: "placeholder image 1"
    title: "Placeholder 1"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: kanun.jpg
    alt: "placeholder image 2"
    title: "Placeholder 2"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - image_path: law.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
---

{% include feature_row id="intro" type="center" %}

<!-- {% include feature_row %} -->
<div class="archive">
  {% unless page.header.overlay_color or page.header.overlay_image %}
  <h1 class="page__title">{{ page.title }}</h1>
        {% endunless %}
  <div class="grid__wrapper">
    {% for post in site.posts %}
      {% include archive-single.html type="grid" %}
    {% endfor %}
  </div>
</div>
