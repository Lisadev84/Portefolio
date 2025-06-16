---
title: LisaWalk
publishDate: 2024-08-22 00:00:00
img: /assets/LisaWalk.png
img_alt: Logo du site
description: |
  L'application Lisawalk est dédié à la randonnées, à la proposition d'itinéraires et de téléchargement de traces gpx. 
tags:
  - Analyse de projet
  - HTML5/CSS
  - Bootstrap
  - PHP8
  
---
<p style = "text-align:justify;">
Lisawalk est un projet personnel développé dans le cadre de la soutenance du  titre de Développeur Web et Web mobile. 
Le projet a été initié par étape : analyse du projet, définition du schéma de navigation et de la charte graphique, modélisation de données avec "Merise" et création de la base de données, développement du site et mise en production.

Initialement, l'application permettait à l'utilisateur de s'inscrire et d'avoir accès à une liste de randonnées, détaillée par un descriptif, accompagnées d'une carte de localisation avec la possibilité de télécharger la trace gpx.
Je l'ai amélioré progressivement en y ajoutant des fonctionnalités supplémentaires:

- Amélioration du BackOffice ; 
- réalisation d'un template pour chaque randonnée ; 
- création d'une page profil ;
- Définition d'un statut pour les randonnées et ajout dans le profil utilisateur.
</p>

##### Fonctionalités
Pour l'utilisateur : 
- Inscription / Connexion / Déconnexion / Désinscription
- Consultation des randonnées / Affichage et Téléchargement de traces GPX
- Commentaires / Livre d'or du site
- Gestion du statut des randonnées (A faire, Réalisée)
- Affichage des randonnées sélectionnées sur la page profil

Pour l'administrateur : 
- Gestion des utilisateurs
- Gestion des randonnées
- Gestion des commentaires
- Gestion des messages du livre d'or

##### Stack

- Frontend : HTML, CSS, JavaScript, Figma pour le maquettage
- Framework : Bootstrap5
- Bibliothèque : Leaflet pour les cartes de localisation et traces gpx
- Base de données relationnelle : Mysql / interface graphique : MysqlWorbench
- Backend : PHP8
- FTP : Filezilla
- Hébergement : O2Switch, <a href = "https://www.lisawalk.fr" target="_blank">lien vers le site</a>

Le projet évoluera encore avec le partage de randonnées provenant des utilisateurs, la possibilité d'imprimer la carte itinéraire en pdf... 