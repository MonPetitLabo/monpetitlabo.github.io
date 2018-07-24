---
title: Hello
layout: default
---
 
Bienvenue sur le blog du fablab Mon Petit Labo !

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
