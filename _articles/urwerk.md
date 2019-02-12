---
title: project » urwerk - EMC
description: >-
  Découvrez ce magnifique projet de la haute Horlogerie qui a reçu le prix de
  l'innovation du GPHG en 2014
class: building
order: 1
image: /assets/images/urwerk-emc2.jpg
tags: <span>eagle pcb</span> <span>c/c++</span> <span>AVR</span> <span>watchmaker</span>
published: true
---

## EMC 1, EMC 2
Dans le cadre de ce projet, nous avons développé l'électronique et le logiciel d’une montre mécanique équipée d’un « microcontroller », permettant de mesurer la précision du mouvement (mesure avec une précision de minimum 10 microsecondes). Le «CPU» est alimenté par un supercondensateur qui se charge avec l'aide d'une manivelle. Pas d'obsolescence de la batterie avec cette limite de 1000 charges. Avec un supercondensateur la limite de charge est inexistante! (**EMC1, prix de l'innovation du GPHG en 2014**)


![urwerk 1](/assets/images/urwerk-emc-dev1.jpg){: .full-width}


## L'électronique n'est pas un problème !
* :boom: Création des schémas électroniques  
  * étage d'énergie qui doit fonctionner avec une source qui varie de 0.7 à 2.8 [V] (contrainte des supercapacitors) pour ensuite l'élever de manière stable à 3.0 [V]
  * étage d'affichage (moteur et LED)
  * étage CPU (microcontrolleur AVR)
  * étage de programmation des boards
* :boom: Analyse de maximisation de l'énergie sans compromettre la précision de la mesure
* :boom: Sélection des meilleurs composants électroniques
* :boom: Développement du logiciel pour effectuer une mesure et piloter l'affichage

![urwerk 2](/assets/images/urwerk-emc3.jpg)

* :boom: Production d'un kit de montage et de programmation rapide des boards
![urwerk 2](/assets/images/urwerk-emc4.jpg)


