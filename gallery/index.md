---
title: Gallery
permalink: /gallery/
nav:
  order: 6
  tooltip: Gallery
---

# {% include icon.html icon="fa-solid fa-images" %} Gallery

<ul class="gallery-list">
  {% assign gallery_posts = site.pages | where_exp: "item", "item.path contains 'gallery/post' and item.layout == 'gallery-post'" | sort: "date" | reverse %}
  {% for post in gallery_posts %}
    <li class="gallery-item-card">
      <p class="gallery-title"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></p>
      <p class="gallery-date">{{ post.date | date: "%Y-%m-%d" }}</p>
      {% if post.images and post.images[0] %}
        <a href="{{ site.baseurl }}{{ post.url }}">
          <img src="{{ site.baseurl }}{{ post.images[0] }}" alt="{{ post.title }}" class="gallery-thumbnail"/>
        </a>
      {% endif %}
    </li>
  {% endfor %}
</ul>

<style>
  .gallery-list {
    list-style: none;
    padding: 0;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    grid-gap: 20px;
  }

  .gallery-item-card {
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 15px;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .gallery-item-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  }

  .gallery-thumbnail {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 4px;
  }

  .gallery-date {
    color: #666;
    font-size: 0.9em;
  }

  .gallery-item-card p.gallery-title {
    font-size: 1.0em;
    margin-top: 0;
    margin-bottom: 8px;
  }

  .gallery-item-card p.gallery-title a {
    text-decoration: none;
    color: inherit;
  }

  .gallery-item-card p.gallery-title a:hover,
  .gallery-item-card p.gallery-title a:visited,
  .gallery-item-card p.gallery-title a:active {
    color: inherit;
    text-decoration: none;
  }
</style>