---
title: Propri'Opti
publishDate: 2024-08-21 00:00:00
img: /assets/logo-propriopti.png
img_alt: Logo de l'application
description: |
  Propri’Opti est une solution numérique multiplateforme conçue pour moderniser la gestion locative saisonnière des propriétaires de gîtes et chambres d'hôtes. 
tags:
  - Angular
  - Java
  - API
---
##### Version 1 en cours : démarrée dans le cadre de la soutenance du titre de Concepteur Développeur d'applications  
<p style = "text-align:justify;">
L'objectif de Propri’Opti est de fournir un outil complet qui centralise la gestion des réservations, la communication avec les clients et l’automatisation des opérations quotidiennes. En outre, cette application vise à s'intégrer harmonieusement dans l'écosystème numérique actuel des locations saisonnières, en offrant une synchronisation avec les principales plateformes de réservation et un accès facile via différents dispositifs numériques. Propri’Opti se positionne comme un partenaire stratégique pour les propriétaires en leur permettant de se concentrer sur l'amélioration de l'expérience client tout en maximisant leur rentabilité.

Le développement de l'application sera réalisé en 3 versions sucessives. L'application proposera des modules de fonctionnalités aux utilisateurs. 
</p>

##### Organisation du projet :    
- Analyse des besoins ;
- Elaboration du cahier des charges ;
- Etude de l'architecture  et choix des technologies
- Modélisation des données (Merise et UML)
- Maquettage du projet ; 
- Sécurité de l'application et des données ;
- Gestion de projet / Plan d'organisation du projet de développement ; 
- Développement de l'application et création de la base de données;

##### Fonctionnalités pour les propriétaires :  
- Module n°1 : Module de base
- Module n°2 : Module n°1 + Module Organisation des tâches et Mail
- Module n°3 : Module n°1 et n°2 + Module Channel Manager
- Module n°4 : Module n°1, n°2, n°3 + Module Gestion commerciale et comptable
- Module n°5 : Module de Génération de site Web

La version 1 se concentre sur le développement des fonctionnalités de base :   
- **Accueil** : Page initiale (landing page) offrant un aperçu global de l’application avec un descriptif des fonctionnalités par module et un accès rapide aux différentes sections de l'application.
Cette page proposera également à l’utilisateur un essai de l’application. Un bouton « Démonstration » permettra de découvrir l’application et de la tester.  
- **Inscription/Connexion**: Système d'inscription pour de nouveaux utilisateurs et de connexion pour les utilisateurs existants.  
Contact : Formulaire de contact pour les visiteurs et les requêtes générales.
- **Dashboard Administrateur :** Panneau de contrôle présentant les indicateurs clés utiles à l’administrateur (rendez-vous, relances clients, modules les plus représentatifs…). Il donnera accès à la gestion des prospections, des modules, des clients et à une messagerie qui sera développé sur la version 2. Un menu et un pied de page spécifiques seront dédiés à la partie administrateur.  
- **Dashboard des Propriétaires :** Panneau de contrôle présentant les indicateurs clés de performance, les réservations récentes et l'activité en cours (check in, check out, suivi clientèle). Il s’étoffera au fur et à mesure du développement d’autres fonctionnalités dans les versions suivantes. Il donnera accès au menu de l’application de gestion locative.   
- **Paramétrages de l’activité :** Cette section permettra à l’utilisateur de configurer les aspects spécifiques de l’activité locative comme les hébergements à la location, les prestations, les tarifs et les disponibilités.  
- **Gestion des réservations :** Module pour créer, modifier et visualiser les réservations actuelles et historiques. La page Gestion des réservations affichera un calendrier aux vue mensuelles, semestrielles ou annuelle au choix. Un clic sur une date proposera un formulaire de réservation. L’état des réservations permettra de suivre l’avancée de la réservation et son changement de statut (de pré-réservation à clôture). La validation du formulaire créera une fiche client qui pourra être compléter par son profil et préférence.  
- **Cardex clients :** Espace dédié à la gestion des informations des clients, de leur profil et préférences ainsi que de l'historique de réservation.


##### Stack :
- Couche Web : Angular / Typescript / Tailwind ; 
- Android : Environnement de développement Android Studio / Java ; 
- couche métier : JAVA / Spingboot
- server : Tomcat
- Conteneurisation : Docker
- Base de données : Serveur Mysql / interface graphique Mysql Workbench
- ApiRestfull :  Postman et Swagger UI 
- Versionning / Tests : Git / Gitlab
- <a href = "https://gitlab.com/Lisadev/proprioptibev1" target="_blank">lien vers gitlab</a> (back)
- <a href = "https://gitlab.com/Lisadev/proprioptifev1" target="_blank">lien vers gitlab</a> (front)
