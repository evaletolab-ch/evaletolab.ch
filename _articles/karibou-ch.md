---
title: karibou.ch
description: Karibou.ch est une place de marché décentralisée spécialisée dans la distribution en flux tendu de produits alimentaires à Genève
class: best-practices
order: 1
image: /assets/images/k.ch/k2.jpg
tags: <span>mongodb</span> <span>travis-ci</span> <span>Angular7</span> <span>node/express</span> <span>github</span>
---


Karibou.ch est une place de marché décentralisée spécialisée dans la distribution en flux tendu de produits alimentaires à Genève.
Son horizon c’est de créer un réseau social dont le but est de simplifier — depuis n’importe ou — l’accès à l’alimentation artisanale et celle de proximité ! Si les GAFA n’ont pas encore “réglés” ce problème avec un un gros DONE, c’est principalement parce qu’il n’y a pas de recette simple. Mais karibou.ch avec son expérience et ses logiciels, apporte un début de solution qui pourrait changer le monde de la distribution alimentaire de proximité.

>En effet, où que vous soyez, vous verrez apparaître sur votre écran les communautés de paysans, d’artisans, de cavistes et d’épiciers qui s’engagent à vous servir la meilleure nourriture en dépôt collecte ou à votre porte. En attendant, Karibou.ch c’est une première communauté de vendeurs à Genève qui offre une réelle alternative au supermarché. Notre première mission est de fournir :

## :boom: Un super logiciel pour le client 
![le client](/assets/images/k.ch/client.png){: .full-width}
karibou.ch a fait peau neuve et est passé de angular-js à angular-7. Une petite note technique [en résumé] car c’est du grand Art, 
* **1]** utilisation de Angular 7, 
* **2]** super modulaire (Lazy loading), 
* **3]** compilation AoT (qui remplace le système de template basé sur la compilation en runtime)
* **4]** décollage de PWA — *[pas à 100% car il y a encore des :bug: :shit: de compatibilité sur certains téléphones*. 
* **5]** capture des erreurs avec [sentry.io](sentry.io) 
* **6]** capture de l’entonnoir des ventes — *“funnel reports” basés sur le retour de comm et l’activité des users* — mais je détaillerais tout ça dans un article dédié.

## :boom: Un super logiciel pour les vendeurs et la logistique,
![les vendeurs et la logistique](/assets/images/k.ch/admin.jpg){: .full-width}

Les livraisons sont planifiées à l'avance par l'équipe logistique. Une fois les commandes organisées, les artisans voient l'ordre de préparation selon les besoins de la logistique. Ensuite les artisans préparent les commandes de leurs clients et peuvent communiquer avec eux si besoin.

## :boom: Un super d'entonnoir des ventes,
![funnel](/assets/images/k.ch/funnel.png){: .full-width}


## Objectifs réalisés:

* :+1: plus de 50% de l’activité Internet provient d’un mobile, cette nouvelle version est super efficace sur presque tous les * smartphones **— attention version du navigateur ≥2015**.
* :+1: l’application est maintenant international (i18n).
* :+1: La navigation a été repensée en partant cette fois du mobile.
* :+1: La sélection des produits est effectuée par un algorithme (une variante du TF-IDF) qui calcul un score selon l’état du produit, votre activité et celle des autres membres.
* :+1: En haut de l’application il y a un espace de présentation de notre sélection.
* :+1: Le client est sollicité pour faire un «feedback positif ou négatif (🌟🌟🌟)» sur ces commandes: «C’est super simple, au moindre souci avec un produit, le client est remboursé»
* :+1: Dès maintenant le client peut choisir de collecter sa commande et ainsi éviter les frais de livraison.

<aside markdown="1" class="pquote hide">
  <img src="https://ucarecdn.com/5b03bb17-e6e5-453c-9152-e92c8c9053ca/-/resize/200x/delp.jpg" class="pquote-avatar" alt="avatar">
  Spécialiste en organisation d'événements et Cofondatrice du club Weetamix, **Delphine Cluzel** est aussi la Co-fondatrice de l'entreprise [karibou.ch](http://karibou.ch). Delphine assure le planning des projets, leur organisation, elle sait se placer à la place de l'utilisateur, elle coordonne les relations publiques et connait bien le marketing social (avec mailchimp et facebook). 


  <p markdown="1" class="pquote-credit">
— @dcluzel, une bonne communication est la clé d'un projet
  </p>
</aside>

<!-- 
![np](/assets/images/karibou.ch-800x768.jpg)

<aside markdown="1" class="pquote">
  <img src="//ucarecdn.com/e79f59da-1081-4c89-a00f-b2499aaf0afa/-/resize/200x/oli.jpg" class="pquote-avatar" alt="avatar">
  Spécialiste des technologies depuis très longtemps, **Olivier Evalet** connait sur le bout des doigts toutes les variantes possibles pour créer une application moderne web ou mobile. Il s'est passioné de l'expérience utilisateur qui est à la base d'une belle création. 
  Cette longue expérience lui permet d'être très efficace pour déterminer le bon déroulement d'un projet.
  
  <p markdown="1" class="pquote-credit">
— @evaletolab, Quoi de plus motivant que de donner à chaque projet les meilleurs outils du moment?
  </p>
</aside>
 -->


