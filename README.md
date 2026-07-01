# DevSetup

> Répertoire de configuration de mon environnement de développement  
> Projet 1.1, Phase 1 (Environnement & Setup), Akieni Academy — Cohorte 2, 2026.

Ce repository documente la mise en place complète de mon environnement de développement Fullstack : installation des outils, configuration Git/GitHub, et bonnes pratiques de démarrage de projet.

---

##  Sommaire

- [DevSetup](#devsetup)
  - [Sommaire](#sommaire)
  - [Objectif du projet](#objectif-du-projet)
  - [Outils installés](#outils-installés)
    - [Vérifier les installations](#vérifier-les-installations)
  - [Configuration Git](#configuration-git)
  - [Structure du repository](#structure-du-repository)
  - [Comment utiliser ce repo](#comment-utiliser-ce-repo)
    - [1. Cloner le repository](#1-cloner-le-repository)
    - [2. Consulter les notes](#2-consulter-les-notes)
    - [3. Reproduire la configuration](#3-reproduire-la-configuration)
  - [Commandes Git essentielles](#commandes-git-essentielles)
    - [Push final](#push-final)
  - [Bonus réalisés](#bonus-réalisés)
  - [Notes d'apprentissage](#notes-dapprentissage)
  - [👤 Auteur](#-auteur)

---

##  Objectif du projet

Ce projet constitue la première étape du parcours Fullstack de Akieni Academy. Il vise à :

- Installer et configurer les outils de base d'un développeur (VSCode, Git, Node.js)
- Comprendre le fonctionnement du terminal et du système de contrôle de version Git
- Créer un compte GitHub et effectuer mes premiers commits/push
- Structurer un projet de façon professionnelle dès le départ

---

##  Outils installés

| Outil | Version | Rôle |
|---|---|---|
| **Node.js** | v24.16.0 | Environnement d'exécution JavaScript côté serveur |
| **npm** | 11.13.0 | Gestionnaire de paquets Node.js |
| **Git** | (configuré localement) | Système de contrôle de version |
| **VSCode** | — | Éditeur de code principal |
| **GitHub** | — | Hébergement distant du repository |

### Vérifier les installations

```bash
node -v
npm -v
git --version
```

---

##  Configuration Git

Configuration globale appliquée sur la machine :

```bash
user.name=FullStack-Steven
user.email=stevenkilonda1@gmail.com
http.postbuffer=524288000
core.autocrlf=true
```

Vérification :

```bash
git config --list
```

---

##  Structure du repository

```
DevSetup/
├── README.md          # Documentation du projet (ce fichier)
├── .gitignore         # Fichiers/dossiers ignorés par Git
├── .editorconfig       # Règles de formatage cohérentes entre éditeurs
└── notes/
    ├── 01-terminal.md      # Notes sur les bases du terminal
    ├── 02-git-github.md    # Notes sur Git et GitHub
    └── 03-environnement.md # Notes sur la configuration de l'environnement
```

---

##  Comment utiliser ce repo

### 1. Cloner le repository

```bash
git clone git@github.com:FullStack-Steven/DevSetup.git
cd DevSetup
```

### 2. Consulter les notes

Le dossier `notes/` contient mes notes personnelles prises pendant l'apprentissage (terminal, Git/GitHub, environnement).

### 3. Reproduire la configuration

Si tu veux repartir de ce setup comme base pour un nouveau projet, copie simplement `.gitignore` et `.editorconfig` dans ton nouveau dossier de projet.

---

##  Commandes Git essentielles

| Commande | Description |
|---|---|
| `git init` | Initialise un nouveau repository local |
| `git status` | Affiche l'état des fichiers (modifiés, indexés, etc.) |
| `git add <fichier>` | Ajoute un fichier à la zone de staging |
| `git add .` | Ajoute tous les fichiers modifiés |
| `git commit -m "message"` | Crée un commit avec les fichiers en staging |
| `git branch -M main` | Renomme la branche courante en `main` |
| `git remote add origin <url>` | Lie le repo local à un repo distant |
| `git push -u origin main` | Envoie les commits vers GitHub (1ère fois) |
| `git push` | Envoie les commits suivants |
| `git pull` | Récupère les dernières modifications distantes |
| `git log --oneline` | Historique des commits, format court |
| `git checkout -b dev` | Crée et bascule sur une nouvelle branche `dev` |
| `git merge dev` | Fusionne la branche `dev` dans la branche courante |

---

### Push final

```bash
git push -u origin main
```

---

##  Bonus réalisés

- [ ] Nodemon configuré pour le développement
- [x] Fichier `.editorconfig` ajouté au projet
- [ ] Branche `dev` créée et mergée dans `main`

---

##  Notes d'apprentissage

Voir le dossier [`notes/`](./notes) pour le détail de mes apprentissages sur :
- Les commandes de base du terminal
- Le fonctionnement de Git et GitHub
- La configuration d'un environnement de développement complet

---

## 👤 Auteur

**Steven Kilonda** ([FullStack-Steven](https://github.com/FullStack-Steven))
Académicien Fullstack — Akieni Academy, Cohorte 2 (2026)

---

*Ce projet fait partie du Projet 1.1 de la Phase 1 du parcours Fullstack de Akieni Academy.*