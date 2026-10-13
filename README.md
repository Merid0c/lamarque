# 🏐 La Marque

Application web mobile (PWA) gratuite et libre pour suivre les matchs de volley depuis le bord du terrain.

- Score en direct : un appui sur une zone de couleur = +1 point, glissement vers le bas = annuler le dernier point
- Affichage horizontal « table de marque » pour les joueurs
- Sets, changement de côté, matchs interrompus, forfaits, entraînements
- Historique, modification des matchs, statistiques de saison, classement à points
- Plusieurs équipes, export CSV, sauvegarde et restauration des données
- Fonctionne hors connexion une fois installée

Les données restent **sur le téléphone** (dans le navigateur) : rien n'est envoyé sur Internet.

## Utiliser l'application

Ouvre l'adresse du site (voir plus bas), puis installe-la :

- **Android (Chrome)** : menu ⋮ → « Installer l'application » ou « Ajouter à l'écran d'accueil ».
- **iPhone (Safari)** : bouton Partager → « Sur l'écran d'accueil ».

> iPhone : l'application installée a son propre espace de stockage, séparé de Safari. Fais ta restauration de données **depuis l'application installée**.

## Publier ta propre copie (GitHub Pages)

1. Crée un compte gratuit sur github.com.
2. Clique sur **New repository**, nomme-le `lamarque`, laisse-le **Public**, puis **Create repository**.
3. Clique sur **uploading an existing file**, glisse **tous les fichiers de ce dossier** (index.html, manifest.json, sw.js, les 3 images, LICENSE, README.md), puis **Commit changes**.
4. Va dans **Settings → Pages**. Dans « Build and deployment », choisis **Deploy from a branch**, la branche **main**, le dossier **/ (root)**, puis **Save**.
5. Attends 1 à 2 minutes. Ton application est en ligne à l'adresse `https://TON-PSEUDO.github.io/lamarque/`.

Pour mettre à jour l'application plus tard : dans le dépôt, ouvre `index.html`, clique sur le crayon ✏️, remplace le contenu, puis **Commit changes**.

## Reprendre tes données d'une ancienne version

1. Sur l'ancienne version : **Réglages → Sauvegarde → Afficher ma sauvegarde → Copier la sauvegarde**. Colle-la dans un mail ou une note.
2. Sur la nouvelle version : **Réglages → Restaurer depuis une sauvegarde**, colle le texte, touche **Restaurer** et confirme.

Fais une sauvegarde de temps en temps : si tu vides les données du navigateur, elles sont perdues.

## Licence

Licence MIT : tu peux utiliser, copier, modifier et partager cette application librement, y compris pour un usage commercial. Pour un don au domaine public, remplace le fichier LICENSE par le texte CC0 1.0 (creativecommons.org/publicdomain/zero/1.0/).
