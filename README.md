# 🍽️ Vite Gourmand - Frontend

> Application web de gestion de recettes développée avec Angular 18

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=nicov51_Vite-Gourmand_frontend&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=nicov51_Vite-Gourmand_frontend)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=nicov51_Vite-Gourmand_frontend&metric=bugs)](https://sonarcloud.io/summary/new_code?id=nicov51_Vite-Gourmand_frontend)
[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=nicov51_Vite-Gourmand_frontend&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=nicov51_Vite-Gourmand_frontend)

## 📋 Table des matières

- [Prérequis](#-prérequis)
- [Installation](#-installation)
- [Développement](#-développement)
- [Tests](#-tests)
- [Build et déploiement](#-build-et-déploiement)
- [Qualité du code](#-qualité-du-code)
- [Architecture](#-architecture)
- [Scripts utiles](#-scripts-utiles)

## 🔧 Prérequis

Avant de commencer, assurez-vous d'avoir installé :

- **Node.js** : Version 20.x ([Télécharger](https://nodejs.org/))
- **npm** : Version 11.x+ (fourni avec Node.js)
- **Angular CLI** : Version 18.x

```bash
# Vérification des versions
node --version    # v20.x.x
npm --version     # 11.x.x+

# Installation d'Angular CLI si nécessaire
npm install -g @angular/cli@18
ng version
```

## 🚀 Installation

### 1. Cloner le projet

```bash
git clone https://github.com/nicov51/Vite-Gourmand_frontend.git
cd Vite-Gourmand_frontend
```

### 2. Installer les dépendances

```bash
npm install
```

### 3. Démarrer l'application

```bash
# Lancement du serveur de développement
ng serve

# Ou avec npm
npm start
```

L'application sera accessible à l'adresse : **http://localhost:4200**

Le serveur redémarre automatiquement lors des modifications de code.

## 💻 Développement

### Serveur de développement

```bash
# Démarrage standard
ng serve

# Avec port personnalisé
ng serve --port 4201
```

## 🧪 Tests

### Tests unitaires

```bash
# Lancement des tests unitaires
npm test

# Tests avec surveillance des changements
npm run test:watch

# Tests en mode headless pour CI/CD
npm run test:ci
```

### Linting

```bash
# Vérification du code (si configuré)
ng lint

# Correction automatique
ng lint --fix
```

## 🏗️ Build et déploiement

### Build de développement

```bash
ng build
```

### Build de production

```bash
# Build optimisé pour la production
ng build --configuration production

# Ou plus court
ng build --prod
```

Les fichiers sont générés dans le dossier `dist/vite-gourmand-frontend/`

### Preview du build de production

```bash
# Après avoir fait un build de production
npx http-server dist/vite-gourmand-frontend -p 8080
```

## 📊 Qualité du code

### SonarCloud

Ce projet utilise **SonarCloud** pour l'analyse automatique de la qualité du code.

- **Déclenchement** : À chaque push sur `main` ou `develop`
- **Analyse** : Bugs, vulnérabilités, code smells, couverture de tests
- **Seuils de qualité** :
  - 🎯 Coverage : à definir
  - 🐛 Bugs : 0 tolérance
  - 🔒 Vulnerabilities : 0 tolérance
  - 📊 Maintainability : A minimum

**Accéder aux résultats :** [SonarCloud Dashboard](https://sonarcloud.io/project/overview?id=nicov51_Vite-Gourmand_frontend)

### Configuration SonarCloud

Le projet est configuré avec :
- `sonar-project.properties` : Configuration des règles
- `.github/workflows/build.yml` : Pipeline CI/CD

## 📁 Architecture

```
src/app/
├── components/        # Composants réutilisables
├── directives/        # Directives personnalisées
├── guards/           # Guards de navigation
├── interceptors/     # Intercepteurs HTTP
├── models/          # Interfaces et types TypeScript
├── pipes/           # Pipes personnalisés
├── services/        # Services applicatifs
└── utils/           # Utilitaires et helpers
```

### Conventions de nommage

- **Composants** : `recipe-card.component.ts`
- **Services** : `recipe.service.ts`
- **Models** : `recipe.interface.ts`
- **Guards** : `auth.guard.ts`
- **Pipes** : `truncate.pipe.ts`

## Scripts utiles

```bash
# Package.json scripts disponibles
npm start              # ng serve
npm run build          # ng build
npm run build:prod     # ng build --configuration production
npm test               # Tests unitaires
npm run test:watch     # Tests en mode surveillance
npm run test:ci        # Tests pour CI/CD
```

## 🔗 Ressources utiles

- **Documentation Angular** : [angular.io](https://angular.io)
- **Angular CLI** : [cli.angular.io](https://cli.angular.io)
- **SonarCloud** : [sonarcloud.io](https://sonarcloud.io)

## 🤝 Contribution

1. **Fork** le projet
2. Créer une branche feature (`git checkout -b feature/my-feature`)
3. **Commit** les changements (`git commit -m 'Add my-feature'`)
4. **Push** vers la branche (`git push origin feature/my-feature`)
5. Ouvrir une **Pull Request**

## 👥 Équipe

- **Développeur Principal** : Nicolas V.
- **Framework** : Angular 18.2.x
- **Qualité** : SonarCloud intégré

---

⭐ **N'hésitez pas à laisser une étoile si ce projet vous plaît !**

