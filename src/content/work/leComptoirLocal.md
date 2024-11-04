---
title: Le comptoir local
publishDate: 2024-11-20 00:00:00
img: /assets/logo-comptoir-local.png
img_alt: Logo de l'application
description: |
  Le Comptoir Local est un projet en cours développé en collaboration avec l'organisation Github Pinqo.
tags:
  - SpringBoot/Java
  - React
  - API
---

##### Objectif

- Marketplace : Mise en relation directe des producteurs et des consommateurs.
- Filtrage avancé : Permet aux utilisateurs de trouver rapidement les produits qu'ils recherchent en fonction de critères spécifiques (lieu, type de produit, certifications, etc.).
- Gestion des commandes : Simplifier le processus de commande et de livraison, avec une traçabilité complète.
- Interface producteur : Fournir aux producteurs un tableau de bord clair pour gérer leur activité et analyser leurs performances.
- Outils d'analyse : Permettre aux consommateurs d'évaluer l'impact environnemental de leurs achats.

##### Organisation du projet :

- Analyse des besoins ;
- Etude de l'architecture et choix des technologies
- Modélisation des données
- Maquettage du projet ;
- Sécurité de l'application et des données ;
- Gestion de projet / Plan d'organisation du projet de développement ;
- Développement de l'application

##### Fonctionnalités :

**Front-End**

- Recherche de produits : Recherche et filtrage des produits en fonction de divers critères.
- Détails du produit : Informations détaillées sur le produit
- Panier d'achat : Ajouter des articles au panier, afficher le contenu du panier et passer à la caisse.
- Profil de l'utilisateur : Gérer les informations relatives au compte, consulter l'historique des commandes.

**Back-End**

- Gestion des utilisateurs : Enregistrement, authentification et autorisation des utilisateurs.
- Gestion des produits : Opérations CRUD pour les produits, y compris les catégories et les attributs.
- Gestion des commandes : Création, traitement et suivi des commandes.
- Traitement des paiements : Intégration avec Stripe pour les paiements sécurisés.
- Panneau d'administration : Pour la gestion de la plateforme, y compris la modération des produits et la gestion des utilisateurs.

##### Stack :

- Couche Web : React / Typescript / Vite;
- couche métier : JAVA / SpingBoot
- server : Tomcat
- Conteneurisation : Docker
- Base de données : Serveur Postgres
- ApiRestfull : Swagger UI
- Versionning / Tests : Github
- <a href = "https://github.com/Pinqo-community/marketplace-app" target="_blank">lien vers github</a>
