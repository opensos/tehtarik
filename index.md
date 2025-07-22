---
layout: default
title: Galeri Gambar
---

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 p-4">
  {% for post in site.posts %}
    <a href="{{ post.url }}" class="block text-center">
      <img src="{{ post.image }}" alt="{{ post.title }}" class="mx-auto mb-2 rounded-lg shadow-md" />
      <p class="text-gray-700">{{ post.description }}</p>
    </a>
  {% endfor %}
</div>
