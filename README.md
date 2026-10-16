# 🏐 La Marque

**La table de marque de poche pour le volley.** Une application web gratuite, libre et sans compte, pour suivre un match depuis le bord du terrain, garder l'historique de ses équipes et analyser sa saison.

*Version 2.5 · Licence MIT · Fonctionne hors connexion · Aucune donnée n'est envoyée sur Internet*

## En un coup d'œil

| | |
|---|---|
| ⏱ **Score en direct** | Un appui = +1 point, glisser vers le bas = annuler. Affichage horizontal pour les joueurs, chronomètre, durée de chaque set |
| 🎯 **Mode avancé** | Qualifie chaque point (ace, attaque, bidouille, bloc, fautes…), activable ou désactivable en plein match |
| 🏐 **Mode analyse (optionnel)** | Liste des joueurs par équipe (onglet Équipe), choix des présents, puis analyse de la réception (parfaite / bonne / jouable / zippée puis manchette ou dix doigts, terrain en losange, changement de joueur, moyennes en direct, bilan dans l'historique). Désactivé, l'application reste simple |
| 🟨 **Mode arbitre / Mode coach** | Arbitre : table de marque seule, écran paysage automatique, score visible des joueurs. Coach : écran d'options (points, réception, passes, deux observateurs) |
| 👥 **Analyse à deux observateurs** | Un téléphone tient la table et qualifie les points ; un second, rejoint avec un code d'invitation (équipe, joueurs, match), note la réception et la répartition des passes (en 4, en 3, en 2). À la fin, son code d'analyse s'intègre au match du premier téléphone |
| 📜 **Historique** | Chaque match avec son déroulé point par point, ses séries, une notation en étoiles et des notes |
| 📈 **Saison** | Victoires, sets, Points championnat, courbes, frise des derniers matchs, statistiques par type de point |
| 🖼 **Fiche de match** | Image A4 à partager (WhatsApp, Discord…) avec camemberts, déroulé des sets et photo facultative |
| 👥 **Staff** | Partage et fusion des données entre collègues, sans jamais écraser les données de l'autre |
| 💾 **Sauvegarde** | Fichier .json versionné à garder sur un drive, restauration complète en un geste |

## Nouveautés de la version 2.5

### Deux façons de lancer un match
La page **Match** est simplifiée : adversaire, date, lieu, compétition (remplie automatiquement avec la catégorie et la saison de l'équipe), couleurs, règles repliables, puis deux gros boutons.
- **Mode arbitre** : la table de marque seule. L'écran se met en paysage tout seul (un bouton « Inverser le sens de l'écran » est dans le menu), idéal pour montrer le score aux joueurs.
- **Mode coach** : ouvre un écran avec de grandes tuiles carrées pour choisir l'analyse du match : aucune, qualifier les points, réception, passes, ou analyse à deux observateurs. Plus d'interrupteur « Mode analyse » caché dans les réglages : tout se choisit match par match.

### Réception sur 4 niveaux
La réception se note maintenant **parfaite / bonne / jouable / zippée**, puis **manchette ou dix doigts**. Le type de service adverse est retiré pour alléger la prise de notes. Le bilan (en direct, dans l'historique et sur la fiche A4) affiche la moyenne sur 3, le pourcentage de réceptions parfaites, et à la fin les **pourcentages manchette / dix doigts**.
> Tes anciennes analyses sont converties automatiquement : l'ancien « jouable » reste « jouable » dans la nouvelle échelle (les moyennes anciennes baissent légèrement).

### Module « passes »
Un module indépendant de la réception, pour noter la répartition des passes **en 4, en 3 et en 2**. Il n'est pas nécessaire de toutes les noter : ce sont des proportions. Utilisable seul (mode coach) ou en même temps que la réception.

### Analyse à deux observateurs
Un téléphone tient la table et qualifie les points ; un second observateur note la réception et les passes.
- Le premier téléphone crée un **code d'invitation** (équipe, joueurs, adversaire, compétition, règles). Le second le colle dans **Match → Rejoindre comme observateur** : le match se lance tout seul.
- L'écran de l'observateur rappelle le match (équipes, compétition, règles) et le **score des sets**, qui suit le « Set + » (avec choix de l'équipe gagnante) et le « − Set ».
- À la fin, un écran de fin de match propose un seul bouton **Copier le code** à envoyer au premier téléphone, qui l'intègre au match terminé (« Intégrer l'analyse »).
- Le second téléphone retrouve ses matchs observés, en bleu, dans **Historique → Matchs observés**, avec le code à renvoyer et la possibilité de supprimer (avec confirmation).

### Points qualifiés par set
Quand on qualifie les points seulement sur certains sets, l'application le sait : « Set #2 évalué », « Sets #2 et #4 évalués ». Les statistiques de saison portent sur le pourcentage de points qualifiés.

### Fiche de match A4 repensée
- Panneau de points qualifiés à gauche, réception et passes à droite ; si un seul module est utilisé, il occupe toute la largeur.
- Le set analysé est indiqué sur chaque panneau, la photo facultative est mise en valeur avec l'icône 📸.
- La « Lecture rapide » n'est plus sur la fiche (elle reste dans le détail du match).

### Un onglet Équipe, des réglages allégés
- **Équipe** : mes équipes, profil, joueurs, règles par défaut (repliables), partage avec le staff et réception d'un code.
- **Réglages** : apparence, vibration, sauvegarde et restauration.
- Un **rappel de sauvegarde** apparaît désormais en fenêtre au milieu de l'écran, de façon rare (après une semaine d'usage, ou si la dernière sauvegarde a plus de 7 jours).
- « Saisir un match non suivi » n'est plus que dans l'Historique.

### Mettre à jour
Remplace simplement `index.html` dans ton dépôt (voir plus bas). Tes données ne bougent pas : le format de sauvegarde est inchangé. Fais une sauvegarde avant, par précaution.

## Fonctionnalités

### Table de marque
- Un appui sur une zone de couleur = +1 point, glissement vers le bas = annuler le dernier point
- Affichage horizontal « table de marque », écran maintenu allumé, mode « plein soleil » à fort contraste
- Sets, changement de côté, set décisif, règles personnalisables (FFVolley, loisir, ou à la carte pour chaque match)
- Chronomètre du match en haut de l'écran et durée de chaque set
- Mode avancé : qualification de chaque point, activable ou désactivable en cours de match
- Analyse de la réception : parfaite / bonne / jouable / zippée, manchette ou dix doigts, stats par joueur
- Module passes (en 4, en 3, en 2), seul ou avec la réception, et analyse à deux observateurs
- Notes pendant les temps morts, écrites ou dictées
- Mise en pause d'un match et reprise plus tard, vibration à chaque point (Android)
- Matchs interrompus (départage à la différence de points), forfaits, entraînements hors championnat
- Rappel du dernier résultat contre l'adversaire quand on prépare une rencontre retour

### Historique
- Liste des matchs, modification, saisie d'un match non suivi
- Matchs observés (en tant que second observateur), avec le code à renvoyer
- Déroulé point par point de chaque set, séries max de chaque équipe
- « Lecture rapide » dans le détail du match : point fort, point faible, plus longue série
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

Dans **Équipe → Partager avec mon staff**, choisis une ou plusieurs équipes (et, si tu veux, seulement les 5 ou 10 derniers matchs), puis **Créer le code**. Envoie-le par message avec **Partager**, ou en fichier avec **Envoyer en fichier**.

Ton collègue va dans **Équipe → Recevoir un code**, colle le message (ou choisit le fichier) et touche **Lire le code** : il voit un résumé (nouveaux matchs, mis à jour, déjà présents), puis **Fusionner**. Ses autres équipes et ses autres matchs restent intacts. Un bouton **Annuler la dernière fusion** permet de revenir en arrière.

Règles : les équipes sont reconnues par leur nom ; un match déjà présent n'est jamais dupliqué (si les deux versions ont été modifiées, la plus récente gagne) ; un match supprimé sur un téléphone n'est pas supprimé sur l'autre. Les matchs en cours ne sont pas transférés.

## Licence

Licence MIT : tu peux utiliser, copier, modifier et partager cette application librement, y compris pour un usage commercial. Pour un don au domaine public, remplace le fichier LICENSE par le texte CC0 1.0 (creativecommons.org/publicdomain/zero/1.0/).

## Crédits

Le ballon de l'icône est l'émoji 🏐 de la police **Noto Color Emoji** (Google), distribuée sous licence SIL Open Font License 1.1 : https://github.com/googlefonts/noto-emoji
