---
layout: default
title: "Beranda"
---

<div class="container">
  <h2>Postingan Terbaru</h2>

  {% for post in site.posts limit:5 %}
    <article class="post">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p><small>{{ post.date | date: "%d %B %Y" }}</small></p>
      {{ post.excerpt }}
      <p><a href="{{ post.url | relative_url }}">Baca selengkapnya...</a></p>
    </article>
  {% endfor %}

  <p><a href="{{ '/posts' | relative_url }}">Lihat semua postingan →</a></p>
</div>
