---
layout: page
title: Flash Fiction
permalink: /writing/flash-fiction/
---

Here I will post flash fiction pieces, vignettes and short atmospheric scenes.

<ul>
{% for post in site.posts %}
  {% if post.categories contains "flash-fiction" %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> — {{ post.date | date: "%d %b %Y" }}</li>
  {% endif %}
{% endfor %}
</ul>

