# 🌿 Notes — Git & GitHub

## Git vs GitHub

- **Git** : un système de contrôle de version, installé localement, qui permet de suivre l'historique des modifications d'un projet.
- **GitHub** : une plateforme en ligne qui héberge des repositories Git et permet la collaboration (push, pull, pull requests, issues...).

## Initialiser un projet Git

```bash
git init                # initialise un repo Git dans le dossier courant
git status               # affiche l'état des fichiers (modifiés, suivis, non suivis)
git add <fichier>        # ajoute un fichier précis au staging
git add .                # ajoute tous les fichiers modifiés au staging
git commit -m "message"  # crée un commit avec les fichiers du staging
```

## Lier le projet local à GitHub

```bash
git branch -M main
git remote add origin <url-du-repo>
git push -u origin main
```


## Commandes utiles au quotidien

| Commande | Description |
|---|---|
| `git log --oneline` | Historique des commits en version courte |
| `git diff` | Affiche les différences non indexées |
| `git checkout -b <branche>` | Crée une nouvelle branche et bascule dessus |
| `git merge <branche>` | Fusionne une branche dans la branche courante |
| `git remote -v` | Affiche les remotes configurés |
| `git pull` | Récupère et fusionne les changements distants |

## Ce que j'ai retenu

- Un bon message de commit doit être clair et décrire **ce qui a changé**, pas juste "update".
- Il vaut mieux faire des petits commits fréquents plutôt qu'un seul gros commit.
