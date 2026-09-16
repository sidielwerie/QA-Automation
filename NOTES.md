# Mes notes — Apprentissage QA Automatisation

## Terminal — navigation de base
- `pwd` → affiche le dossier où je suis actuellement
- `ls` → liste le contenu du dossier actuel
- `cd nom-dossier` → entre dans un dossier
- `cd ..` → remonte d'un niveau
- `cd ~` → retourne à mon dossier personnel

## Création de projet
- `mkdir nom-dossier` → crée un nouveau dossier
- `git init` → transforme le dossier actuel en dépôt Git (active le suivi de versions)

## Homebrew (gestionnaire de paquets Mac)
- `brew --version` → vérifie si Homebrew est installé
- `brew install nom-outil` → installe un outil en ligne de commande
- `brew install --cask nom-app` → installe une application avec interface graphique (ex: VS Code)

## VS Code
- `code --version` → vérifie que VS Code est installé et accessible en ligne de commande
- `code .` → ouvre le dossier actuel dans VS Code

## Node.js et nvm
- `nvm --version` → vérifie que nvm est installé
- `nvm install --lts` → installe la dernière version stable (LTS) de Node.js
- `nvm use --lts` → active cette version
- `node --version` → vérifie la version de Node active
- `npm --version` → vérifie la version de npm (gestionnaire de librairies JavaScript)

## Playwright
- `npm init playwright@latest` → crée un nouveau projet de tests Playwright
- `npx playwright test` → lance tous les tests
- `npx playwright show-report` → ouvre le rapport HTML du dernier lancement de tests

## Git — sauvegarder son travail
- `git status` → montre l'état des fichiers (modifiés, non suivis, etc.)
- `git add .` → prépare tous les fichiers modifiés pour la prochaine sauvegarde
- `git commit -m "message"` → crée une sauvegarde (un "commit") avec un message explicatif
- `git log` → affiche l'historique des commits
- `git config --global user.name "Nom"` → configure le nom associé à mes commits
- `git config --global user.email "email"` → configure l'email associé à mes commits
- `git commit --amend --reset-author --no-edit` → corrige l'auteur d'un commit déjà fait

## Concepts clés
- **Git** = outil local de gestion de versions (pas de site web)
- **GitHub** = site web qui héberge des projets Git en ligne, pour partager/sauvegarder/collaborer
- **Chromium** = version open source sur laquelle Chrome est basé, utilisée par Playwright pour l'automatisation
- **Auto-waiting** = Playwright attend automatiquement qu'un élément soit prêt avant d'agir dessus (contrairement à Selenium qui demande des attentes explicites)
- **.gitignore** = fichier qui liste ce que Git doit ignorer (ex: node_modules, trop volumineux et régénérable)