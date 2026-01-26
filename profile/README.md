<div align="center">
  <img src="https://avatars.githubusercontent.com/u/246091640?s=200&v=4" alt="ZenBNB Logo" width="120" height="120">
  <h1>ZenBNB</h1>
  <p><strong>La plateforme de référence pour le ménage des locations courte durée.</strong></p>
  
  <a href="https://zenbnb.fr">Site Web</a> • 
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

ZenBNB construit la première **Marketplace Contrôlée** qui connecte instantanément les propriétaires de biens immobiliers (Airbnb/Booking) avec des Cleaners professionnels vérifiés.

Notre défi technique est de combiner :
1.  **Flexibilité** : Un système d'enchères encadrées (Smart Pricing).
2.  **Rapidité** : Géolocalisation temps réel et matching instantané.
3.  **Sécurité** : Traçabilité totale (Photos, GPS, Logs) et paiements sécurisés.

---

## 📂 Architecture & Repositories

Nous fonctionnons avec une architecture **Monorepo** pour garantir la cohérence entre le Backend et le Frontend, accompagnée d'un dépôt de documentation.

| Repository | Description | Accès |
| :--- | :--- | :--- |
| **[`zenbnb-app`](./zenbnb-app)** | **⚡ LE CORE (Monorepo).** Contient tout le code source.<br>• `apps/backend` (NestJS API)<br>• `apps/frontend` (Next.js PWA)<br>• `packages/` (Shared Types, Config, Utils) | 🔒 **Restricted** |
| **[`zenbnb-specs`](./zenbnb-specs)** | **📘 LA DOCUMENTATION.**<br>La source de vérité fonctionnelle.<br>• Schémas de BDD (Looping/MCD)<br>• Spécifications V1 (PDF/Docx)<br>• Maquettes & Assets | 🔒 **Restricted** |
| **`.github`** | Configuration globale de l'organisation et templates de PR/Issues. |  public |

---

## 🛠 Notre Stack Technique

Nous utilisons des technologies modernes, typées et robustes pour assurer la scalabilité dès le premier jour.

### 🎨 Frontend (Web & Mobile PWA)
![Next.js](https://img.shields.io/badge/Next.js-14+-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat-square&logo=typescript)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-3-38B2AC?style=flat-square&logo=tailwind-css)
![PWA](https://img.shields.io/badge/PWA-Ready-purple?style=flat-square&logo=pwa)

### ⚙️ Backend (API)
![NestJS](https://img.shields.io/badge/NestJS-10-E0234E?style=flat-square&logo=nestjs)
![Node.js](https://img.shields.io/badge/Node.js-22_(LTS)-339933?style=flat-square&logo=node.js)
![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?style=flat-square&logo=prisma)

### 🗄️ Data & Infrastructure
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-316192?style=flat-square&logo=postgresql)
![PostGIS](https://img.shields.io/badge/PostGIS-Enabled-316192?style=flat-square&logo=postgresql)
![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker)
![Turborepo](https://img.shields.io/badge/Turborepo-Monorepo-EF4444?style=flat-square&logo=turborepo)

---

## 👥 L'Équipe

La Core Team technique et produit derrière la V1 de ZenBNB.

### 🧢 Management & Produit
| Rôle | Nom | Responsabilités |
| :--- | :--- | :--- |
| **CEO / Product Owner** | **M. Lazare** | Vision produit, Règles métier, Validation fonctionnelle, Administration Apple/Google. |

### 💻 Engineering Team
| Rôle | Nom | Github | Focus Principal |
| :--- | :--- | :--- | :--- |
| **Lead Developer** | **Adam** | [@AzmogEx](https://github.com/AzmogEx) | Architecture Backend, Base de données, DevOps, Sécurité. |
| **Frontend Developer** | **Victoire** | [@Vic2511](https://github.com/Vic2511) | UI/UX, Intégration Next.js, Animations, Responsive. |
| **Fullstack Developer** | **Victor** | [@vic-mtf](https://github.com/vic-mtf) | Logique métier, API, Intégration des flux (Paiement/Chat). |

---

## 🔄 Workflow de Développement

Pour maintenir une qualité de code "Production Ready", nous suivons ces règles strictes :

### 1. Gestion des Branches
* `main` : Code de production (Stable). Déploiement automatique.
* `develop` : Branche d'intégration (Test).
* `feature/nom-de-la-feature` : Branche de travail pour chaque développeur.

### 2. Règles de Commit (Conventional Commits)
Vos messages de commit doivent être clairs :
* `feat: ajout de la table CLEANER_PAYOUT`
* `fix: correction du calcul GPS sur la mission`
* `docs: mise à jour du README`
* `refactor: nettoyage du module Auth`

### 3. Code Review (PR)
Aucun code ne va sur `main` sans :
1.  Une **Pull Request (PR)** ouverte.
2.  Une validation par au moins 1 autre développeur.
3.  Le passage au vert des tests CI (Linting, Build).

---

## 🔐 Sécurité & Accès

* **Identifiants :** Ne committez JAMAIS de clés API ou de mots de passe. Utilisez le fichier `.env` (ajouté au `.gitignore`).
* **Base de Données :** Le script d'initialisation SQL "Gold Version" se trouve dans `packages/database/init.sql`. Ne modifiez pas la structure sans l'accord du Lead Dev.

---

## 📞 Contact Interne

En cas de problème critique (Prod down, faille de sécurité) :

* **Urgence Technique :** Adam (Discord / Tel / WhatsApp)
* **Urgence Produit :** M. Lazare (WhatsApp)

---

<div align="center">
  <small>© 2025 ZenBNB. Tous droits réservés. Code propriétaire et confidentiel.</small>
</div>
