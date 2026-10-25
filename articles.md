---
layout: default
title: Articles
description: "Articles on software engineering, Linux, and open source."
permalink: /articles/
---

<div class="page-heading">
  <p class="eyebrow">THE ARCHIVE</p>
  <h1>Articles</h1>
  <p class="page-description">Notes, experiences, and lessons from building with technology.</p>
</div>

<section class="article-list" aria-label="Published articles">
  {% for post in site.posts %}
  <article class="article-item">
    <p class="article-date">{{ post.date | date: "%b %-d, %Y" }}</p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
    <a class="read-link" href="{{ post.url | relative_url }}">Read article →</a>
  </article>
  {% endfor %}
</section>
