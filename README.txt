DYNAMOS HOCKEY STATS - VERSION 1.9 BETA

Correctif de connexion Google Drive :
- Google Identity Services est préchargé pendant l'ouverture de l'application.
- Le bouton de connexion appelle directement la demande OAuth dans le geste utilisateur, sans await préalable, afin d'éviter le blocage de la fenêtre Google sur Android/Chrome.
- Si la bibliothèque n'est pas encore prête au premier clic, l'application indique qu'elle est prête et demande un second clic.
- La reconnexion silencieuse à l'ouverture est conservée lorsque Google permet de rétablir l'accès.

Installation : remplacer les fichiers du dépôt GitHub Pages avec le contenu de ce dossier.
Avant l'installation, exporter une sauvegarde JSON des données locales.
