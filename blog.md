---
layout: blog
permalink: /blog/
title: Blog
---

<header class="blog-header">
  <h1 class="blog-heading">Blog</h1>
  <p class="blog-intro">Notes on robotics, embodied AI, and the occasional engineering detour.</p>
</header>

<div class="blog-list">  {% for post in site.posts %}
  <article class="blog-item">
    {% if post.image %}
    <a class="blog-item-thumb" href="{{ post.url | relative_url }}"><img src="{{ post.image | relative_url }}" alt="{{ post.title | escape }}" loading="lazy"></a>
    {% endif %}
    <div class="blog-item-body">
      <h2 class="blog-item-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="blog-item-meta">
        <time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: "%b %d, %Y" }}</time>
        {% assign words = post.content | number_of_words %}
        · {{ words | divided_by: 180 | plus: 1 }} min read
      </p>
      <p class="blog-item-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      <a class="blog-item-more" href="{{ post.url | relative_url }}">Read more →</a>
    </div>
  </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
<p class="blog-empty">No posts yet. Stay tuned!</p>
{% endif %}
