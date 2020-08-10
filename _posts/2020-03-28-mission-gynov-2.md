---
layout: post
title:  "Mission : Réaliser un site de gestion de ressources matérielles (2/2)"
date:   2020-03-28 15:00:00 +0200
categories: mission gynov
---

Cet article est la suite du premier traitant de ma mission pour Toulouse Ynov Campus.  
Vous pouvez le consulter [ici]({% post_url 2020-03-07-mission-gynov %}).

___ 

## Difficulté

La principale difficulté dans la réalisation de cette mission est d'exprimer de manière simple et intuitive le besoin du client.  
Cette une des priorités imposées par le client.  

## Design

Concernant le design du site, je me suis inspiré du design du site de réservation de la salle de coworking pour lequel j'ai également était son créateur.  
Ainsi, les guidelines d'Ynov sont bien respectées en reprenant leur design tout en y ajoutant ma "touche personnelle".

Le principal étant la partie "réservation" du site où tout étudiant pourra y accéder, je me suis concentré sur cette partie en premier.  

## Réservation

J'ai porté mon choix sur la génération d'un calendrier mois par mois. Dès que l'on clique sur un jour on peut voir apparaître une modal dans laquelle une liste des horaires disponibles est affichée de 8h à 19h par tranche de 30 min.  
Une fois la tranche sélectionner le système nous redirige vers une autre page de réservation complète avec la tranche horaire pré-remplie (voir screens ci-dessous).

![home_screen](/assets/images/gynov-home.png){:class="big-img"}

![horaires](/assets/images/gynov-horaires.png){:class="big-img"}

![reservation](/assets/images/gynov-reservation.png){:class="big-img"}

Sur cette page nous pouvons voir une liste de matériel avec sa disponibilité pour la tranche horaire et le jour sélectionné.
Une fois sa liste constituée, le matériel est réservé !  
Il est toujours possible de revenir sur sa réservation pour la modifier ou l'éditer.

## Autres parties

Il y a 3 autres parties seulement visible par le staff et les administrateurs (= directeurs).  
La première est la liste du matériel avec la possibilié d'en ajouter, de signaler un problème, d'éditer et supprimer un matériel.  
La seconde est la liste des membres avec possibilité de changer le statut d'un membre (ex: membre => staff) et de consulter les informations rentrés lors de l'inscription.  
Enfin, la dernière partie est la liste des réservations avec le matériel réservé pour chaque réservation.

## Bilan

Après plusieurs jours de travail, je suis fier du résultat du site. J'ai effectué une présentation aux 2 directeurs de Toulouse Ynov Campus qui sont ravis du résultat.  
Cependant, souhaitant que cette application s'exporte vers les autres campus également, nous sommes en attente de validation par la DSI d'Ynov qui doit m'indiquer les éventuels changements à effectuer pour être conforme aux normes d'Ynov.  

Dès lors qu'il sera conforme, il sera intégré chez le client et mis à disposition des élèves.

