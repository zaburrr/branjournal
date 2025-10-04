---
layout: default
title: Postingan
---

<h2>Semua Postingan</h2>

{% for post in site.posts %}
<article class="post">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
</article>
{% endfor %}
