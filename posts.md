---
layout: list_posts
title: Blog Posts
subtitle: Some information to share
use-site-title: false
permalink:/posts/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>