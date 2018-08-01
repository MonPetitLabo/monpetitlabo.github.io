---
title: Bienvenue sur le blog du fablab Mon Petit Labo
layout: default
---

## Description du projet

Suivez l'aventure merveilleuse d'un mini fablab entre collègues permettant à chacun de monter en compétence sur la conception, l'électronique et le développement.

## Les dernières nouvelles

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>