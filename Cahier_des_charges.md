## 1. **Introduction**

Ce document décrit le cahier des charges du projet Heimdall. Ce cahier des charges est destiné à la compréhension des fonctionnalités implémentées lors de la conception et du développement de ce projet.

## 2. **Cahier des charges**

Front-End (Mobile):

- Choix du serveur à l&#39;installation de l&#39;application
- Se connecter en tant qu&#39;étudiant

  - Liste de toute ses absences (à justifier, validée ou refusée)
  - Accès aux absences à justifier ou refusées
    - Accède à l&#39;absence où il peut justifier en envoyant un fichier (photo) et choisir le type de justificatif (transport, famille, malade, autre)

- Se connecter en tant que professeur
  - Accès à la liste des émargements effectuées
  - Créer un nouvel émargement

  - Choix d&#39;un groupe via une liste déroulante
    - Affichage des élèves du groupe sous forme de liste (avec photo)
    - Renseigner les absences et retards des élèves (par défaut tous les élèves sont notés présents)
    - Valider la liste

Front-End (Application web) : cette application est utilisée seulement par le gestionnaire

- Définissable par une zone admin où :
  - CRUD groupe (classe)
  - CRUD utilisateur (professeur, étudiant)

- Accéder à la liste des émargements pour un groupe
  - Accéder à un élève et visualiser ses absences et justificatif
  - Valider ou Refuser un justificatif



Back-End :

- --Notifier l&#39;étudiant (notification mobile) qu&#39;il est noté absent par un professeur dans un cours (deuxième validation après récapitulatif)

- --A la fin de la journée envoyer un mail avec un fichier récapitulatif des émargements de la journée à un mail paramétrable
