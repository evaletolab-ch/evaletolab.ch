---
title: SIB - nextprot.org
description: Une base de données RDF centrée sur les protéines humaines, le génome, les maladies, les publications, etc. 
class: best-practices
order: 1
image: /assets/images/graph-1.jpg
tags: <span>RDF</span> <span>noSQL</span> <span>AngularJS</span> <span>java-spring</span> <span>github</span>
---
## Réalisation
La base de données de neXtProt était principalement en SQL *[Postgres]* et la recherche de son contenu reposait à 100% sur l'utilisation de l'algorithme [TF-IDF](https://fr.wikipedia.org/wiki/TF-IDF) (SolR). Le problème est qu'il s'est révélé impossible d'effectuer des recherches croisées entre différentes relations de données: 
> Avec SolR, la relation [graph] entre les données est trop simple, et ce n'est pas possible de résoudre une question du genre **«les personnes qui habitent Genève, qui ont un chien brun qui aboie quand il neige»** :unamused:! Également, SQL fonctionne sur une normalisation des données ce qui le rend inutilisable sans une couche de services dédiée pour chaque usecase!

Olivier Evalet a été impliqué dans ce projet pour remplacer le moteur de recherche ​ TF-IDF​ (de SolR) de neXtProt​ la plateforme de connaissances en ligne sur les protéines humaines.

* Proposer une solution technique pour répondre aux recherches suivantes :
  * `Proteins phosphorylated and located in the cytoplasm,`
  * `Proteins with 7 transmembrane regions`
  * `Proteins whose genes are on chromosome 13 and are associated with a disease`
  * [liste complète des recherches](https://snorql.nextprot.org)
* Étude des bases de données orientées [Graphe](https://fr.wikipedia.org/wiki/Base_de_donn%C3%A9es_orient%C3%A9e_graphe)
* Modélisation d'un graphe de données [RDF] sur la base du schéma normalisé SQL
* Implémentation des outils d'exports SQL *(dénormalisation)* en assertions au format `(sujet, prédicat, objet)`
* Implémentation et mesures de performance sur différents triplestores :**virtuoso, fuseki et bigdata**
* Implémentation d'un front-end pratique pour tester les recherches [snorql.nextprot.org](https://snorql.nextprot.org/)
* Design et implémentation du front-end de la v1

## Nextprot, a human protein database
neXtProt est une plateforme de connaissances en ligne sur les protéines humaines. neXtProt s’efforce d’être une ressource complète fournissant une variété d’informations sur les protéines humaines, telles que leur fonction, leur localisation sous-cellulaire, leur expression, leurs interactions et leur rôle dans les maladies. La majeure partie des informations contenues dans neXtProt provient de la base de données UniProt Swiss-Prot, mais elle est complétée par des données provenant d'études à haut débit mettant l'accent sur la protéomique. neXtProt offre également une capacité de recherche avancée basée sur la technologie *SPARQL* ainsi qu'une *API* permettant d'extraire par programme les données stockées dans la ressource. Il est développé par le groupe CALIPHO dirigé par Amos Bairoch et Lydie Lane de l'Institut suisse de bioinformatique (SIB).


* [snorql.nextprot.org](https://snorql.nextprot.org/)
* [nextprot.org/proteins/search?query=MSH6](https://www.nextprot.org/proteins/search?query=MSH6)
* [github.com/calipho-sib/](https://github.com/calipho-sib/)

![np-v1](/assets/images/nextprot-web-filters.jpg){: .full-width.border}
Exemple d'un des tout premier design effectué pour la v1 (basée sur SolR et Postgres)

