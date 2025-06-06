# 🎨 VirtuArt

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

> **Projet Final Collaboratif - Wild Code School | Plateforme Artistique Full-Stack**

Plateforme web dédiée aux artistes et amateurs d'art, permettant de publier, découvrir et apprécier des créations artistiques. Développé en équipe lors du projet final de formation, ce projet illustre une maîtrise complète de la stack React/Express/MySQL avec des fonctionnalités avancées de gestion d'images et d'interactions sociales.


## 🎯 Contexte du Projet

**Type :** Projet final collaboratif (3-4 développeurs)  
**Formation :** Wild Code School - Développeur Web & Mobile  
**Durée :** 6 semaines de développement intensif  
**Méthodologie :** Agile avec sprints et daily stand-ups  

### 🎨 Vision du Projet
Créer un espace numérique où les artistes peuvent **partager leurs œuvres**, recevoir des **feedbacks constructifs** et développer leur **communauté artistique**. Une plateforme qui démocratise l'accès à l'art et encourage la créativité.

## ✨ Fonctionnalités Développées

### 🖼️ Gestion d'Œuvres Artistiques
- **Upload d'images** haute résolution avec optimisation automatique
- **Galerie Masonry** avec disposition dynamique des œuvres
- **Carousel interactif** pour navigation fluide entre images
- **Catégorisation** par style, technique et thème
- **Métadonnées enrichies** (dimensions, année, technique...)
- **Visualisation plein écran** avec zoom et navigation

### 👥 Interactions Sociales
- **Système de likes** et réactions sur les œuvres
- **Commentaires** constructifs et modérés
- **Profils d'artistes** avec biographie et portfolio
- **Système de followers** pour suivre ses artistes préférés
- **Notifications** en temps réel pour les interactions

### 🔍 Découverte & Navigation
- **Moteur de recherche** avancé avec filtres multiples
- **Feed personnalisé** basé sur les préférences
- **Recommandations** d'œuvres similaires
- **Navigation intuitive** par catégories et tags
- **Trending** et œuvres populaires

## 🚀 Stack Technique Complète

**Frontend React :**
- **React 18** avec hooks modernes (useState, useEffect, useContext)
- **React Router** pour navigation SPA fluide
- **CSS3 moderne** avec design responsive natif
- **Masonry** pour layouts de galerie dynamiques
- **Carousel library** pour navigation d'images fluide
- **Axios** pour communication API optimisée

**Backend Express :**
- **Express.js** avec architecture MVC structurée
- **Node.js** environnement serveur JavaScript
- **MySQL** base de données relationnelle avec Workbench
- **Multer** pour gestion avancée d'upload de fichiers

**Sécurité & Authentication :**
- **Argon2** pour hashage sécurisé des mots de passe
- **JWT** (JSON Web Tokens) pour sessions authentifiées
- **Middleware d'autorisation** pour protection des routes
- **Validation** côté client et serveur

**Outils de Développement :**
- **Harmonia** framework Wild Code School
- **ESLint + Prettier** pour qualité de code
- **Husky** pour hooks Git automatisés
- **Concurrently** pour développement full-stack

## 🏗️ Architecture Full-Stack

```
virtuart/
├── client/                    # Frontend React
│   ├── src/
│   │   ├── components/        # Composants réutilisables
│   │   │   ├── ArtworkCard.jsx
│   │   │   ├── UserProfile.jsx
│   │   │   └── SearchFilters.jsx
│   │   ├── pages/            # Pages principales
│   │   │   ├── Gallery.jsx
│   │   │   ├── ArtistProfile.jsx
│   │   │   └── Upload.jsx
│   │   ├── contexts/         # State management global
│   │   └── services/         # API calls et utilitaires
│   └── public/               # Assets statiques
│
├── server/                   # Backend Express
│   ├── src/
│   │   ├── controllers/      # Logique métier
│   │   │   ├── artworkController.js
│   │   │   ├── userController.js
│   │   │   └── authController.js
│   │   ├── middlewares/      # Authentification & validation
│   │   ├── models/          # Modèles de données MySQL
│   │   └── routes/          # Endpoints API REST
│   └── uploads/             # Stockage images uploadées
│
└── database/                # Configuration MySQL
    ├── schema.sql           # Structure des tables
    └── fixtures.sql         # Données de test
```

## 🛠️ Installation et Développement

### Prérequis
- Node.js 18+
- MySQL 8.0+
- npm ou yarn

### Configuration Rapide

```bash
# Cloner le repository
git clone https://github.com/Agraheris/afac974.git
cd afac974

# Installer les dépendances (client + server)
npm install

# Configuration base de données
# 1. Créer la base MySQL
# 2. Copier .env.sample vers .env dans client/ et server/
# 3. Configurer les variables d'environnement

# Migration et seed de la database
npm run db:migrate
npm run db:seed

# Lancer l'application complète
npm run dev
```

