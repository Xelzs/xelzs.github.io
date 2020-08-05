---
layout: post
title:  "Système de logging"
date:   2020-01-19 18:30:00 +0200
categories: stage madelink
---
Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Madelink présenté sur [cette page]({% link enterprises.md %}).

___


## Introduction

Pour cette première semaine au sein de Madelink, j'ai pu rencontrer l'équipe technique réalisant la solution informatique d'e-learning.  
Etant intéressé par les différents aspects de l'informatique que sont l'infrastructure et le développement web, j'ai découvert ainsi l'étendu des solutions mises en oeuvre pour réaliser cette plateforme et me rendre compte des différentes technologies nécessaire à son bon fonctionnement.

## L'infrastructure

Afin d'être rapidement opérationnel et utile à la société, j'ai appris l'une des technologies qu'ils utilisent, openshift.  
Cet outil crée par Red Hat m'étais jusqu'alors totalement inconnu. 
Avec cet outil j'ai appris une nouvelle notion : les images S2I (Source-to-Image).  
Puis en poursuivant "l'état des lieux" de son infrastructure, M. LEBON (Maître de stage), a soulevé un problème grandissant au sein de son infrastructure : le manque d'espace disque.  

## Bilan / Premier objectif

Après cette première semaine à découvrir l'infrastructure et suite à l'apprentissage de nouvelles notions telles qu'OpenShift et les images S2I, ma première mission au sein de l'entreprise s'est dessiné : trouver une solution au problème d'espace disque.  