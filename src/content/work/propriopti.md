---
title: SaaS en cours — Propri'Opti
publishDate: 2026-01-15 00:00:00
img: /assets/logo-propriopti.png
img_alt: Logo de l'application Propri'Opti
description: |
  Propri'Opti est une application SaaS de gestion locative dédiée aux hébergements saisonniers (gîtes, chambres d’hôtes, locations touristiques).
projectUrl: "https://app.propriopti.fr/"
projectLabel: Voir l’app
tags:
  - SpringBoot/Java
  - Angular 20
  - AWS 
---

#### Contexte & problématique

La gestion d’une activité de location saisonnière repose souvent sur un empilement d’outils (tableurs, e-mails, agendas, modèles Word/PDF, paiements, messageries).
Résultat : des tâches répétitives, des oublis (relances, documents), des informations dispersées, et un risque accru d’erreur (surbooking, incohérences de statut, documents envoyés trop tôt/trop tard).

**Propri'Opti** est conçu pour centraliser ces flux dans une plateforme unique, en s’appuyant sur un modèle métier robuste et une architecture prête à évoluer.  Le produit vise à réduire la charge mentale des exploitants et à fiabiliser leurs processus (réservations, documents, suivi client),tout en préparant une montée en puissance vers l’intégration OTA via Channel Manager.

---

#### Objectifs produit

Concevoir une plateforme **robuste, modulaire et intuitive** permettant de :

- Centraliser les réservations (MVP : hors OTA)
- Gérer un **planning fiable** et exploitable
- Structurer la relation client (fiche client / cardex)
- Automatiser les documents et les communications (contrat, devis, facture, relances)
- Préparer l’intégration d’un Channel Manager (ex. Beds24) et l’industrialisation du modèle



#### Analyse des besoins & cadrage fonctionnel

##### Segmentation des utilisateurs (personas)

Le produit répond à deux réalités opérationnelles distinctes :

1. **Propriétaire (Owner)**  
   Besoin principal : *gérer efficacement son ou ses hébergements*, sécuriser ses procédures (réservation → confirmation → documents), et gagner du temps au quotidien.

2. **Mandataire / Gestionnaire (Manager)**  
   Besoin principal : *piloter une activité multi-propriétaires* avec une vision consolidée (réservations, planning, documents), tout en gardant des règles d’accès contrôlées et traçables.

Ce cadrage structure les fonctionnalités et l’UX : tableau de bord, filtres multi-entités, délégations, historique d’actions, etc. :contentReference[oaicite:0]{index=0}

##### Besoins clés identifiés (problèmes récurrents)

- **Centralisation** : informations dispersées (agenda, mails, pièces jointes, fichiers modèles)
- **Fiabilité** : statut de réservation ambigu, règles non uniformes, risques d’erreurs de synchronisation
- **Automatisation** : relances, documents, rappels (arrivée, solde, signature)
- **Gestion multi-acteurs** : propriétaire seul vs gestion multi-propriétaires avec droits contrôlés
- **Évolutivité** : préparer le terrain pour de futures intégrations (OTA/Channel Manager)

##### Traduction en règles métier (exemple : réservations)

Une partie importante du travail consiste à **transformer les besoins en invariants métier** :  
- prévention du **surbooking**  
- gestion d’un cycle de vie clair (intention, option, confirmation, annulation)  
- traçabilité via un historique d’évènements (approche append-only)  
:contentReference[oaicite:1]{index=1}



#### Fonctionnalités (MVP)

##### Propriétaire
- Dashboard organisationnel (check-in/out, alertes, suivi)
- Gestion des hébergements (création, liste, optimisation pricing : saisonnalités, règles de durée, duplication multi-hébergements)
- Planning & gestion des réservations et de leurs statuts
- Fiche client (cardex)
- Automatisation des documents et envois (confirmations / relances)
- Listing & suivi des documents produits

##### Gestionnaire
- Vue centralisée des réservations + filtrage multi-propriétaires
- Paramétrage activité (parc, documents type, informations commerciales)
- Blocage massif de calendrier multi-biens
- Journal d’activités (audit) et historique des actions (cible MVP)
- Collaboration : délégations et droits ajustables

Référentiel de priorisation MVP/V1 : :contentReference[oaicite:2]{index=2}



#### Stack technique & architecture

##### Backend
- Java 21 / Spring Boot 3
- API REST
- Hibernate/JPA
- Sécurité : JWT + contrôle d’accès fin (scopes)

##### Frontend
- Angular 20 (standalone) + Angular Material
- UI orientée rôles (Owner / Manager / Tech/Admin)

##### Données
- MySQL
- Modélisation relationnelle orientée métier (UML/MLD)

##### Cloud & DevOps
- AWS : EC2, S3, RDS, VPC, Load Balancer, CloudFront
- Préparation à l’Infrastructure as Code (IaC)

##### Qualité
- Tests unitaires & intégration (JUnit, Mockito)
- Git / GitHub



#### Défis rencontrés

- **Multi-utilisateurs & isolation des données** : conception d’un modèle d’autorisations cohérent, limitation des accès selon rôle et périmètre.
- **Complexité métier des réservations** : définition d’états, transitions, règles de non-chevauchement, et logique d’option (hold/expiration). :contentReference[oaicite:3]{index=3}
- **Conception “prête pour l’avenir”** : préparer l’intégration OTA sans sur-complexifier le MVP (découpage modulaire, métadonnées, extensibilité).
- **Montée en compétence cloud / Angular** : mise en place progressive d’une architecture AWS et d’un front moderne.



#### Leçons apprises

- Le **cadrage fonctionnel** est structurant : il évite de “coder dans le vide” et guide l’architecture.
- La **modélisation métier** est centrale en SaaS : elle conditionne la sécurité, l’évolutivité, et la maintenabilité.
- La **traçabilité** (audit / historique d’évènements) devient vite indispensable dès qu’il y a multi-acteurs et enjeux de fiabilité.
- Développement en conditions proches du réel : itérations, arbitrages MVP, revues de code, priorisation.



#### Perspectives (V1+)

- Intégration Channel Manager (marque blanche)
- Moteur de réservation en ligne
- Industrialisation de l’automatisation documentaire (templates,    e-signature)
- Module de gestion commerciale et comptable
- Renforcement résilience AWS + automatisation CI/CD





