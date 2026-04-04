---
layout: page
title: Short Stories
permalink: /writing/short-stories/
---

## Short Stories
This is the place for my short stories, longer scenes or worldbuilding pieces.

---

{% raw %}
{% for post in site.posts %}
  {% if post.categories contains "short-stories" %}
    - [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%d %b %Y" }}
  {% endif %}
{% endfor %}
{% endraw %}
