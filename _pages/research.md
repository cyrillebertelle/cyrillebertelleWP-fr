---
layout: page
permalink: /research/
collection: research
title: recherche
description: list de mes activités ci-dessous ; cliquer sur chaque item pour plus d'information
nav: true
profile:
  align: right
  image: research.jpg
  address: >
    <p>   </p>

pagination:
  enabled: true
  collection: research
  permalink: /page/:num/
  per_page: 8
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3  # The number of links after the current page
---

Résumé à faire 

<div class="post"> 
  <div class="header-bar">
    <!-- <h1>Teaching</h1>
    <h2>Material for courses</h2> -->
    Abstract (in progress)
  </div>

  Abstract (soon available)
  
  <ul class="post-list">
    Abstract in progress<br>
    {% for post in paginator.posts %}
      <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <!-- <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p> -->
        <p>{{ post.description }}</p>
      </li>
    {% endfor %}
  </ul>

  {% include pagination.html %}

<!-- </div> -->
