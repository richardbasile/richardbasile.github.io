---
layout: default
title: Archive
---

## All Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
      <div class="post-details">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p class="post-excerpt">{{ post.excerpt | strip_html }}</p>
      </div>
    </li>
  {% endfor %}
</ul>