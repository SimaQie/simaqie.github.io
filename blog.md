---
layout: homepage
permalink: /blog/
title: Blog
---

## Blog

{% for post in site.posts %}
<div class="blog-entry">
  {% if post.image %}
  <a href="{{ post.url }}" class="blog-thumb"><img src="{{ post.image }}" alt="{{ post.title }}" /></a>
  {% endif %}
  <div class="blog-info">
    <h3 class="blog-title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="blog-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p class="blog-excerpt">{{ post.excerpt | strip_html | truncate: 180 }}</p>
  </div>
</div>
{% endfor %}

{% if site.posts.size == 0 %}
<p>No posts yet. Stay tuned!</p>
{% endif %}
