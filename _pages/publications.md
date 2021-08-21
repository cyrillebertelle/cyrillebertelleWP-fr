---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, 1999, 1998, 1997, 1996, 1995, 1994, 1993, 1992, 1991, 1990, 1989, 1988, 1987]
nav: true
---

Une grande partie de mes publications sont accessibles :
* [depuis mon dépôt Hal](https://haltools.archives-ouvertes.fr/Public/afficheRequetePubli.php?auteur_exp=cyrille+bertelle&CB_auteur=oui&CB_titre=oui&CB_article=oui&langue=Anglais&tri_exp=annee_publi&tri_exp2=typdoc&tri_exp3=date_publi&ordre_aff=TA&Fen=Aff&css=../css/VisuRubriqueEncadre.css)
* ou [depuis ma Google Scholar page](https://scholar.google.com/citations?user=Twj3qDQAAAAJ&hl=fr)

Ci-dessous, ma liste de mes publications par années et par catégories, générée par jekyll-scholar. Elle contient 250 références dont 7 livres, 14 publications de proceedings ou de numéros spéciaux de revues, 24 chapitres de livres, 48 articles de revues scientifiques, 148 communications dans des conférences (à la fin Août 2021).

<div class="publications">
 
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
