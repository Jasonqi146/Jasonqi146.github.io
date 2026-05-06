---
layout: default
permalink: /blog/
title: blog
nav: true
nav_order: 5
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 20
  sort_field: date
  sort_reverse: true
---

<div class="post blog-simple">
  <header class="post-header">
    <h1 class="post-title">blog</h1>
  </header>

  <article>
    <ul class="simple-post-list">
      {% for post in site.posts %}
        <li>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
          {% if post.redirect == blank %}
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          {% elsif post.redirect contains '://' %}
            <a href="{{ post.redirect }}" target="_blank" rel="noopener noreferrer">{{ post.title }}</a>
          {% else %}
            <a href="{{ post.redirect | relative_url }}">{{ post.title }}</a>
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  </article>
</div>
