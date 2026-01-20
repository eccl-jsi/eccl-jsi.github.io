---
title: "ECCL - Cover Gallery"
layout: page
title: Cover Gallery
permalink: /cover_gallery.html
---

<p>
  Intro text for the page. You can explain what visitors are seeing here.
</p>

<div class="gallery-grid">
  {% for item in site.data.gallery %}
    <figure class="gallery-card">
      <a href="{{ item.image }}" class="gallery-image-link">
        <img src="{{ item.image }}" alt="{{ item.alt | escape }}" loading="lazy">
      </a>

      {% if item.title %}
        <figcaption class="gallery-caption">
          <div class="gallery-title">{{ item.title }}</div>
          {% if item.text %}
            <div class="gallery-text">{{ item.text }}</div>
          {% endif %}

          {% if item.links %}
            <div class="gallery-links">
              {% for l in item.links %}
                <a href="{{ l.url }}" {% if l.url contains 'http' %}rel="noopener noreferrer"{% endif %}>
                  {{ l.label }}
                </a>
              {% endfor %}
            </div>
          {% endif %}
        </figcaption>
      {% endif %}
    </figure>
  {% endfor %}
</div>
