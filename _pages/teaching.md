---
layout: page
permalink: /teaching/
collection: teaching
title: teaching
description: Materials for courses you taught
display_categories: [current, past]
nav: true
profile:
  align: right
  image: teaching.jpg
  address: >
    <p>   </p>

pagination:
  enabled: true
  collection: teaching
  permalink: /page/:num/
  per_page: 3
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
<img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/9.jpg' | relative_url }}" alt="" title="example image"/>
Abstract (in progress)
  <ul class="post-list">
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
