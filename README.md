# GPT-3

<div align="center">

**[Français](#français)** · **[English](#english)**

</div>

---

## Français

### 📋 Présentation

Bienvenue sur le code source de **GPT-3**, une landing page sur le thème de l'intelligence artificielle. Ce projet met l'accent sur l'intégration d'une interface en **React** : composition en composants réutilisables, mise en page responsive et travail visuel en CSS, avec un fond bleu nuit, des titres en dégradé et des illustrations.

L'application fonctionne aujourd'hui avec **React 19** et **Vite 8**. Il s'agit d'une vitrine frontend au contenu en anglais ; elle n'intègre pas l'API OpenAI et ne propose pas de génération de texte.

### 📑 Les sections

Le site se compose d'une seule page, avec une navigation par ancres.

| Section | Ce qu'on y trouve |
| --- | --- |
| `/#home` | Présentation principale, illustration, champ email et appel à l'action |
| Marques | Bandeau de logos Google, Slack, Atlassian, Dropbox et Shopify |
| `/#wgpt3` | Présentation de GPT-3 et de ses usages : chatbots, base de connaissances et éducation |
| `/#features` | Liste de fonctionnalités organisée avec le composant réutilisable `Feature` |
| `/#possibility` | Illustration et présentation des possibilités de l'IA |
| Appel à l'action | Bandeau invitant à demander un accès anticipé |
| `/#blog` | Grille de cinq cartes d'articles avec images, dates et titres |
| Pied de page | Logo, liens et coordonnées de démonstration |

### 🎨 Interface & Navigation

- **Mise en page responsive** : dispositions adaptées aux écrans de bureau, tablettes et mobiles grâce aux media queries CSS.
- **Menu mobile** : ouverture et fermeture pilotées par `useState`, avec les icônes Remix de React Icons.
- **Navigation par ancres** : accès aux sections depuis la barre de navigation, avec défilement fluide en CSS.
- **Identité visuelle** : police Manrope chargée via Google Fonts, titres en dégradé et animation CSS d'apparition du menu.
- **Composants réutilisables** : cartes d'articles, blocs de fonctionnalités, bandeau de marques et appel à l'action.

> Le champ email et les boutons d'inscription ou d'accès sont des éléments de démonstration : aucun email n'est envoyé et aucun compte n'est créé. Les cartes du blog ne sont pas reliées à des pages d'articles.

### 🛠 Stack technique

| Catégorie | Technologies |
| --- | --- |
| Librairie UI | React 19.3.1 + React DOM 19.3.1 |
| Outil de développement & Build | Vite 8.3.5 + plugin React 6.1.2 |
| Langage | JavaScript (JSX), modules ES |
| Package manager | Bun 1.4.2 |
| Styling | CSS, variables, Flexbox, Grid et media queries |
| Icônes | React Icons 5.7.0 — Remix Icons |
| Typographie | Manrope via Google Fonts |

### 📁 Structure du projet

```text
gpt3/
├── public/                      # Ressources statiques publiques
├── src/
│   ├── assets/                  # Illustrations, logos et images du blog
│   ├── components/
│   │   ├── article/             # Carte d'article
│   │   ├── brand/               # Bandeau de marques
│   │   ├── cta/                 # Bandeau d'appel à l'action
│   │   ├── feature/             # Bloc de fonctionnalité réutilisable
│   │   └── navbar/              # Navigation bureau et menu mobile
│   ├── containers/
│   │   ├── blog/                # Grille d'articles
│   │   ├── features/            # Section des fonctionnalités
│   │   ├── footer/              # Pied de page
│   │   ├── header/              # Section d'accueil
│   │   ├── possibility/         # Présentation illustrée
│   │   └── whatGPT3/            # Présentation de GPT-3
│   ├── App.jsx                  # Assemblage de la page
│   ├── App.css                  # Styles partagés et animations
│   ├── index.css                # Police et variables de thème
│   └── main.jsx                 # Point d'entrée React (createRoot)
├── index.html                   # Document HTML d'entrée
├── vite.config.js              # Configuration Vite et plugin React
├── bun.lock                     # Versions verrouillées des dépendances
└── package.json                 # Dépendances et scripts
```

### 🚀 Pour lancer le projet

**Prérequis** : Bun 1.4.2 et une version de Node.js compatible avec Vite 8 (`^20.19.0 || >=22.12.0`). Le projet a été vérifié avec Node.js 24.

```sh
git clone https://github.com/ruddyautem/gpt3.git
cd gpt3
bun install --frozen-lockfile
bun run dev
```

Direction [http://localhost:5173](http://localhost:5173), ou l'adresse affichée par Vite si ce port est occupé. Aucun fichier `.env` ni aucune clé API ne sont nécessaires.

Pour générer et prévisualiser la version de production :

```sh
bun run build
bun run preview
```

Le build est généré dans `dist/`. La prévisualisation est disponible par défaut sur [http://localhost:4173](http://localhost:4173) ; elle sert à vérifier le build localement avant de publier les fichiers sur un hébergement statique.

### ✅ Vérifications & Maintenance

`bun.lock` est le lockfile de référence et les dépendances directes sont fixées à des versions précises. Après une modification :

- Exécuter `bun run build` et `git diff --check`.
- Vérifier le rendu, le chargement des images et les liens de navigation sur bureau et mobile.
- Tester la saisie email et l'ouverture/fermeture du menu mobile en développement et via `bun run preview`.
- Vérifier l'absence d'erreur ou d'avertissement React dans la console du navigateur.

Le dépôt ne contient actuellement ni suite de tests automatisés ni configuration de lint. Le README est bilingue ; le contenu de l'application reste en anglais.

### À propos de moi

Je suis Ruddy Autem, développeur Full Stack. Retrouvez mes autres projets sur [autem.dev](https://autem.dev) ou sur [GitHub](https://github.com/ruddyautem).

---

## English

### 📋 Overview

Welcome to the source code of **GPT-3**, an AI-themed landing page. This project focuses on building a **React** interface with reusable components, responsive layouts and CSS styling, featuring a dark blue background, gradient headings and illustrations.

The application now runs on **React 19** and **Vite 8**. It is a frontend showcase with English content; it does not integrate the OpenAI API or generate text.

### 📑 Sections

The site is a single page with anchor navigation.

| Section | What you'll find |
| --- | --- |
| `/#home` | Hero section with an illustration, email field and call to action |
| Brands | Logo strip featuring Google, Slack, Atlassian, Dropbox and Shopify |
| `/#wgpt3` | Introduction to GPT-3 and its uses: chatbots, knowledge bases and education |
| `/#features` | Feature list built with the reusable `Feature` component |
| `/#possibility` | Illustration and introduction to AI possibilities |
| Call to action | Banner inviting visitors to request early access |
| `/#blog` | Five article cards with images, dates and titles |
| Footer | Logo, links and placeholder contact details |

### 🎨 Interface & Navigation

- **Responsive layout**: CSS media queries adapt the page to desktop, tablet and mobile screens.
- **Mobile menu**: `useState` controls opening and closing, using Remix icons from React Icons.
- **Anchor navigation**: navigation links lead to page sections with CSS smooth scrolling.
- **Visual style**: Manrope loaded through Google Fonts, gradient headings and a CSS menu entrance animation.
- **Reusable components**: article cards, feature blocks, brand strip and call-to-action banner.

> The email field and sign-up/access buttons are demonstration UI: no email is sent and no account is created. Blog cards do not link to article pages.

### 🛠 Tech Stack

| Category | Technologies |
| --- | --- |
| UI library | React 19.3.1 + React DOM 19.3.1 |
| Development & Build | Vite 8.3.5 + React plugin 6.1.2 |
| Language | JavaScript (JSX), ES modules |
| Package manager | Bun 1.4.2 |
| Styling | CSS, custom properties, Flexbox, Grid and media queries |
| Icons | React Icons 5.7.0 — Remix Icons |
| Typography | Manrope via Google Fonts |

### 📁 Project Structure

```text
gpt3/
├── public/                      # Public static assets
├── src/
│   ├── assets/                  # Illustrations, logos and blog images
│   ├── components/              # Article, Brand, CTA, Feature and Navbar
│   ├── containers/              # Blog, Features, Footer, Header,
│   │                            # Possibility and WhatGPT3 sections
│   ├── App.jsx                  # Page composition
│   ├── App.css                  # Shared styles and animations
│   ├── index.css                # Font and theme variables
│   └── main.jsx                 # React entry point (createRoot)
├── index.html                   # HTML entry point
├── vite.config.js              # Vite configuration and React plugin
├── bun.lock                     # Locked dependency versions
└── package.json                 # Dependencies and scripts
```

### 🚀 Running Locally

**Requirements**: Bun 1.4.2 and a Node.js version supported by Vite 8 (`^20.19.0 || >=22.12.0`). The project has been verified with Node.js 24.

```sh
git clone https://github.com/ruddyautem/gpt3.git
cd gpt3
bun install --frozen-lockfile
bun run dev
```

Open [http://localhost:5173](http://localhost:5173), or the address printed by Vite if that port is busy. No `.env` file or API key is required.

To build and preview the production version:

```sh
bun run build
bun run preview
```

The build is generated in `dist/`. The preview defaults to [http://localhost:4173](http://localhost:4173); use it to check the build locally before publishing the files to a static host.

### ✅ Checks & Maintenance

`bun.lock` is the reference lockfile, and direct dependencies are pinned to specific versions. After making changes:

- Run `bun run build` and `git diff --check`.
- Check the layout, image loading and navigation links on desktop and mobile.
- Test email input and opening/closing the mobile menu in development and through `bun run preview`.
- Check the browser console for React errors or warnings.

The repository currently has no automated test suite or lint configuration. This README is bilingual; the application content remains in English.

### About Me

I'm Ruddy Autem, a Full Stack developer. Find my other projects at [autem.dev](https://autem.dev) or on [GitHub](https://github.com/ruddyautem).
