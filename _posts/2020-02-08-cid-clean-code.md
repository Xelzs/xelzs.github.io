---
layout: post
title:  "CorrelationID / Optimisation de code"
date:   2020-02-08 12:15:00 +0200
categories: stage madelink
---
Cet article fait parti de la suite d'articles sur le retour de mon expérience au sein du stage alterné que j'ai réalisé chez l'entreprise Madelink présenté sur [cette page]({% link enterprises.md %}).

___


## Optimisation API en Nest.JS

La prochaine mission que j'ai pu effectuer a été de refactoriser et d'améliorer le code crée par un autre développeur.  
M. LEBON me faisant confiance et ayant pu faire mes preuves, il me laissa optimiser le code réalisé en en Node.JS avec le framework Nest.JS dont j'avais déjà utilisé auparavant lors de mon premier stage.  

Le but était principalement de réorganiser le code codé de manière procédurale en programmation orientée objet.  
Ayant pratiqué dans divers langages cette syntaxe je n'ai pas rencontré de problème pour la réalisation de cette tâche.

## CorrelationID

Ma dernière mission traitant du développement back-end consistera en la mise en place d'une gestion complète du CorrelationID à travers l'architecture micro-services que dispose Madelink.  

Jusqu'alors je n'avais jamais entendu parler de "CorrelationID". L'équipe m'a alors expliqué qu'il s'agit d'un identifiant permettant de garder la trace de l'information lors d'une requête.  
Ainsi lorsque qu'un appel à l'api est effectué, un CorrelationID est généré et est transféré via toutes les APIs jusqu'à que la requête soit terminée.

Le CorrelationID était déjà mis en place sur la partie Java mais pas sur la partie Node.JS.  
Après plusieurs jours j'ai pu réussir à mettre en place un début de cette gestion de CorrelationID.  
Début ? Oui seulement, car nous nous sommes rendu compte qu'il était compliqué de gérer cette partie là dans le framework Nest.JS à moins de coder nous même une partie du framework.

## Bilan

Après une optimisation réussie du code en Node.JS, j'ai dû abandonner la partie CorrelationID étant donné la masse de travail et le peu de temps restant avant la fin de mon stage.