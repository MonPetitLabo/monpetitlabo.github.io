---
title: Test du capteur de ligne
date:  2018-07-23 12:30:00 +0200
post_description: Durant cette séance, nous avons testé un capteur de contraste IR.
---

Afin de pouvoir suivre une ligne, il est nécessaire que notre robot puisse la voir. Nous avons donc cherché un capteur de contraste permettant de détecter cette ligne et nous sommes tombés sur celui-ci :

[https://www.lextronic.fr/capteurs-infrarouge/29999-capteur-suiveur-de-ligne-lineaire.html](https://www.lextronic.fr/capteurs-infrarouge/29999-capteur-suiveur-de-ligne-lineaire.html)

Après l'avoir reçu, il est temps de le tester. Une breadboard, un arduino et c'est parti pour récupérer les retours du capteurs sur une des entrées analogiques de la carte Arduino.

Le capteur est composé de 3 diodes IR ainsi que de 3 capteurs infrarouges. Cela permet de détecter de quel côté de la ligne le robot déviera et ainsi pouvoir corriger sa trajectoire.

Les résultats ne sont pas probants, nous n'arrivons pas à avoir de vraies différences de retour quand nous plaçons le capteur devant un support clair  puis devant un support foncé.

Il reste encore à étudier ce capteur plus en profondeur et voir s'il est possible de le calibrer ou si un autre positionnement peut améliorer le retour.