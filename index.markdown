---
layout: home
title: Home
---

{% for post in site.posts %}
  {% assign image_filename = post.title | append: ".png" %}
<div class="grid-item">
  <a href="{{ post.url }}">
    <img src="{{ site.baseurl }}/thumbs/{{ image_filename }}" alt="{{ post.title }}">
    <div class="overlay">{{ post.title }}</div>
  </a>
</div>
{% endfor %}

