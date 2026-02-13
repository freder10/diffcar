Problème

Lors de la modification d’une offre bonus, lorsque l’on envoie une liste vide pour les opérations ou les fonds liés, la modification n’est pas prise en compte côté projet CSERVICES.

Étapes pour reproduire

Créer ou modifier une offre bonus avec au moins une opération ou un fonds associé.

Supprimer tous les éléments (opérations ou fonds) depuis le frontend.

Sauvegarder la modification (envoi d’une liste vide [] au backend).

Résultat actuel

La modification n’est pas appliquée : les opérations ou fonds précédemment associés restent persistés.
Côté frontend, cela donne l’impression qu’il est impossible de supprimer le dernier élément de la liste.

Résultat attendu

L’envoi d’une liste vide ([]) devrait être interprété comme une demande de suppression de tous les éléments associés (opérations ou fonds) à l’offre bonus.