**URLs de développement :**
- Frontend : [http://localhost:3000](http://localhost:3000)
- Backend API : [http://localhost:5000](http://localhost:5000)

### Scripts Disponibles

```bash
npm run dev          # Lance client + server en parallèle
npm run dev:client   # Frontend React seul
npm run dev:back     # Backend Express seul
npm run db:migrate   # Migration base de données
npm run db:seed      # Insertion données de test
npm run lint         # Vérification qualité code
```

## 🎯 Fonctionnalités Techniques Avancées

### 📸 Gestion d'Images Professionnelle
- **Upload multiformat** (JPEG, PNG, WEBP) avec validation
- **Compression automatique** préservant la qualité artistique
- **Génération de thumbnails** pour performances optimales
- **Stockage organisé** par utilisateur et catégorie
- **Métadonnées EXIF** extraites et exploitées

### 🔐 Sécurité Renforcée
- **Authentification JWT** avec refresh tokens
- **Hashage Argon2** résistant aux attaques par force brute
- **Validation stricte** des inputs utilisateur
- **Protection CORS** configurée finement
- **Rate limiting** pour prévenir les abus

### ⚡ Optimisations Performance
- **Cache** des requêtes fréquentes
- **Optimisation bundle** React avec code splitting

## 💼 Compétences Développées

### 🎯 Développement Full-Stack
- **Architecture MVC** complète et scalable
- **API REST** bien structurée avec Express
- **State management** React avec Context API
- **Base de données relationnelle** MySQL avancée

### 👥 Collaboration en Équipe
- **Git Flow** avec branches feature et pull requests
- **Code review** systématique entre développeurs
- **Méthodologie Agile** avec sprints et rétrospectives
- **Pair programming** sur fonctionnalités complexes

### 🚀 Gestion de Projet Technique
- **Architecture système** pensée pour la scalabilité
- **Décomposition fonctionnelle** en user stories

## 🌟 Défis Techniques Relevés

### 🖼️ **Gestion d'Images à Grande Échelle**
Challenge majeur : optimiser l'upload et l'affichage de contenus visuels haute qualité tout en maintenant des performances web optimales.


### 🔗 **Architecture Full-Stack Cohérente**
Défi : assurer une communication fluide et sécurisée entre React frontend et Express backend avec gestion d'état complexe.

**Solutions développées :**
- API REST bien documentée
- Context API pour state global
- Middleware d'authentification robuste

### 👥 **Développement Collaboratif**
Challenge : coordonner le travail de 3-4 développeurs sur un projet complexe avec des fonctionnalités interdépendantes.

**Méthodologie appliquée :**
- Git workflow structuré
- Code review obligatoire
- Intégration continue

## 🎨 Aperçu Visuel


- Page d'accueil avec feed artistique
- Interface d'upload d'œuvres
- Profil d'artiste avec galerie
- Recherche avancée avec filtres

## 🔄 Évolutions et Améliorations

### 🎯 **Fonctionnalités Futures**
- **Messagerie privée** entre artistes
- **Système de commissions** et ventes
- **Events artistiques** et expositions virtuelles
- **Mobile app** React Native
- **AI recommendations** basées sur les goûts

### 🚀 **Optimisations Techniques**
- **Migration TypeScript** pour robustesse accrue
- **Tests automatisés** Jest/Cypress
- **CI/CD pipeline** avec déploiement automatique
- **Monitoring** et analytics avancés

## 🏆 Résultats du Projet

### ✅ **Objectifs Atteints**
- ✅ **Plateforme fonctionnelle** avec toutes les features MVP
- ✅ **Code quality** respectant les standards professionnels
- ✅ **Collaboration efficace** en équipe agile
- ✅ **Présentation réussie** devant jury professionnel
- ✅ **Expérience utilisateur** fluide et intuitive

### 📊 **Métriques Techniques**
- **Frontend :** ~15 composants React réutilisables
- **Backend :** 8 endpoints API REST documentés
- **Database :** 6 tables relationnelles optimisées
- **Performance :** <2s de temps de chargement
- **Responsive :** Compatible mobile/tablet/desktop

## 👨‍💻 Équipe de Développement

**Wild Code School - Projet Final Collaboratif**  
**Lead Developer :** Clément Vigouroux  
**Équipe :** 3-4 développeurs juniors  
**Durée :** 6 semaines intensives  
**Technologies :** React, Express, MySQL, Tailwind CSS

---

*🎨 Développé avec passion lors du projet final Wild Code School - Démonstration de maîtrise full-stack et collaboration en équipe*
