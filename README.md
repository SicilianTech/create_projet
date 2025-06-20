# create_projet
tapes principales :
Récupération des informations du Deal :

Nom du compte, ID, contact associé, montant, description, adresse des travaux, fiche technique, etc.

Le contact associé est utilisé pour extraire le numéro de téléphone mobile.

Calcul du budget de coût (cost_budget) :

Basé sur le montant total (Amount) et le pourcentage de profit brut (Pourcentage_profit_brut_vis_proposition_de_Oli).

Formule : coût cible = montant du deal - (montant du deal * % profit)

Préparation des paramètres du projet :

name, description, budget_value, revenue_budget, hourly_budget, UDF_XXX pour les champs personnalisés (ex. : fiche technique, couleur).

Récupération du modèle de projet :

Recherche du modèle nommé "Modèle de projet" parmi les projets templates existants dans Zoho Projects.

Création du projet :

Si le modèle est trouvé, un nouveau projet est créé via l’API Zoho Projects avec les paramètres précédemment définis.

Mise à jour du Deal dans Zoho CRM :

L'ID du projet nouvellement créé est sauvegardé dans le champ personnalisé Project_ID du Deal.

Association du projet au Deal :

Le projet est associé au Deal via l'API de liaison entre Zoho CRM et Zoho Projects.
