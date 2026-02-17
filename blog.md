---
layout: default
title: Blog
---

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date_to_string }} - {{ post.author }}</p>
      <div>{{ content }}</div>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
