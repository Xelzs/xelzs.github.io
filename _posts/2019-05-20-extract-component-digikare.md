---
layout: post
title:  "Extraction de composants Angular"
date:   2019-05-20 19:00:00 +0200
categories: stage digikare
---

Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Digikare présenté sur [cette page]({% link enterprises.md %}).

___

## La mission

Ces trois dernières semaines, ma mission était donc d'extraire la fonctionnalité de connexion de 2 applications en production (toutes deux de la solution Orthense).  
En effet, afin de résoudre des problèmes de compatibilité entre navigateur et de chargement de page plus rapide, la fonctionnalité de connexion devait être recodé en HTML / CSS / JavaScript.

## Les principales fonctionnalités

Il fallait reproduire le design de la page de connexion exact, généré à l'aide de framework comme Angular Material. Puis il fallait appeler la librairie OIDC afin de faire appel au service d'authentification correspondant.  
Un système de traduction devait également être mis en place sur la page de connexion, étant donné qu'un service s'occupait de faire la traduction dans toute l'application Angular.  
Enfin, il fallait réaliser une détection de navigateur accédant à cette page, et s'il n'est pas dans la liste des navigateurs compatibles à l'application, l'indiquer sur la page et désactivé le système d'authentification.

## Difficultés

La plus grosse difficulté que j'ai rencontré lors de la réalisation de cette application fût de mettre en place la compatibilité avec Internet Explorer 11 et donc de devoir développer du code avec d'anciens standards (pas d'ES6/7).  
La seconde difficulté fût de mettre en place le service de traduction. Dans un premier temps j'avais utilisé un plugin jQuery, cependant l'équipe me l'ayant fait remarquer, charger jQuery seulement pour la traduction n'était pas nécessaire. J'ai donc dû réaliser mon propre code et le charger via un fichier javascript (appel au JSON étant non pris en charge par IE11).

## Bilan

Cette mission fût enrichissante car elle m'a permis d'être confronté à des contraintes de compatibilité sur de vieux navigateurs web.  
De plus, j'ai pu voir la difficulté d'extraire et de mettre en place soit même un code généré à l'aide de framework tel qu'Angular.  
Ma prochaine mission sera un gros chantier sur cette même application, et donc également un développement qui ira à termes en production. 