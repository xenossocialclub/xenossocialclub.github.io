---
layout: page
title: Writing
permalink: /writing/
---

This is the writing section of the site, where I collect short fiction, vignettes and longer narrative pieces.

<div class="writing-sections">
  <div class="writing-block">
    border-bottom: dotted 2px black;
    <h2><a href="/writing/flash-fiction/">Flash Fiction</a></h2>
    <p>Brief atmospheric scenes, fragments and character moments.</p>
  </div>

  <div class="writing-block">
    border-bottom: dotted 2px black;
    <h2><a href="/writing/short-stories/">Short Stories</a></h2>
    <p>Longer standalone fiction and more developed narrative pieces.</p>
  </div>
</div>

## Recent Writing

<div class="post-list">
{% for post in site.posts limit:3 %}
  <article class="post-preview">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%d %b %Y" }}</p>

    {% if post.excerpt %}
      <p class="post-excerpt">{{ post.excerpt }}</p>
    {% endif %}

    <p><a href="{{ post.url | relative_url }}">Read more →</a></p>
  </article>
{% endfor %}
</div>
