---
title: "Image Gallery"
layout: 'layouts/normal.njk'
permalink: "gallery.html"
---

{% for item in collections.images %}
    <h3><a href="{{ item.url }}">{{ item.data.title }}</a></h3>
    {% if item.data.description %}
    <p>{{ item.data.description }}</p>
    {% endif %}
  <img src="{{ item.data.imgSrc }}" alt="{{ item.data.title }}">
{% else %}
<p>No images found. Tag pages with `image` in frontmatter to include them.</p>
{% endfor %}