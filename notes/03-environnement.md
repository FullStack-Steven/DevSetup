# Configuration de l'environnement de développement

## Pourquoi bien configurer son environnement ?

Un environnement de développement bien configuré dès le départ permet de :
- Gagner du temps sur le long terme
- Éviter les erreurs liées à des configurations incohérentes entre projets
- Faciliter la collaboration avec d'autres développeurs (formatage cohérent, fichiers ignorés communs, etc.)

## Outils installés et leur rôle

| Outil | Rôle |
|---|---|
| **VSCode** | Éditeur de code principal, avec extensions pour améliorer la productivité |
| **Node.js** | Permet d'exécuter du JavaScript en dehors du navigateur (côté serveur) |
| **npm** | Gestionnaire de paquets livré avec Node.js, pour installer des librairies |
| **Git** | Suivi de version du code source |

## Configuration Git globale

```bash
git config --global user.name "FullStack-Steven"
git config --global user.email "stevenkilonda1@gmail.com"
git config --global http.postbuffer 524288000
git config --global core.autocrlf true
```

- `user.name` / `user.email` : identifient l'auteur des commits.
- `http.postbuffer` : augmente la taille du buffer HTTP, utile pour les gros pushs.
- `core.autocrlf` : gère la conversion des fins de ligne entre Windows (CRLF) et Unix (LF).

## Le fichier `.gitignore`

Sert à indiquer à Git quels fichiers/dossiers ne doivent **jamais** être suivis ni envoyés sur GitHub (fichiers sensibles, fichiers générés automatiquement, dépendances lourdes...).

Exemple standard pour un projet Node.js :
```
node_modules/
.env
.DS_Store
npm-debug.log
dist/
build/
.vscode/
```

## Le fichier `.editorconfig`

Permet d'imposer des règles de formatage cohérentes (indentation, encodage, fin de ligne) quel que soit l'éditeur utilisé par les contributeurs du projet.

```ini
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true
```

## Nodemon (bonus)

Nodemon est un outil qui redémarre automatiquement une application Node.js à chaque modification de fichier, évitant de devoir relancer le serveur manuellement pendant le développement.

```bash
npm install --save-dev nodemon
```

Dans `package.json` :
```json
"scripts": {
  "dev": "nodemon"
}
```

## Ce que j'ai retenu

- La configuration globale de Git (`--global`) s'applique à tous les projets, alors qu'une configuration locale ne s'applique qu'au projet courant.
- Un `.gitignore` mal configuré peut faire fuiter des informations sensibles (mots de passe, clés API) si elles sont accidentellement commit.
- Structurer un projet proprement dès le premier commit facilite grandement la suite du développement.
