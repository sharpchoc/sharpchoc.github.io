---
layout: default
title: Blog
permalink: /blog/
---

# Blog

<div class="entry-list">
{% if site.posts.size > 0 %}
  {% for post in site.posts %}
  <div class="entry-item">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <div class="meta-line">{{ post.date | date: "%B %-d, %Y" }}</div>
    <p>{{ post.excerpt | strip_html | strip_newlines }}</p>
  </div>

  <hr>
  {% endfor %}
{% else %}
No posts yet.
{% endif %}
</div>
