---
title: Bienvenue sur le blog du fablab Mon Petit Labo
---

## Description du projet

Suivez l'aventure merveilleuse d'un mini fablab entre collègues permettant à chacun de monter en compétence sur la conception, l'électronique et le développement.

## Les dernières nouvelles

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date | date: "%d/%m/%Y" }} - {{ post.title }}</a>
      <p>{{ post.post_description }}</p>
    </li>
  {% endfor %}
</ul>