---
layout: page
title: Flash Fiction
permalink: /writing/flash-fiction/
---

Brief scenes, vignettes and short atmospheric pieces.

<div class="post-list">
{% for post in site.posts %}
  {% if post.categories contains "flash-fiction" %}
    <article class="post-preview">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="post-meta">{{ post.date | date: "%d %b %Y" }}</p>

      {% if post.excerpt %}
        <p class="post-excerpt">{{ post.excerpt }}</p>
      {% endif %}

      {% if post.tags %}
        <p class="post-tags">
          {% for tag in post.tags %}
            <span>#{{ tag }}</span>
          {% endfor %}
        </p>
      {% endif %}

      <p><a href="{{ post.url | relative_url }}">Read more →</a></p>
    </article>
  {% endif %}
{% endfor %}
</div>
