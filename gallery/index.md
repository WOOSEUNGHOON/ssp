---
title: Gallery
permalink: /gallery/
nav:
  order: 5
  tooltip: Gallery
---

# {% include icon.html icon="fa-solid fa-images" %} Gallery

<ul class="gallery-list" id="gallery-list">
  {% assign gallery_posts = site.pages | where_exp: "item", "item.path contains 'gallery/post' and item.layout == 'gallery-post'" | sort: "date" | reverse %}
  {% for post in gallery_posts %}
    <li class="gallery-item-card" data-date="{{ post.date | date: '%Y-%m-%d' }}">
      <p class="gallery-title"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></p>
      <p class="gallery-date">{{ post.date | date: "%Y-%m-%d" }}</p>
      {% if post.images and post.images[0] %}
        <a href="{{ site.baseurl }}{{ post.url }}">
          <img src="{{ post.images[0] }}" alt="{{ post.title }}" class="gallery-thumbnail"/>
        </a>
      {% endif %}
    </li>
  {% endfor %}
</ul>

<div id="pagination-nav" class="pagination-nav">
  <div id="page-numbers" class="page-numbers"></div>
  <button id="next-btn" class="pagination-btn">></button>
</div>

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


  .pagination-nav {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 8px;
    margin-top: 40px;
  }

  .page-numbers {
    display: flex;
    gap: 4px;
    align-items: center;
    margin-right: 8px;
  }

  .pagination-btn {
    padding: 6px 10px;
    border: none;
    background: transparent;
    color: #666;
    cursor: pointer;
    transition: color 0.2s ease;
    text-decoration: none;
    min-width: 32px;
    text-align: center;
    font-family: inherit;
    font-size: 14px;
    border-radius: 3px;
  }

  .pagination-btn:hover:not(:disabled) {
    color: #333;
    background: #f8f8f8;
  }

  .pagination-btn:disabled {
    opacity: 0.3;
    cursor: not-allowed;
  }

  .pagination-btn.current {
    background: #333;
    color: white;
  }

  .pagination-btn.current:hover {
    background: #555;
  }

  #next-btn {
    font-size: 16px;
    padding: 6px 8px;
    min-width: 28px;
  }

  .gallery-item-card.hidden {
    display: none;
  }

  @media (max-width: 768px) {
    .pagination-nav {
      gap: 5px;
    }

    .pagination-btn {
      padding: 6px 10px;
      font-size: 0.9em;
      min-width: 35px;
    }
  }
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const itemsPerPage = 9;
  let currentPage = 1;

  const galleryItems = document.querySelectorAll('.gallery-item-card');
  const totalItems = galleryItems.length;
  const totalPages = Math.ceil(totalItems / itemsPerPage);

  const paginationNav = document.getElementById('pagination-nav');
  const nextBtn = document.getElementById('next-btn');
  const pageNumbers = document.getElementById('page-numbers');

  if (totalPages <= 1) {
    paginationNav.style.display = 'none';
    return;
  }

  function showPage(page) {
    currentPage = page;

    galleryItems.forEach(item => {
      item.classList.add('hidden');
    });

    const startIndex = (page - 1) * itemsPerPage;
    const endIndex = Math.min(startIndex + itemsPerPage, totalItems);

    for (let i = startIndex; i < endIndex; i++) {
      galleryItems[i].classList.remove('hidden');
    }

    updatePaginationButtons();
  }


  function updatePaginationButtons() {
    nextBtn.disabled = currentPage === totalPages;

    pageNumbers.innerHTML = '';

    for (let i = 1; i <= totalPages; i++) {
      const pageBtn = document.createElement('button');
      pageBtn.textContent = i;
      pageBtn.className = 'pagination-btn';

      if (i === currentPage) {
        pageBtn.classList.add('current');
      }

      pageBtn.addEventListener('click', () => {
        showPage(i);
      });

      pageNumbers.appendChild(pageBtn);
    }
  }

  nextBtn.addEventListener('click', () => {
    if (currentPage < totalPages) {
      showPage(currentPage + 1);
    }
  });

  showPage(1);
});
</script>