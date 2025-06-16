---
title: SaaS en cours - Propri'Opti
publishDate: 2025-06-16
img: /assets/logo-propriopti.png 
img_alt: Logo de l'application
description: |
  Application SaaS de gestion locative tout-en-un dédiée aux propriétaires de gîtes, chambres d’hôtes et locations touristiques.  
  Elle vise à automatiser la gestion quotidienne tout en assurant une cohérence métier et une évolutivité technique.
tags:
   - Java / SpringBoot
   - Angular
   - AWS
---
##### Objectif

Concevoir une plateforme robuste, modulaire et intuitive permettant aux propriétaires de :

* Centraliser leurs réservations
* Générer automatiquement leurs documents légaux (contrats, devis, factures)
* Suivre leurs clients
* Automatiser relances et notifications
* Préparer l’intégration à des plateformes de réservation via Channel Manager



##### Fonctionnalités

* Gestion des réservations (hors OTA)
* Cardex clients (fiche client centralisée)
* Génération automatique de documents : contrat, devis, facture
* Notifications temps réel (rappels, arrivée, solde à facturer…)
* Relances automatisées selon le statut des réservations
* Gestion multi-utilisateurs : admin, abonné, période d’essai, mandataire
* Architecture modulaire : modules activables selon abonnement
* Préparation à l’intégration d’un Channel Manager (Beds24…)



##### Stack technique

**Backend :**
* Java 21 / Spring Boot
* Hibernate (ORM)
* API RESTful

**Frontend :**
* Angular 19
* Tailwind CSS

**Base de données :**
* MySQL 
* Modélisation relationnelle orientée métier 
* UML

**Cloud & DevOps :**
* AWS EC2, S3, RDS, VPC
* Load Balancer, architecture haute disponibilité (multi-AZ)
* Préparation à l’IaC (Infrastructure as Code)

**Qualité & Tests :**
* Tests unitaires et d’intégration (JUnit, Mockito)
* Git / GitHub



##### Défis rencontrés

* Structuration d’une base multi-utilisateurs sans collisions de données
* Conception d’une architecture modulaire avec fonctionnalités activables
* Anticipation des besoins d’intégration avec des systèmes tiers (API Beds24…)
* Sécurisation des flux et séparation stricte des données par compte
* Courbe d'apprentissage élevé d'AWS et d'Angular 



##### Leçons apprises

* L’importance du cadrage fonctionnel pour guider l’architecture
* Comment concevoir une API maintenable, sécurisée et claire
* Le rôle central de la modélisation métier dans un SaaS multi-utilisateur
* L’expérience d’un développement en conditions quasi-professionnelles grâce à un coaching encadré



##### Perspectives d’évolution

* Intégration d’un Channel Manager en marque blanche
* Moteur de réservation en ligne intégré
* Simulateur de marge selon modules activés
* Déploiement complet sur AWS avec résilience avancée




