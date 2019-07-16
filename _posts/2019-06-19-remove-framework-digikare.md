---
layout: post
title:  "Suppression d'un framework d'une application existante"
date:   2019-06-19 20:15:03 +0200
categories: stage digikare
---

Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Digikare présenté sur [cette page]({% link enterprises.md %}).

___

## Toujours en production !

Ma prochaine mission, bien que conséquente, portera toujours sur le produit Orthense.  
Les modifications apportées seront donc répercutées sur le client après un "code review" de l'équipe de Digikare.  
Ainsi, suite au succès de ma précédente mission sur ce même produit, Digikare me font confiance pour développer de plus grandes fonctionnalités.

## La mission

Orthense était basé jusqu'à aujourd'hui sur le framework Covalent. Seulement, au fil des versions, Angular Material (utilisé par Covalent) s'est montré de plus en plus complet.  
Ma mission est donc de supprimer totalement le framework Covalent de l'application Orthense, et de remplacer si nécessaire, par Angular Material.  

Cette mission a pour but principal de réduire la taille finale de l'application, tout en gardant ses différentes fonctionnalités sans en impacter l'utilisateur. Ainsi il a fallu reproduire différents composant et comportement de Covalent, en recréant mes propres composants / pipes / services / etc...

## Les difficultés

La principale difficulté a été de bien cerner les différentes utilisations de Covalent dans l'application Orthense.  
En effet, le framework était utilisé dans les fichiers SASS pour le style et mixins pré-défini, le composant de Loading était chargé sur de nombreuses pages, des pipes pour formater les nombres, un menu et bien d'autres emplacements où Covalent était présent.  

De plus, il fallait arriver à reproduire le comportement de ces composants, par exemple le module de chargement faisais apparaître un overlay sur toute la page et ses fonctionnalités étaient accessibles via un service.

Enfin étant donné la taille conséquente du framework, cette mission fût longue à traiter (délai d'environ 1 mois).

## Bilan

La difficulté de supprimer un framework d'une application a été surmonté. Malheureusement arrivant à la fin proche de mon stage, je ne pourrai pas assister au "code review" organisé par l'équipe. Cependant j'ai obtenu l'avis de mon maître de stage qui était satisfait de mon travail et m'a indiqué que ces modifications ne tarderaient pas à être implémenté en production.
Pour ma dernière mission avant la fin de ce stage, je vais effectuer une refonte de 2 fonctionnalités de l'application Orthense.