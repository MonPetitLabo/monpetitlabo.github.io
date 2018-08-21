---
title: Le capteur marche !
date:  2018-08-20 12:30:00 +0200
post_description: Après l'avoir soudé, le capteur donne de meilleurs résultats.
images:
  - image_path: /assets/20180820/IMG_20180820_124013.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_125150.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_125207.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_130500.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_130512.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_130519.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_130918.jpg
    title: 20180820_fablab
  - image_path: /assets/20180820/IMG_20180820_130923.jpg
    title: 20180820_fablab
---

Après l'avoir soudé, le capteur donne de meilleurs résultats. La soudure permet d'éviter les faux contacts et nous permet d'obtenir de vrais retours de la part du capteur.

Nous avons donc pu le calibrer sur une ligne de scotch noir et analyser les résultats.

<a data-fancybox href="/assets/20180820/IMG_20180820_125150.jpg"><img src="/assets/20180820/IMG_20180820_125150.jpg" alt="20180820_fablab"/></a>

Le capteur retourne des valeurs de -1000 à +1000 en fonction de sa position par rapport à la ligne :
  - 0 si le capteur est au milieu de la ligne
  - -/+ 1000 si le capteur est sorti de la ligne d'un côté ou de l'autre

En fonction du retour du capteur, nous pourrons piloter les deux moteurs au niveau des roues du robot :
  - Si la ligne part sur la gauche, il faudra arrêter le moteur de la roue droite et continuer de faire tourner la gauche
  - Inversement, si la ligne part sur la droite, il faudra arrêter le moteur de la roue gauche et continuer de faire tourner la droite

Ne pouvant brancher les moteurs directement sur l'arduino sous peine de le griller, nous avons testé la puce "L293D" permettant d'alimenter deux moteurs en gérant également leur sens de rotation (la puce peut également commander plus de 2 moteurs mais ne pourra dans ce cas pas piloter leur sens de rotation).

<a data-fancybox href="/assets/20180820/L293D.jpg"><img class="small_picture" src="/assets/20180820/L293D.jpg" alt="L293D"/></a>

Nous avons utilisé le câblage suivant afin de tester le pilotage d'un moteur puis de 2 :

<a data-fancybox href="/assets/20180820/L293D_schema.jpg"><img src="/assets/20180820/L293D_schema.jpg" alt="L293D"/></a>

Durant la prochaine session, nous pourrons coupler les retours du capteur avec le pilotage des moteurs afin d'avoir un début de système autonome.