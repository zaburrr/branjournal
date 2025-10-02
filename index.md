---
layout: default
title: Beranda
---

{% for post in paginator.posts %}
<article class="post">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
</article>
{% endfor %}
