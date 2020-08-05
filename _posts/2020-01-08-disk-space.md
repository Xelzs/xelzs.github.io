---
layout: post
title:  "Mission : Espace disque"
date:   2020-01-08 14:00:00 +0200
categories: stage madelink
---
Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Madelink présenté sur [cette page]({% link enterprises.md %}).

___


## Définition du problème

La première étape pour déterminer comment résoudre ce problème était tout d'abord de bien le définir.  
Chez Madelink, le principe des images S2I est utilisé ce qui implique que 2 types d'images Docker sont nécessaires au bon fonctionnement des différents services.  
Ayant déjà pratiqué lors de projets personnels Docker, j'avais déjà une première approche et idée de son fonctionnement.  
Je me suis documenté sur la solution OpenShift et j'ai compris que le premier type d'image servait à créer des images de "build", puis ces images servait de base pour toutes les autres images Docker contenant les différents services.  

## Recherche de la solution

Une fois le problème bien défini, je pouvais maintenant rechercher quelles solutions s'offraient à moi.  
Etant donné que la plupart des services étaient basé sur 3 images principales, pour moi, il fallait les optimiser.  

## Mise en oeuvre

Je me suis rendu compte que ces 3 images étaient toutes basées sur CentOS, le système d'exploitation créé également par Red Hat. Logique étant donné que la solution OpenShift utilisé provenait d'eux.  
Cependant CentOS est un OS assez lourd en terme d'espace disque comparé à d'autres existants sur le marché.  

Par mon expérience je connaissais déjà l'OS Alpine, connu pour faire parti des plus léger.  
J'ai donc décider, suite à l'accord de M. LEBON, de récrire les images de build.  
Après plus de 2 semaines de boulot j'ai réussi à recréer le comportement de chaque image sous CentOS dans Alpine OS. J'ai rencontré quelques difficultés car les 2 systèmes d'exploitation n'utilisent pas les mêmes bases et donc pas les mêmes dépendances.

## Bilan

Suite à l'optimisation de ces images, je suis fier du résultat obtenu, car seulement pour les 3 images de build j'ai économisé en moyenne 250 Mo ce qui permettra par la suite d'optimiser tous les services de chez Madelink.