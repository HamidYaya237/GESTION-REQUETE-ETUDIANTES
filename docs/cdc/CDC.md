	 



PROJET GENIE LOGICIEL










REALISER PAR : HAMIDOU YAYA
MATRICULE :    21A0883FS
LIEN GITHUB : https://github.com/HamidYaya237/GESTION-REQUETE-ETUDIANTES





ENSEIGNANT : M BAYANG SOULOUKNA




I.	CAHIER DES CHARGES FONCTIONNEL

1.	CONTEXTE

         Dans notre université la procédure de dépôt de requête étudiante est essentiellement manuelle.  Les étudiants sont contraints de se déplacer physiquement vers le département pour déposer leurs requêtes, après avoir effectué plusieurs démarche préalables tels que les photocopies, l’achats de chemises cartonner… ce mode de fonctionnement entraine une perte de temps considérable aussi bien pour les étudiants que pour l’administration. 

2.	Problématique

Le traitement manuel des requêtes engendre plusieurs difficultés : lenteur dans l’exécution, risqué de perte ou de mauvais classement des dossiers, et surcharge de travail pour le chef de département et les enseignants qui doivent traiter les requêtes une à une sans outils de suivi structuré. Cette situation nuit à l’efficacité administrative et à la satisfaction des étudiants.


3.	Présentation du projet
Le projet consiste à développer une application web permettant la gestion des requêtes universitaires en ligne dans les universités de Maroua.
L’application permet aux étudiants de soumettre des requêtes administratives et de suivre leur état, tandis que l’administration peut consulter et traiter ces requêtes.
4.	Objectif général
Faciliter la soumission, la consultation et le suivi des requêtes universitaires à travers une application web simple et accessible.
5.	Objectifs spécifiques
	Permettre aux étudiants d’envoyer leurs requêtes en ligne
	Réduire les déplacements physiques vers les services administratifs
	Permettre un suivi simple des requêtes
	Offrir une interface claire et facile à utiliser
4. Acteurs du système
o	Étudiant (soumettre une requête et consulter l’états de toutes les requetés soumis)
o	Enseignants (traiter une requête)
o	Chef de département (consulter toutes les requêtes, traiter les requêtes ; ajouter un enseignant)
5. Fonctionnalités principale
5.1 Fonctionnalités pour les étudiants
•	Création d’un compte étudiant
•	Accès à l’application via un navigateur web
•	Remplissage d’un formulaire de requête
•	Choix du type de requête
•	Envoi de la requête
•	Consultation de la liste des requêtes soumises
•	Consultation de l’état de chaque requête
5.2 Fonctionnalités pour le chef de département
•	Accès à la liste des requêtes
•	Consultation des détails d’une requête
•	Modification de l’état de la requête (en attente, traitée)
•	Ajout des enseignants
5.3 Fonctionnalités pour l’enseignant
•	Accès à la liste des requêtes
•	Consultation des détails d’une requête
•	Modification de l’état de la requête (en attente, traitée)
6.	Besoin fonctionnel 
6.1.	Parcours utilisateurs
   

Parcours 1: dépôt de requête 
Inscription-connexion- tableau de bord – création requête – paiement –confirmation
Parcours 2 :   suivie de requête
Connexion – tableau de bord – consultation des                                       requêtes – visualisation du statut de la requête 
Parcours 3 :   traitement d’une requête
Connexion administrateur – listes des requêtes – consultation – consultation – traitement – mise a jour du statut  
6.2.	User stories 
US-01: en tant qu’étudiants je veux soumettre une requête en ligne afin d’éviter le déplacement physique.
Priorité – must
Critère d’acceptation :
o	Etant donné un formulaire valide, quand je soumets ; alors la requête est enregistrée.
o	Etant donne un formulaire incomplet, quand je valide, alors le système affiche une erreur  
o	Etant donne une requête soumise alors elle apparait dans mon historique.

US-02: en tant qu’étudiants je veux créer un compte afin de pouvoir accéder à la Platte forme 
Priorité – must
Critère d’acceptation :
o	Etant donné les information valides, quand je m’inscris, alors mon compte est créé 
o	Etant donne un matricule déjà utiliser quand je valide alors le système refuse l’inscription 
o	Etant donne des champs incomplets, quand je valide, alors le système refuse l’inscription.
US-03: en tant qu’étudiants je veux payer les 100f pour soumettre une requête. 
Priorité – must
Critère d’acceptation :
o	Etant donné un paiement réussi, alors la requête est envoyée.
o	Etant donne un paiement échoué alors la requête n’est pas soumise. 
6.3.	Exigence fonctionnelle

