---
layout: page
title: Short Stories
permalink: /writing/short-stories/
---

Here I will collect my longer short stories.

<ul>
{% for post in site.posts %}
  {% if post.categories contains "short-stories" %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> — {{ post.date | date: "%d %b %Y" }}</li>
  {% endif %}
{% endfor %}
</ul>
