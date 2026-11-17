DYNAMOS HOCKEY STATS — VERSION 1.9.1 BÊTA

Correctif ciblé Google Drive :
- Version affichée dans l’en-tête.
- Suppression de la tentative OAuth automatique au chargement : le flux Google doit être déclenché par un clic réel.
- La demande d’autorisation ne force plus le consentement à chaque tentative.
- Diagnostic distinct du retour OAuth et de l’accès à l’API Drive.
- Les données locales ne sont pas modifiées par un échec d’autorisation.

Installation : remplacer les fichiers du dépôt GitHub Pages par le contenu de ce dossier.
Faire une sauvegarde JSON avant la mise à jour.

Limite : cette version ne peut pas corriger la configuration du projet Google Cloud. Si Google refuse le compte, vérifier que le compte utilisé est inscrit dans Audience > Test users du projet OAuth, et que Google Drive API est activée.
