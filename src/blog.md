---
permalink: "/blog.html"
layout: 'layouts/normal.njk'
title: "Blog - des"
---

## Blog

### [Diary](blog/diary.html) - Last updated 9/13/2026

<ul>
{% for post in collections.diary | reverse %}
<li><a href="{{ post.url }}">{{ post.data.title }}</a></li>
{% endfor %}
</ul>

<hr class="simplehr">

<ul>
{% for post in collections.blog | reverse %}
<li><a href="{{ post.url }}">{{ post.data.title }}</a></li>
{% endfor %}
</ul>