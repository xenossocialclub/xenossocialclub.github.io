---
layout: page
title: Flash Fiction
permalink: /writing/flash-fiction/
---

## Flash Fiction

{% raw %}
{% for post in site.posts %}
  {% if post.categories contains "flash-fiction" %}
    - [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%d %b %Y" }}
  {% endif %}
{% endfor %}
{% endraw %}
