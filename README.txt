DYNAMOS HOCKEY STATS — VERSION 1.8 BÊTA

Installation / mise à jour GitHub Pages
- Remplacer les fichiers de la version précédente par ceux de ce dossier.
- Conserver le même dépôt et le même chemin GitHub Pages.
- Recharger l’application. Si une ancienne version demeure affichée, fermer puis rouvrir l’application pour actualiser le cache.

Données
- Les données locales et la synchronisation Google Drive utilisent les mêmes clés que les versions précédentes.
- Avant la mise à jour, exporter une sauvegarde JSON depuis l’onglet Sauvegarde.
- Ne pas effacer les données du navigateur ou le stockage du site.

Version 1.8 BÊTA
- Totaux joueurs et gardiens, avec pourcentages recalculés à partir des totaux.
- Pourcentage de mises au jeu et de tirs cadrés par joueur.
- Carte des tirs filtrable par joueur depuis le sommaire du match ou les statistiques.
- Boutons d’enregistrement à plusieurs endroits.
- Gravité obligatoire pour chaque tentative de tir, sans valeur présélectionnée.
- Tri des listes de joueurs par numéro.
- Modification étendue des événements.
- Affichage visiteur à gauche et local à droite.
- Conservation de la synchronisation Google Drive.

BÊTA : valider les calculs et les saisies avec des données de test avant une utilisation officielle.


VERSION 1.8 BÊTA — CORRECTION GOOGLE DRIVE
- Correction du chargement de Google Identity Services lorsqu’un script existe déjà.
- Délai maximal de chargement et messages d’erreur explicites.
- Tentative de restauration silencieuse de l’autorisation Google à l’ouverture, si le compte a déjà été connecté.
- Si Google exige une interaction, utiliser le bouton « Connecter Google Drive ».
- Aucun jeton d’accès Google n’est enregistré dans le stockage local.
