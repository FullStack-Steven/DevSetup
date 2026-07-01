# Notes — Les bases du terminal

## Qu'est-ce qu'un terminal ?

Le terminal est une interface en ligne de commande qui permet d'interagir directement avec le système d'exploitation, sans passer par une interface graphique. C'est l'outil de base indispensable à tout développeur.

## Commandes de navigation

| Commande | Description |
|---|---|
| `pwd` | Affiche le dossier courant (Print Working Directory) |
| `ls` | Liste le contenu du dossier courant |
| `ls -la` | Liste tout, y compris les fichiers cachés, en format détaillé |
| `cd <dossier>` | Se déplacer dans un dossier |
| `cd ..` | Remonter d'un niveau |
| `cd ~` | Retourner au dossier utilisateur (home) |

## Gestion des fichiers et dossiers

| Commande | Description |
|---|---|
| `touch <fichier>` | Crée un fichier vide |
| `mkdir <dossier>` | Crée un nouveau dossier |
| `rm <fichier>` | Supprime un fichier |
| `rm -r <dossier>` | Supprime un dossier et son contenu |
| `mv <source> <destination>` | Déplace ou renomme un fichier/dossier |
| `cp <source> <destination>` | Copie un fichier |
| `cat <fichier>` | Affiche le contenu d'un fichier |
|  `nano <fichier>` | Permet de modifier le contenu d'un fichier |

## Vérifier les outils installés

```bash
node -v      # version de Node.js
npm -v       # version de npm
git --version
```

## Ce que j'ai retenu

- Le terminal permet d'exécuter des actions bien plus rapidement qu'avec une souris une fois les commandes maîtrisées.
- Chaque commande a des options (flags) qui modifient son comportement, ex: `-l`, `-a`, `-r`.
- La touche `Tab` permet l'auto-complétion des noms de fichiers/dossiers — un gain de temps énorme.
- La flèche du haut (`↑`) permet de récupérer les commandes précédentes dans l'historique.
- Combiner plusieurs commandes avec `&&` permet de les exécuter à la suite (ex: `node -v && npm -v`).
