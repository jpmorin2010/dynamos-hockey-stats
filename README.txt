# Dynamos Hockey Stats — Prototype 1.0

## Démarrage rapide
1. Décompressez le dossier.
2. Pour tester sur ordinateur, servez le dossier avec un petit serveur local (ex. `python -m http.server 8000`) puis ouvrez `http://localhost:8000`.
3. Pour installer sur Android et activer le mode hors ligne, hébergez les fichiers en HTTPS (GitHub Pages convient), ouvrez l'adresse dans Chrome, puis menu ⋮ > Ajouter à l'écran d'accueil / Installer l'application.

## Première utilisation
- Ouvrez **Équipes & joueurs** et ajoutez vos équipes et joueurs avec leurs numéros.
- Revenez à **Match**, choisissez l'équipe suivie et l'adversaire.
- Pour un tir ou un but, sélectionnez le joueur puis touchez la patinoire pour placer le tir.
- Pour un but, choisissez la force de jeu et cochez les joueurs sur la glace avant d'enregistrer.
- Dans **Statistiques**, choisissez l'équipe pour consulter les chiffres du match.
- Dans **Sauvegarde**, exportez régulièrement le JSON.

## Limites connues de ce prototype
- Les données sont conservées dans le navigateur de cet appareil. Exportez souvent une sauvegarde JSON.
- Les statistiques de +/- reposent sur les joueurs cochés manuellement sur la glace au moment du but. Les buts en avantage numérique sont exclus; buts à égalité et en désavantage numérique sont comptés.
- Les gardiens et les changements de joueurs sont saisis comme événements/présences, mais le suivi automatique du temps de glace, des tirs contre et du pourcentage d'arrêts n'est pas encore implémenté.
- Le CSV est un export des événements; l'export Excel formaté et les rapports de saison sont prévus pour une version suivante.
- Il s'agit d'un prototype, pas encore d'une application publiée sur Google Play.

## xG (buts attendus)
Pour chaque tir (cadré, but, manqué ou bloqué), choisissez le niveau de danger : faible = 0,1; moyen = 0,2; élevé = 0,3. La valeur est ajoutée au xG du joueur et de l'équipe. Ce modèle est un indice simplifié défini par l'utilisateur, et non un modèle statistique professionnel entraîné sur des données historiques.

## Statistiques des gardiens — version 1.2
Lors de l'enregistrement d'un tir cadré ou d'un but, sélectionnez le gardien de l'équipe qui défend. Dans l'onglet Statistiques de cette équipe, le tableau des gardiens affiche tirs contre, arrêts, buts alloués, SV%, xGA et l'écart xGA − buts alloués. Les tirs manqués et bloqués ne comptent pas comme tirs cadrés contre. Le xGA est calculé avec le barème simplifié faible/moyen/élevé.
