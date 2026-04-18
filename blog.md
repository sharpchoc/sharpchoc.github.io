---
layout: default
title: Blog
permalink: /blog/
---

# Blog

A place for short pieces, reviews, and random thoughts.

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
  <div class="post-list-item">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <div class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</div>
    {{ post.excerpt }}
  </div>
  {% endfor %}
{% else %}
No posts yet.
{% endif %}
