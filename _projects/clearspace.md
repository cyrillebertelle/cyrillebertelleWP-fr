---
layout: page
title: Clearspace
description: Projet collaboratif soutenu par la Région Normandie 
img: /assets/img/clearspace-v2.png
importance: 8
category: projets récents
---
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/clearspace-v2.png' | relative_url }}" alt="" title="assaillant logo"/>
    </div>
</div>
<!-- 
<div class="caption">
    FuMa logo
</div>
-->

### Clearspace : Solution globale constituant des preuves juridiques de survols illégaux de drones

**Financeur** :
Union Européenne et Région Normandie  
**Montant total du financement** :
95 000€ (38 000€ région /57 000€ FEDER)  
**Période de réalisation** :
01/11/2022 – 31/12/2025 (24 mois)   
**Responsable scientifique pour l'Université Le Havre Normandie** : 
Claude Duvallet   

#### Partenaires 
* LITIS – Laboratoire d’Informatique, du Traitement de l’Information et des Systèmes (ULHN)
* XTR Drones 
* Cegelec Defense


#### Descriptif du projet  
Le projet ClearSpace a été mené par le LITIS pour l’Université Le Havre Normandie, en collaboration avec les sociétés XTR Drones et Cegelec Défense. Il avait pour objectif d’explorer l’utilisation de la technologie blockchain pour certifier et préserver l’intégrité des preuves associées à la détection d’intrusions de drones dans des zones surveillées.

Dans ce cadre, les partenaires industriels XTR Drones et Cegelec Défense ont développé une solution technique permettant de détecter la présence de drones dans une zone donnée et de collecter un ensemble d’informations relatives à ces événements. Ces informations incluent notamment les coordonnées géographiques de la détection, la date et l’heure de l’événement ainsi que des photographies ou autres éléments visuels permettant de documenter l’intrusion. L’un des enjeux majeurs du projet consistait à garantir l’intégrité, la traçabilité et l’horodatage fiable de ces données afin de pouvoir démontrer qu’elles n’avaient pas été modifiées ou altérées après leur collecte, en particulier dans des contextes où elles pourraient être utilisées comme éléments de preuve.

La technologie blockchain constitue une solution particulièrement adaptée à ce besoin. En effet, une blockchain repose sur un registre distribué, partagé entre plusieurs nœuds du réseau, dans lequel les informations enregistrées sont horodatées et rendues immuables grâce à l’utilisation de mécanismes cryptographiques et de chaînage des blocs. Une fois une donnée inscrite dans la blockchain, il devient extrêmement difficile de la modifier sans que cela soit détectable, ce qui permet de garantir l’intégrité et la traçabilité des informations dans le temps.

Le LITIS est intervenu en apportant son expertise dans le domaine des technologies blockchain afin de concevoir et de mettre en œuvre un mécanisme d’ancrage des données dans une blockchain, dans le cadre d’une preuve de concept. Plutôt que d’enregistrer directement l’ensemble des données dans la blockchain, ce qui serait coûteux et peu adapté aux volumes importants générés par les images, l’architecture retenue repose sur l’inscription dans la blockchain des seules empreintes cryptographiques (hash) des données. Les fichiers volumineux, tels que les photographies, sont ainsi conservés hors de la blockchain, tandis que leur empreinte numérique, immuable, est enregistrée dans la chaîne de blocs. Ce mécanisme permet de vérifier ultérieurement l’intégrité des données en comparant leur empreinte recalculée avec celle inscrite dans la blockchain.

Afin de faciliter l’intégration de ce mécanisme dans les systèmes développés par les partenaires industriels, le LITIS a également conçu et déployé un ensemble d’API permettant d’interagir avec la blockchain. Ces interfaces permettent aux partenaires d’ancrer indirectement les preuves de détection d’intrusions en soumettant les empreintes des données collectées au système d’ancrage. Cette approche rend l’utilisation de la blockchain transparente pour les applications métier tout en garantissant la traçabilité, l’intégrité et l’horodatage fiable des informations enregistrées.

<img src="/assets/img/fig3-clearspace.png" width="700"/>

<img src="/assets/img/AntenneClearSpace.png" width="450"/>

<img src="/assets/img/fig2-clearspace.png" width="700"/>

<img src="/assets/img/fig4-clearspace.png" width="700"/>

<img src="/assets/img/fig1-clearspace.png" width="700"/>



