---
layout: default
title: Home
---

# Welcome to My Blog
This is a simple markdown-based blog running on Jekyll.

## Latest Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date: "%Y-%m-%d" }})
    </li>
  {% endfor %}
</ul>
