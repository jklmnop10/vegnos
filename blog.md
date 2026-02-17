---
layout: default
title: Blog
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <article>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.author }} | {{ post.date | date_to_string }}</p>
      {{ post.excerpt }}
      </article>
    </li>
  {% endfor %}
</ul>
