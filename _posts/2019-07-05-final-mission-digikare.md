---
layout: post
title:  "Dernière mission chez Digikare"
date:   2019-07-05 12:43:19 +0200
categories: stage digikare
---

Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Digikare présenté sur [cette page]({% link enterprises.md %}).

___

## La dernière mission

Pour ces 2 dernières semaines et suite à ma "grosse" mission de suppression d'un framework, j'obtiens donc 2 composants à repenser.  
Le premier est un tableau où une donnée est manquante et il faut pouvoir la faire "remonter" de l'API afin de l'afficher sur l'interface de l'utilisateur.  
La difficulté est donc de parcourir l'API Node.JS de cette application, de s'y familiariser et d'ajouter la fonctionnalité.  
De plus, une réorganisation des colonnes et des diverses tailles affectées à ces colonnes a dû être mise en place.

## Une dernière fonctionnalité

Le second composant est donc une fonctionnalité à réimplémenter. En effet une timeline permettant de visualiser différentes informations est disponible sur l'application Orthense, cependant lorsque le nombre d'informations est trop grand, la vue mobile se retrouve "entassée" et on ne peux plus visualiser les informations essentielles.  
Pour ce faire, j'ai détourné (suite à l'idée de M. Guérot) l'utilisation des mat-tabs d'Angular Material pour en réaliser une timeline. Ainsi des modifications au niveau du style ont été effectuées et la vue sur mobile a pu être rétablie.

## Bilan

Ces 2 fonctionnalités m'ont servi une nouvelle fois à approfrondir ma pratique d'Angular et m'ont aidé à mettre en place une certaine rigueur syntaxique au niveau du code JavaScript / TypeScript réalisé.  
Mon dernier article à propos de ce stage réalisé au sein de Digikare traitera de mon bilan de stage.