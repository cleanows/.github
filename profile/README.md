<div align="center">
  <img src="https://cleanows.fr/logo_cleanows_horizontal.svg" height="60">
  <p style="margin-top: 50px;"><strong>La plateforme de référence pour le ménage des locations courte durée.</strong></p>

  <a href="https://cleanows.fr">Site Web</a> • 
  <a href="#-architecture--repositories">Repositories</a> • 
  <a href="#-notre-stack-technique">Tech Stack</a> • 
  <a href="#-léquipe">L'Équipe</a>

  <br><br>
  
  ![Status](https://img.shields.io/badge/Status-V1%20Development-blue?style=for-the-badge)
  ![License](https://img.shields.io/badge/Private-Proprietary-red?style=for-the-badge)
</div>

---

## 🚀 Notre Mission

**"Vous louez, on s'occupe du reste."**

Cleanow’s construit la première **Marketplace Contrôlée** qui connecte instantanément les propriétaires de biens immobiliers (Airbnb/Booking) avec des Cleaners professionnels vérifiés.

Notre défi technique repose sur trois piliers :
1. **Flexibilité** : Système d’enchères encadrées (Smart Pricing).
2. **Rapidité** : Géolocalisation temps réel & matching instantané.
3. **Sécurité** : Traçabilité totale (Photos, GPS, Logs) & paiements sécurisés.

---

## 📂 Architecture & Repositories

L’architecture n’est **plus un monorepo** :  
Chaque application est **indépendante**, versionnée et déployée séparément.

Chaque repository contient au minimum :
- une branche **main** (production)
- une branche **dev** (tests & intégration)

### 🔧 Repositories Principaux

| Repository | Description | Accès |
| :--- | :--- | :--- |
| **`app-server`** | API Backend (NestJS, Prisma, Auth, Logic métier). | 🔒 Privé |
| **`app-client`** | Application Web & Mobile (Expo, React Native, Web). | 🔒 Privé |
| **`landing-page`** | Site vitrine Cleanow’s (Next.js / Static). | 🔒 Privé |
| **`.github`** | Templates PR/Issues & configuration globale. | Public |

---

## 🛠 Notre Stack Technique

Nous utilisons des technologies modernes, typées et robustes pour assurer la scalabilité dès le premier jour.

### 🎨 Frontend (Web & Mobile)
![Expo](https://img.shields.io/badge/Expo-React_Native-black?style=flat-square&logo=expo)
![React Native](https://img.shields.io/badge/React_Native-0.7x-61DAFB?style=flat-square&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat-square&logo=typescript)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-NativeWind-38B2AC?style=flat-square&logo=tailwind-css)

### ⚙️ Backend (API)
![NestJS](https://img.shields.io/badge/NestJS-10-E0234E?style=flat-square&logo=nestjs)
![Node.js](https://img.shields.io/badge/Node.js-22_(LTS)-339933?style=flat-square&logo=node.js)
![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?style=flat-square&logo=prisma)

### 🗄️ Data & Infrastructure
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-316192?style=flat-square&logo=postgresql)
![PostGIS](https://img.shields.io/badge/PostGIS-Enabled-316192?style=flat-square&logo=postgresql)
![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker)

---

## 👥 L'Équipe

La Core Team technique et produit derrière la V1 de Cleanow’s.

### 🧢 Management & Produit
| Rôle | Nom | Responsabilités |
| :--- | :--- | :--- |
| **CEO / Product Owner** | **M. Lazare** | Vision produit, Règles métier, Validation fonctionnelle, Administration Apple/Google. |

### 💻 Engineering Team
| Rôle | Nom | Github | Focus Principal |
| :--- | :--- | :--- | :--- |
| **Lead Developer** | **Adam** | [@AzmogEx](https://github.com/AzmogEx) | Architecture Backend, Base de données, DevOps, Sécurité. |
| **Frontend Developer** | **Victoire** | [@Vic2511](https://github.com/Vic2511) | UI/UX, Expo, Web/Mobile, Animations. |
| **Fullstack Developer** | **Victor** | [@vic-mtf](https://github.com/vic-mtf) | Logique métier, API, Intégration des flux (Paiement/Chat). |

---

## 🔄 Workflow de Développement

### 1. Gestion des Branches
* `main` : Code de production (stable). Déploiement automatique.
* `dev` : Branche d’intégration (tests).
* `feature/nom-de-la-feature` : Branche de travail.

### 2. Règles de Commit (Conventional Commits)
Exemples :
* `feat: ajout du module de réservation`
* `fix: correction du matching GPS`
* `docs: mise à jour du README`
* `refactor: nettoyage du module Auth`

### 3. Code Review (PR)
Aucun code ne va sur `main` sans :
1. Une **Pull Request** ouverte.
2. Une validation par au moins 1 développeur.
3. Les tests CI au vert (Linting, Build).

---

## 🔐 Sécurité & Accès

* **Identifiants :** Ne jamais commit des clés API ou mots de passe. Utiliser `.env` (ignoré par Git).
* **Base de Données :** Le script d’initialisation SQL est maintenu dans `app-server`.  
  Toute modification de structure doit être validée par le Lead Dev.

---

## 📞 Contact Interne

En cas de problème critique (prod down, faille de sécurité) :

* **Urgence Technique :** Adam (Discord / Tel / WhatsApp)
* **Urgence Produit :** M. Lazare (WhatsApp)

---

<div align="center">
  <small>© 2025 Cleanow’s — Tous droits réservés. Code propriétaire et confidentiel.</small>
</div>
