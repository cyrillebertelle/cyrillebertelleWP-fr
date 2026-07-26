---
layout: page
permalink: /teaching/
collection: teaching
title: enseignement
description: liste de mes activitées ci-dessous; cliquer sur chaque item pour plus d'informations
display_categories: [cours récents, archive d'anciens cours]
nav: false
profile:
  align: right
  image: teaching.jpg
  address: >
    <p>   </p>

pagination:
  enabled: true
  collection: teaching
  permalink: /page/:num/
  per_page: 7
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3  # The number of links after the current page
---
<img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/9.jpg' | relative_url }}" alt="" title="example image"/>
Abstract (in progress) 
   <ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p>{{ post.description }}</p>
      </li>
    {% endfor %}
  </ul>
{% include pagination.html %}