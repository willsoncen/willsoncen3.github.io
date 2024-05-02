---
layout: default
title: Publications
permalink: /publications/
---

<h1>{{ page.title }}</h1>

<ul class="publications-list">
  {% for publication in site.data.publications %}
    <li>
      <span class="publication-title">{{ publication.title }}</span>
      <span class="publication-authors">{{ publication.authors | join: ', ' }}</span>
      <span class="publication-year">{{ publication.year }}</span>
      <span class="publication-venue">{{ publication.venue }}</span>
      <a href="{{ publication.url }}" class="publication-link">Link</a>
      <p class="publication-excerpt">{{ publication.excerpt }}</p>
    </li>
  {% endfor %}
</ul>