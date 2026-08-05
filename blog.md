---
layout: blog
permalink: /blog/
title: Blog
---

<header class="blog-header">
  <p class="blog-kicker">TECHNICAL NOTES</p>
  <h1 class="blog-heading">Blog</h1>
  <p class="blog-intro">Notes on robotics, embodied AI, and the occasional engineering detour.</p>
</header>

<div class="blog-grid">
  {% for post in site.posts %}
  <article class="blog-card">
    <a class="blog-card-media" href="{{ post.url }}">
      {% if post.image %}<img src="{{ post.image }}" alt="{{ post.title }}" loading="lazy" />{% endif %}
    </a>
    <div class="blog-card-body">
      <h3 class="blog-card-title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="blog-card-meta">
        {{ post.date | date: "%b %d, %Y" }}
        {% assign words = post.content | number_of_words %}
        · {{ words | divided_by: 180 | plus: 1 }} min read
      </p>
      <p class="blog-card-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      <a class="blog-card-more" href="{{ post.url }}">Read more →</a>
    </div>
  </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
<p class="blog-empty">No posts yet. Stay tuned!</p>
{% endif %}
