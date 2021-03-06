---
layout: post
title:  "Première fonctionnalité en production"
date:   2019-04-30 12:00:00 +0200
categories: stage digikare
---

Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Digikare présenté sur [cette page]({% link enterprises.md %}).

___

## Ils me font confiance !

Pour cette nouvelle mission, je vais développer une nouvelle fonctionnalité qui sera directement disponible aux utilisateurs finaux du produit Orthense de Digikare.  
Cette mission permet de démontrer que l'équipe pense que j'ai suffisamment fait mes preuves et démontré mes compétences pour qu'ils puissent me faire confiance et me donner du travail d'une plus grande importance.

## La fonctionnalité

L'application Orthense avait besoin d'une nouvelle fonctionnalité permettant aux différents chirurgiens de partager des "screens" (capture d'écran) de leur tableau de bord sans risquer de compromettre les données auxquelles ils ont accès. Ainsi il fallait développer un mode "discret", permettant de remplacer toutes données sensibles par des croix (ex: Paul => XXXXX).  
Pour cela j'ai donc cherché dans l'application tous les emplacements de données sensibles et j'y ai appliqué mon pipe Angular permettant cette transformation.  
La fonctionnalité devait également être activable d'un simple clic de l'utilisateur, le choix de la position du bouton s'est donc porté dans la toolbar présente sur chacune des pages de l'application.

## Le résultat

Au bout d'1 semaine et demie de développement, cette fonctionnalité a donc été correctement intégrée et l'équipe de Digikare a accepté sa mise en place en production après un "code review".  
C'est donc la semaine du 15 mai 2019 que ma première "vraie" fonctionnalité a été incorporé dans un outil utilisé par une clientèle et donc directement en production.

## Bilan

Cette mission m'a apporté la satisfaction et le plaisir de développer pour des utilisateurs finaux tels que les chirurgiens d'Orthense.  
La reconnaissance d'autres développeurs, même à titre modeste, m'a conforté dans cette motivation à développer à leur côté.  
Pour la prochaine étape de mon stage, je vais réaliser une extraction de composant Angular en code HTML/CSS/JavaScript.