---
layout: default
title: "Blog"
---

# Blog

{% for post in site.posts %}
<div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 15px;">
  <div><a href="{{ post.url }}">{{ post.title }}</a></div>
  <div style="color: #666; font-size: 0.9em;">{{ post.date | date: "%Y-%m-%d" }}</div>
</div>
{% endfor %}
