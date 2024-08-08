# ocr-3

Contexte:

CodeIguanas est une entreprise de service numérique divisé en plusieurs pôles de développement web et mobile.

Je suis employé chez eux en tant que lead dev d'une équipe de l'entité web, composée de 4 développeurs (2 front, 2 back). L'équipe de développement est comptétente sur les technos actuelles. Aucune formation ne leurs est requise pour ce projet.

Mon équipe est moi même nous sommes vu attribuer une mission pour HomeSkolar, une association metant en relation des élève en difficulté scolaire avec des tuteurs bénévole. Un élève à un tuteur et vice versa.
L'application est international.
L'élève et le tuteurs ont des rendez-vous courts (visio) chaque semaine.
Durant ses rendez-vous le tuteurs aide l'élève pour ses devoirs.

Thomas est mon responsable chez CodeIguanas.

Mission pour HomeSkolar:

- Developper from scratch la plateforme web de mise en relation entre tuteurs et élèves.
- Mon rôle: Cadrer les équipes et coordonner l'équipe de développement.
- Définir les besoins client

ETAPE 1 : Création du cahier des charge contennant les éléments suivant:

- Une liste des spécifications fonctionnelles présentant ce que le produit va réaliser.

* Authentification pour les tuteurs et élèves:
  _ Inscription
  _ Connexion
  _ Gestion du mot de passe
  _ Gestion des donnèes personnelles

* Communication (Messagerie):
  _ Echange de messages
  _ Epingler des messages

* Calendrier
  _ Affichage des rendez vous de l'utilisateur
  _ Affichage des évènements de l'utilisateur

* Todo
  _ Liste de tâches à réaliser pour les élèves à la suite de leurs rendez vous avec leurs tuteurs (les tuteurs crée des tâches pour les élèves)
  _ Notification des tâches
  \_ Les utilisateurs doivent pouvoir se créer des tâches à eux mêmes

- Une veille technologique justifiant des choix technologique adopté dans la spécification technique.

- Une liste des spécifications techniques, qui présentera les technologies utilisées et comment la technique répond au besoin client.

- Un diagramme de classe utilisant la nomenclature UML

ETAPE 2 : Création d'un backlog Produit sur Notion, contenant toute les tâche liées au produit:

- Des users story priorisées avec critères d'acceptation

- Une estimation du temps de réalisation (Jour homme?)

ETAPE 3, Créer une présentation PowerPoint d'une slide minimum pour chaque sujet suivant:

- Context du projet
- Fonctionnalité
- Choix technique

* REDACTION DE LA SECTION "Spécifications fonctionelles" DU CAHIER DES CHARGES :

1. Introduction
   Le projet HomeSkolar a pour objectif de créer une plateforme web permettant de mettre en relation des enfants en difficulté scolaire avec des tuteurs bénévoles. Le site web doit être convivial, intuitif et répondre aux besoins spécifiques de HomeSkolar pour faciliter le tutorat scolaire en ligne.

2 Fonctionnalités principales:

INSCRIPTION
Objectif: Permettre aux utilisateurs (élèves et tuteurs) se s'inscrire à la plateforme.

Fonctionnalité:

- Page d'inscription avec les champs suivant: nom, prénom, adresse email, mot de passe, rôle (élève ou tuteur).

AUTHENTIFICATION:
Objectif: Permettre aux utilisateurs (élèves et tuteurs) se s'inscrire à la plateforme.

Fonctionnalité:

- Page de connexion avec les champs "adresse email" et "mot de passe"

MODIFICATION DE MOT DE PASSE:
Objectif: Permettre aux utilisateurs de modifier leurs mot de passe

Fonctionnalités:

- L'utilisateur peut demander la réinitialisation de son mot de passe en entrant son adresse email
- Un lien de réinitialisation est envoyé à l'utilisateur par e-mail
- L'utilisateur clique sur le lien, accède à une page de réinitalisation et entre un nouveau mot de passe valide selon les règles syntaxiques mise en place.

GESTION DE PROFIL:

- Objectif: Permettre aux utilisateurs de gérer leurs compte et de mettre à jour leurs informations personnelles.

Fonctionnalités:

- Posibilité de se deconnecter de son compte.
- Possibilité d'afficher les informations personnelles de l'utilisateurs.
- Possiblité de modifier les informations personnelles (adresse email, mot de passe, description personnelle).

COMMUNICATION:
Objectif: Permette les échanges entre les élèves et les tuteurs depuis la plateforme

fonctionnalités:

- Système de messagerie intégré permettant l'envoi et la récéption de messages.
- Possibilité d'épingler des messages importants pour un accès facile ultérieur
- Notification pour les messages non lus

PLANIFICATION DES RENCONTRE ÉLÈVE TUTEURS
Objectif : Permettre la planification et la gestion des rendez-vous entre élèves et tuteurs

Fonctionnalité:

- Page de calendrier affichant les évènement et rendez-vous de l'utilisateur
- Possibilité pour les tuteurs de créer et de planifier des sessions de tutorat avec date, heure et description
- Possibilité pour les élève de visualiser leur emploi du temps sur le calendrier
- Possibilité pour les tuteurs uniquement de modifier un rendez-vous (annulation ou modification de date/heure)

GESTION DES TACHES:
Objectif: Creation et sivit des taches à réaliser pour les élèves et tuteurs.

Fonctionnalité:

