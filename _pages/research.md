---
layout: page
permalink: /research/
collection: research
title: research
description: research activities and animation
display_categories: [current, past]
nav: true
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
<!-- <div class="post"> -->
<!--  <div class="header-bar">
    <h1>Teaching</h1>
    <h2>Material for courses</h2>
  </div>
-->
Abstract (in progress)

  <ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
        <p>{{ post.description }}</p>
      </li>
    {% endfor %}
  </ul>

  {% include pagination.html %}

<!-- </div> -->