RF-01 : le système doit permettre à un étudiant à créer un compte.
RF-02 : le système doit permettre la soumission de requêtes en ligne 
RF-03 : le système doit intégrer le paiement de 100f par requête.
RF-04 : le système doit permettre le suivi de l’état des requêtes.
6.4.	Contraintes fonctionnelles
•	Application utilisable sans connexion à une base de données
•	Stockage des informations localement
•	Utilisation simple, adaptée aux étudiants
7. Résultats attendus
•	Une application web fonctionnelle
•	Une meilleure organisation des requêtes
•	Une interface claire et compréhensible
 
II.	CAHIER DE CHARGE TECHNIQUE
         Application web de gestion des requêtes universitaires
1.	Présentation générale
      Ce cahier des charges technique décrit les choix technologiques, l’architecture, les contraintes techniques et l’environnement de développement de l’application web de gestion des requêtes universitaires dans les universités de Maroua. L’application est développée dans un cadre académique et fonctionne sans serveur ni base de données, uniquement avec des technologies web côté client.
2.	Environnement de développement
	Système d’exploitation : Windows 
	Éditeur de code : Visual Studio Code 
	Navigateur de test : Mozilla Firefox
	Langages utilisés :HTML, CSS et JavaScript.

3.	Architecture technique
L’application repose sur une architecture client-side.
3.1. Principe :
•	Le navigateur web constitue la plateforme d’exécution
•	Toute la logique applicative est gérée par JavaScript
•	Aucune communication avec un serveur externe
Schéma simplifié :
Utilisateur
↓
Navigateur Web
↓
HTML + CSS + JavaScript


3.2. Justification du choix technologique

	Simplicité de mise en oeuvre ;
	Maitrise de la technologie par le concepteur ;
	Réduction de complexité liées aux bases de données et au back-end 

3.3. Limites connues
o	Les données sont stockées localement sur le navigateur ;
o	Les donnes ne sont pas partagées entre plusieurs appareils ;
o	Le stockage est limité par le navigateur ;
o	Application non destinée à une utilisation réelle à grande échelle ;
o	Données non partagées entre plusieurs utilisateurs.

4.	Organisation du projet
La structure du projet est organisée de manière simple et claire :
•	index.html : page principale
•	style.css : feuille de styles
•	script.js : logique de l’application
Cette organisation facilite la compréhension et la maintenance du code.
5.	Sécurité
•	Aucune authentification avancée
•	Données accessibles uniquement via le navigateur local
•	Niveau de sécurité adapté à un projet académique

6.	¬¬Tests et validation
•	Tests fonctionnels via navigateur
•	Vérification de la soumission et de l’affichage des requêtes
•	Tests de compatibilité sur plusieurs navigateurs


7.	Maintenance et évolutivité
•	Code simple et lisible
•	Possibilité d’ajouter ultérieurement :
	Un serveur backend
	Une base de données
	Une authentification sécurisée.
Conclusion
Ce cahier des charges technique présente une solution simple et a, répondant aux objectifs pédagogiques du projet. Les choix techniques effectués permettent de développer une application fonctionnelle tout en respectant les contraintes académiques.

 
ANNEXE
1-	DIAGRAMME DE CLASSE 
CLASSE :
	ETUDIANTS (matricule ; nom ; prénom ; filière ; niveau)
	Enseignant (matricule ; Nom ; prénom unité d’enseignement)
	Chef de département (matricule ; Nom ; prénom unité d’enseignement)
	Requête (id requête ; type ; description ; Matricule étudiant)















	

2-	DIAGRAMME DE CAS D’UTILISATION


ACTEURS :
	ETUDIANTS 
	ENSEIGNANT
	CHEF DE DEPARTEMENT qui hérite des propriétés de l’enseignant
Cas d’utilisation :
            Pour ETUDIANTS :
o	S’inscrire
o	Se connecter 
o	Soumettre une requête
o	Effectuer un paiement
o	Consulter l’état de requête
o	Consulter l’historique des requête
      Pour ENSEIGNANTS :
o	Se connecter 
o	Consulter les requêtes 
o	Traiter une requête 
o	Modifier le statut d’une requête
        Pour CHEF DE DEPARTEMENT :
o	Ajouter un enseignant