- Les tuteurs peuvent créer des tâches et les attribuer à leurs élèves
- Les utilisateurs peuvent se créer des taches personnelles
- Notification pour les nouvelles taches assignées par les tuteurs au élèves.

SPECIFICATIONS TECHNIQUES:

1. Introduction
   Le projet HomeSkolar a pour objectif de créer une plateforme web facilitant le tutorat scolaire en ligne. Les spécifications techniques détaillées ci-dessous permettent de guider le développement et la maintenance de cette plateforme.

2. Fonctionnalités Techniques
   INSCRIPTION
   Objectif : Permettre aux utilisateurs (élèves et tuteurs) de s'inscrire à la plateforme.

Backend :

Endpoints API : Création de comptes utilisateur avec validation des données.
Base de données : Stockage sécurisé des informations utilisateur.
Frontend :

Formulaire d'inscription avec validation côté client.
AUTHENTIFICATION
Objectif : Permettre aux utilisateurs de se connecter à la plateforme.

Backend :

Endpoints API : Authentification des utilisateurs avec génération de JWT.
Sécurité : Chiffrement des mots de passe.
Frontend :

Formulaire de connexion avec gestion des tokens JWT pour maintenir la session utilisateur.
MODIFICATION DE MOT DE PASSE
Objectif : Permettre aux utilisateurs de modifier leur mot de passe.

Backend :

Endpoints API : Réinitialisation des mots de passe avec envoi de lien par email.
Frontend :

Formulaire de réinitialisation de mot de passe avec validation des champs.
GESTION DE PROFIL
Objectif : Permettre aux utilisateurs de gérer leur compte et de mettre à jour leurs informations personnelles.

Backend :

Endpoints API : Récupération et mise à jour des informations de profil.
Frontend :

Interface de gestion de profil pour afficher et modifier les informations personnelles.
COMMUNICATION
Objectif : Permettre les échanges entre les élèves et les tuteurs depuis la plateforme.

Backend :

Endpoints API : Gestion des messages.
WebSockets : Communication en temps réel.
Frontend :

Interface de messagerie avec support pour épingler des messages et notifications pour les nouveaux messages.
PLANIFICATION DES RENCONTRES ÉLÈVE-TUTEUR
Objectif : Permettre la planification et la gestion des rendez-vous entre élèves et tuteurs.

Backend :

Endpoints API : Création, récupération et modification des événements de calendrier.
Frontend :

Interface de planification avec vue calendrier interactive.
GESTION DES TÂCHES
Objectif : Création et suivi des tâches à réaliser pour les élèves et tuteurs.

Backend :

Endpoints API : Gestion des tâches avec création et mise à jour des tâches.
Frontend :

Interface de gestion des tâches pour afficher, créer et mettre à jour les tâches.

1. Simplicité et Synergie des Technologies
   a. JavaScript Universel (Node.js)
   Le fait que Node.js utilise JavaScript, tout comme React pour le front-end, offre une grande cohérence dans le développement. Les développeurs peuvent ainsi utiliser un seul langage de programmation sur toute la pile technologique, ce qui simplifie l'apprentissage et réduit les contextes de switch entre différents langages.

b. Express.js - Simplification du Serveur
Express.js est un framework minimaliste pour Node.js qui facilite la création de serveurs web. Sa simplicité et flexibilité permettent de développer des applications robustes avec moins de code et plus d'efficacité, grâce à un riche écosystème de middleware pour répondre à divers besoins de l'application.

c. MongoDB - Flexibilité des Données
MongoDB est une base de données NoSQL qui offre une grande flexibilité dans la gestion des données. Elle permet une scalabilité horizontale et est conçue pour gérer de grands volumes de données de manière efficace, avec un schéma dynamique qui est idéal pour les applications modernes qui nécessitent une évolution rapide.

d. ReactJS - Composants et Hooks
ReactJS favorise la maintenabilité et la scalabilité grâce à son système de composants réutilisables et son modèle de hooks. Ces derniers permettent de gérer l'état et le cycle de vie des composants de manière plus intuitive et fonctionnelle, rendant le code plus lisible et plus facile à maintenir.

2. Communauté Solide et Ressources Abondantes
   Le stack MERN bénéficie d'une communauté très active et engagée. Que ce soit sur GitHub, Stack Overflow, ou d'autres forums spécialisés, il est facile de trouver de l'aide et de partager des connaissances.

Développeurs et contributeurs : Les projets sous-jacents sont maintenus par des milliers de développeurs.
Ressources éducatives : Il existe de nombreux cours, tutoriels, et guides pratiques qui couvrent chaque technologie du stack MERN.
Documentation à jour : Chaque technologie du stack MERN dispose d'une documentation officielle complète, régulièrement mise à jour, avec des guides de démarrage rapide, des références API, et des exemples de code. 3. Documentation de Qualité
La qualité de la documentation est cruciale pour l'apprentissage et l'utilisation efficace de nouvelles technologies. MongoDB, Express, ReactJS, et NodeJS offrent toutes des documentations bien organisées, claires et détaillées. Elles incluent des tutoriels pour débutants, des descriptions approfondies des fonctionnalités, et des guides de meilleures pratiques qui sont essentiels pour les développeurs de tous niveaux.

Conclusion
Le stack MERN se distingue par sa simplicité, une grande communauté, et d'excellentes documentations. Ces éléments contribuent à un cycle de développement efficace et à une expérience d'apprentissage enrichissante, ce qui fait de MERN un choix populaire pour le développement d'applications modernes, performantes et scalables.
