---
layout: splash
permalink: /
hidden: true
title: " "
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/home/oddworld_header.jpg
  actions:
  caption: "Photo credit: [**Oddworld inhabitants**](http://www.oddworld.com/)"
excerpt: >
  **This site contains articles, resources and tutorials about game design, programming, 3D modelling and other game development topics using free software.**
feature_row:
  - image_path: /assets/images/home/home_godot.png
    alt: "Rendered in Godot"
    title: "Rendered in Godot"
    excerpt: "Godot engine is a powerful development tool with 2D and 3D capabilities. Is simple and user friendly, still capable of wonderful things."
  - image_path: /assets/images/home/home_open_source.png
    alt: "Built wih open source"
    title: "Built wih open source"
    excerpt: "The open source community keeps growing, creating incredible tools and  empowering users all around the world"
  - image_path: assets/images/home/home_linux.png
    alt: "Powered by Linux               "
    title: "Powered by Linux"
    excerpt: "The most popular open source operating system of the world puts you in control of your system, not the other way around."
---

{% include feature_row %}
<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>
{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>
