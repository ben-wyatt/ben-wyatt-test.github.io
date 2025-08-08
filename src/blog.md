---
layout: layout.njk
title: Blog
---

# Blog

Welcome to my blog.  
I write about things I find interesting, from short notes to longer essays.

---

{% for post in collections.post %}
- <a href="{{ post.url }}">{{ post.data.title }}</a> — {{ post.date | date("yyyy-MM-dd") }}
{% endfor %}
