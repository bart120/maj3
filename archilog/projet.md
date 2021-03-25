
# Projet Architecture logiciel

# I- Sujet

## A faire

A partir du cahier des charges ci-joint et des informations ci-dessous, Vous devez réaliser un DAT complet avec notament:
- Les principaux diagrammes UML
- L'architecture matériel
- La/les architectures logiciel utilisées
- Délais de réalisation

## Principaux diagrammes UML
* cas d’utilisation : interactions entre le système et les utilisateurs (et autres systèmes externes). Il aide dans la visualisation des exigences / besoins ;
* activité : séquence et parallélisme dans les activités du système ; autrement dit, modélisation des processus métier avec les échanges de données
* classes : classes, types, interfaces et relations entre eux ;
* objets : instances de classes définissant une configuration importante du système ;
* machine à états4 : états des classes à travers leur cycle de vie (de la création / instanciation des objets à leur destruction) et les événements qui provoquent les transitions / changements d’états ;
interaction, qui se décline en deux types de diagrammes :
* séquence : interactions entre des objets pour lesquelles l’ordre des interactions est important ;
* communications5 : interactions entre objets pour lesquels les connexions entre objets sont importantes ;
* composants : rassemblements de classes ou de composants tels que vus par l’équipe de développement pour décomposer le système en parties de logiciel gérables (du point de vue développement en gestion de projet) ;
* paquetages : rassemblement d’éléments de modélisation par exemple pour les distribuer entre membres de l’équipe de développement ;
* déploiement : unités d’installation, de configuration et de déploiement du produit fini sur un parc de machines.

## modele-da

Modèle de Dossier d'Architecture (DA) applicable à la plupart des projets d'informatique de gestion, indépendamment de l'architecture générale retenue (monolithe, SOA, micro-service, n-tiers, ...).
Ce modèle a déjà été utilisé sur plusieurs projets importants y compris au sein de grandes organisations. Il s'enrichit régulierement.

## Principes du modèle

Nous avons découpé l'architecture en cinq volets (applicatif, sécurité, dimensionnement, infrastructure et développement), chaque volet étant auto-porteur. 

L'idée est de proposer un ensemble de vues d'architecture alignées sur les rôles que l'on trouve le plus fréquemment dans les organisations et sur leurs préoccupations respectives. Par exemple, un(e) architecte d'infrastructure ou un(e) ingénieur DevOps a rarement besoin de connaitre le détail de l'architecture logicielle (le détail des frameworks utilisés ou façon de traiter les erreurs). De même, un(e) PO ou un(e) architecte d'entreprise va s'intéresser à la vision macroscopique des modules applicatifs et de leurs interactions principales ("le batch B appelle le service S")  mais rarement du détail de l'infrastructure sous-jacente (choix de la base de donnée du service, dimensionnement des machines, ...).


Un dossier suivant ce modèle sera ainsi constitué :

* d’un volet applicatif présentant le contexte général et l’architecture applicative ;
* d’un volet développement présentant l’architecture logicielle et son environnement ;
* d’un volet dimensionnement présentant les aspects liés aux performances et au dimensionnement de l'infrastructure ;
* d’un volet infrastructure présentant les serveurs, les middlewares, l'exploitation, etc. ;
* d’un volet sécurité ;

### Conseils sur la rédaction de votre dossier d'architecture 
* Rester bref, chaque mot doit avoir son utilité. Pas d’explication bateau type ‘ceci est l’introduction’, pas de redites d’autres documents, de l’historique de l’entreprise ou de concepts vagues ;
* Un lecteur doit comprendre le fonctionnement et les contraintes de l’application sans être noyé de détails. Le document doit rester maintenable et à jour ;
* Si l’application suit une architecture standardisée par l’organisation, ne jamais la répéter et se référer à un document commun ;
* Si un chapitre n’est pas applicable, ne pas le laisser vide mais simplement mentionner `N/A` pour que le lecteur sache que le sujet a été traité ou `TODO` s'il reste à compléter ;
* Ce modèle se veut suffisamment complet pour couvrir la plupart des applications. Il est donc normal que de nombreux chapitres ne soient pas applicables dans votre contexte ; 
* Lister les hypothèses d’architecture et études en cours dans le chapitre "Points non statués" de chaque volet (ils doivent être exceptionnels, sinon le DA est rédigé trop tôt) ;
* Isoler dans des annexes en fin de document les informations d'architecture importantes mais concernant des points précis n’intéressant que peu de lecteurs ;

### Que ne trouve-t-on *PAS* dans ce document ?
* la conception détaillée du projet (diagrammes UML de classes, de séquences ...) sauf pour présenter un pattern général spécifique à l’application ;
* des éléments d’études (SWOT, scénarios…) : les choix doivent déjà avoir été faits ;
* l’urbanisation du SI (nous nous positionnons ici au niveau d’une application ou d’un ensemble de composants cohérents) ;
* les règles d'architecture de référence (communes à toutes les applications) ;
* des détails techniques (IP, logins) pouvant compromettre la sécurité ;
* le détail des environnements autres que la production (recette, développement...). Ces derniers sont en général trop fluctuants pour figurer dans ce dossier et gagneront à plutôt être documentés par l'intégrateur dans d'autres dossiers, fiches, wikis ou outils de CMDB.

# Groupes et fonctionnement

Le projet est a faire en groupe de 2 personnes (ou seul).
Tous les groupes seront définis en cours, sous la supervision de l'enseignant. Les groupes s'enregistrent avec un nom de groupe ainsi que les noms de leurs membres.

Toute inscription est définitive.  Les étudiants ne sont pas autorisés, par la suite, à changer de groupe.


# Soutenance et rendu

Le rendu aura lieux le jeudi 1er avril 2021.

Les rendus doivent figurer sur un seul compte par groupe.
Le mail de rendu est madani.boukebeche@ynov.com avec en copie vincent.leclerc@ynov.com
Les fichiers rendus doivent contenir
  - Les fichiers et documents techniques du projet.
  - Un AUTHORS.TXT listant les membres du groupe (prénom, nom), à raison d'un par ligne.  Il liste ensuite les responsabilités effectives de chacun dans le groupe.
Le sujet du mail doit contenir votre section ainsi que le nom du projet.
Les fichiers rendus peuvent aussi comprendre: 
  - Des documents de recherche créés pour le projet et fournissant plus de détails pour l'enseignant.
Pour tout autre type de fichier, veuillez demander à l'enseignant si son inclusion est appropriée.

Les groupes sont les suivants:
- Ramirez Tristant	PREDY Marwin	
- MARTIN Matthieu	LEMOAL Baptiste	
- KASSOURI Cherif	MICHEL Tanguy	
- GOULLEY Aurélien	Ousmane	
- KALWAROWSKI Aude	Aminata	
- Ka Sidy	ABBONEAU Cyril	Florian BELLAIR
- Truong Jonathan	Amar Maha	
- LE HEN Diego	BOSGAERD Rémi	
- Pinard Bastien	CELEBY Jerome	
- Aka Jean Elisée	NGOUNÉ Cédric	
- MATTE Floran	TEDESCO Paul	
- TRAN VAN Léon	Kévin Cassar	
- Wassim KHADRAOUI	Nourhen BARHOUMI	
- Abdessalam Benharira	Naomi Paulmin	
- Madjid Djennane	AYOUNI Charif	
- RAHMANE Rahan	Bob Mery	
- BARKA Ramy	LEVEQUE Luc	
- VIRY Quentin		
- BOUGHDIRI Rachida		


Pour ceux dont le groupe n'est pas dans la liste, contactez-moi très rapidement à vincent.leclerc@ynov.com