---
layout: default
title: Blog
permalink: /blog/
---

# Blog

<div class="entry-list">
{% if site.posts.size > 0 %}
  {% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})

<div class="meta-line">{{ post.date | date: "%B %-d, %Y" }}</div>

{{ post.excerpt }}

* * *
  {% endfor %}
{% else %}
No posts yet.
{% endif %}
</div>
