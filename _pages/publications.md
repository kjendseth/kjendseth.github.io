---
layout: page
permalink: /publications/
title: publications
description: Complete list pulled from Google Scholar (auto-sorted newest first).
nav: true
nav_order: 2
---

{% assign pubs = site.data.publications %}

<div class="publications">
  {% for pub in pubs %}
  <div class="card border-0 shadow-sm mb-3">
    <div class="card-body">
      <h3 class="card-title h5 mb-1">
        {% if pub.link %}
          <a href="{{ pub.link }}" target="_blank" rel="noopener">{{ pub.title }}</a>
        {% else %}
          {{ pub.title }}
        {% endif %}
      </h3>
      <p class="text-muted mb-1">{{ pub.authors }}</p>
      <p class="mb-0">
        {{ pub.venue }}
        {% if pub.year %}
          <span class="text-muted">&middot; {{ pub.year }}</span>
        {% endif %}
      </p>
    </div>
  </div>
  {% endfor %}
</div>
