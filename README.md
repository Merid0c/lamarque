# 🏐 La Marque

**La table de marque de poche pour le volley.** Une application web gratuite, libre et sans compte, pour suivre un match depuis le bord du terrain, garder l'historique de ses équipes et analyser sa saison.

*Version 2.4 · Licence MIT · Fonctionne hors connexion · Aucune donnée n'est envoyée sur Internet*

## En un coup d'œil

| | |
|---|---|
| ⏱ **Score en direct** | Un appui = +1 point, glisser vers le bas = annuler. Affichage horizontal pour les joueurs, chronomètre, durée de chaque set |
| 🎯 **Mode avancé** | Qualifie chaque point (ace, attaque, bidouille, bloc, fautes…), activable ou désactivable en plein match |
| 📜 **Historique** | Chaque match avec son déroulé point par point, ses séries, une notation en étoiles et des notes |
| 📈 **Saison** | Victoires, sets, Points championnat, courbes, frise des derniers matchs, statistiques par type de point |
| 🖼 **Fiche de match** | Image A4 à partager (WhatsApp, Discord…) avec camemberts, déroulé des sets et photo facultative |
| 👥 **Staff** | Partage et fusion des données entre collègues, sans jamais écraser les données de l'autre |
| 💾 **Sauvegarde** | Fichier .json versionné à garder sur un drive, restauration complète en un geste |

## Fonctionnalités

### Table de marque
- Un appui sur une zone de couleur = +1 point, glissement vers le bas = annuler le dernier point
- Affichage horizontal « table de marque », écran maintenu allumé, mode « plein soleil » à fort contraste
- Sets, changement de côté, set décisif, règles personnalisables (FFVolley, loisir, ou à la carte pour chaque match)
- Chronomètre du match en haut de l'écran et durée de chaque set
- Mode avancé : qualification de chaque point, activable ou désactivable en cours de match
- Notes pendant les temps morts, écrites ou dictées
- Mise en pause d'un match et reprise plus tard, vibration à chaque point (Android)
- Matchs interrompus (départage à la différence de points), forfaits, entraînements hors championnat
- Rappel du dernier résultat contre l'adversaire quand on prépare une rencontre retour

### Historique
- Liste des matchs, modification, saisie d'un match non suivi
- Déroulé point par point de chaque set, séries max de chaque équipe
- « Lecture rapide » : point fort, point faible, plus longue série
- Notation du match (1 à 5 étoiles) et commentaire facultatifs
- Fiche de match A4 à partager en image, photo facultative (non conservée dans l'application)

### Saison
- Victoires, sets, Points championnat : 3 pour une victoire, 2 pour une défaite avec 2 sets marqués, 1 pour une défaite, 0 pour un forfait
- Courbes d'évolution, frise des derniers matchs, statistiques par type de point (en pourcentage)
- Export CSV

### Équipes et données
- Plusieurs équipes, duplication, réinitialisation, suppression
- Partage et fusion des données entre membres du staff, par code ou par fichier
- Sauvegarde et restauration par fichier .json versionné (version et date dans le nom), ou par texte
- Format de données versionné, avec reprise des anciennes sauvegardes
- Message d'accueil, tutoriel (à revoir dans Réglages) et équipe d'exemple
- Fonctionne hors connexion une fois installée

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

1. Sur l'ancienne version : **Réglages → Sauvegarde → Télécharger ma sauvegarde (.json)** (ou, pour une très ancienne version, copie le texte de sauvegarde).
2. Sur la nouvelle version : **Réglages → Restaurer depuis un fichier**, choisis le fichier et confirme. Le texte copié se colle dans « Sauvegarde par texte ».

Fais une sauvegarde de temps en temps : si tu vides les données du navigateur, elles sont perdues.

## Partager avec un collègue du staff

Dans **Réglages → Partager avec mon staff**, choisis une ou plusieurs équipes (et, si tu veux, seulement les 5 ou 10 derniers matchs), puis **Créer le code**. Envoie-le par message avec **Partager**, ou en fichier avec **Envoyer en fichier**.

Ton collègue va dans **Réglages → Recevoir un code**, colle le message (ou choisit le fichier) et touche **Lire le code** : il voit un résumé (nouveaux matchs, mis à jour, déjà présents), puis **Fusionner**. Ses autres équipes et ses autres matchs restent intacts. Un bouton **Annuler la dernière fusion** permet de revenir en arrière.

Règles : les équipes sont reconnues par leur nom ; un match déjà présent n'est jamais dupliqué (si les deux versions ont été modifiées, la plus récente gagne) ; un match supprimé sur un téléphone n'est pas supprimé sur l'autre. Les matchs en cours ne sont pas transférés.

## Licence

Licence MIT : tu peux utiliser, copier, modifier et partager cette application librement, y compris pour un usage commercial. Pour un don au domaine public, remplace le fichier LICENSE par le texte CC0 1.0 (creativecommons.org/publicdomain/zero/1.0/).

## Crédits

Le ballon de l'icône est l'émoji 🏐 de la police **Noto Color Emoji** (Google), distribuée sous licence SIL Open Font License 1.1 : https://github.com/googlefonts/noto-emoji
