# create_projet
tapes principales :
Récupération des informations du Deal :


Préparation des paramètres du projet :


Récupération du modèle de projet :

Recherche du modèle nommé "Modèle de projet" parmi les projets templates existants dans Zoho Projects.

Création du projet :

Si le modèle est trouvé, un nouveau projet est créé via l’API Zoho Projects avec les paramètres précédemment définis.

Mise à jour du Deal dans Zoho CRM :

L'ID du projet nouvellement créé est sauvegardé dans le champ personnalisé Project_ID du Deal.

Association du projet au Deal :

Le projet est associé au Deal via l'API de liaison entre Zoho CRM et Zoho Projects.
