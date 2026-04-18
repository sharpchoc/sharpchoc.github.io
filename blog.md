---
layout: default
title: Blog
permalink: /blog/
---

# Blog

A place for short pieces, reviews, and random thoughts.

{% if site.posts.size > 0 %}
  <ul class="blog-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <div class="blog-date">{{ post.date | date: "%B %-d, %Y" }}</div>
      </li>
    {% endfor %}
  </ul>
{% else %}
No posts yet.
{% endif %}
