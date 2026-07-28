---
layout: page
title: projets
permalink: /projects/
description: 
nav: true
display_categories: [projets récents, projets anciens, dissemination, others]
horizontal: false
---
Liste des projets de recherche auxquels j'ai contribué soit en tant que responsable, soit en tant qu'expert. 

Il s'agit de mettre en place des solutions innovantes, basées sur des travaux de recherche, répondant à des défis ou problèmatiques académiques, souvent pluridisciplinaires, ou encore répondant à des problèmes concrets en partenariat avec des universitaires ou des entreprises.   

Cliquer sur chacun des pavés pour obtenir des informations plus précises sur ces projets.

<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h2 class="category">{{category}}</h2>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <!-- Generate cards for each project -->
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-2">
          {% for project in sorted_projects %}
            {% include projects_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {% for project in sorted_projects %}
            {% include projects.html %}
          {% endfor %}
        </div>
      {% endif %}
    {% endfor %}

  {% else %}
  <!-- Display projects without categories -->
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for project in sorted_projects %}
          {% include projects_hrz.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for project in sorted_projects %}
          {% include projects.html %}
        {% endfor %}
      </div>
    {% endif %}

  {% endif %}

</div>
