---
layout: default
title: Home
author_profile: true
---

{% for post in site.posts %}
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  {{ post.date | date: "%B %d, %Y" }}
  {{ post.content }}
{% endfor %}