---
layout: page
title: Gallery
permalink: /gallery/
---

<div class="gallery">
  {% for photo in site.data.gallery %}
    <figure class="gallery-item">
      <img src="/assets/images/{{ photo.file }}" alt="{{ photo.alt }}" loading="lazy">
      {% if photo.caption %}
        <figcaption>{{ photo.caption }}</figcaption>
      {% endif %}
    </figure>
  {% endfor %}
</div>
