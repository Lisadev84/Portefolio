---
title: Le cercle des pêcheurs
publishDate: 2024-08-21 00:00:00
img: /assets/logo-pecheurs.png
img_alt: Logo du blog "le cercle des pêcheurs"
description: |
  Blog de partage d'articles déposés par les utilisateurs sur la pratique de la pêche
tags:
  - PHP
  - NGINX VPS
---


<p style = "text-align:justify;">
Cette application a été réalisée au cours de la formation PHP et adapté pour un membre de la famille passionné de pêche. L'objectif premier était l'apprentissage de la partie back-end. Le Front est resté sobre.
Chaque utilisateurs peut soumettre, consulter et éditer un article. 
Le backoffice gère les utilisateurs, les sessions et les articles.
</p> 

##### Fonctionnalités
- Show article : Présentation de tous les articles
- Read article : Lecture d'article en détail
- Create article : Après inscription, chaque utilisateur peut créer un article
- Edit article: Chaque article peut être modifier par son auteur et l'administrateur
- Registration : Inscription des utilisateurs, 
- Profile : Gestion par l'utilisateur de son profil avec la liste des articles produits (modification/suppression) 
- Login/Logout : Connexion/Déconnexion des utilisateurs

##### Stack
- Frontend : HTML, CSS, JavaScript, Bootstrap
- Backend : PHP8
- Base de données relationnelle : Mysql

##### Déploiement
- VPS(Virtual Private Server)
- Mise en production : Nginx, php-fpm, MySQL et configuration de HTTPS avec Cerbot et Letsencrypt
- Hébergement : OVH
- <a href = "https://www.lecercledespecheurs.ovh" target="_blank">lien vers le site</a>


