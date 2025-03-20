---
title: A Dark and Random Jekyll Demo
--- 

## Dark Mode Switch 

Read [my guide to dark mode](https://derekkedziora.com/blog/dark-mode-revisited) to see how I created the dark mode switch on this Jekyll site. 

## Demo Blog Posts 

{% for post in site.posts %}
{% unless post.categories contains "now" %}

[{{ post.title }}]({{ post.url }})

{% endunless %}
{% endfor %}