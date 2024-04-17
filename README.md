# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)

---------------------------------------------------------------------------------------------------------------------------------
I. Général
 --------------------------------------------------------------------------------------------------------------------------------
1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte
   
        - Il faut installer un environnement côté serveur.
  	  Deux exemple : Laragon que l'on utilise en cours, et XAMPP
  	
2.	Qu’est-ce qu’un algorithme ?
	
        - Un algorithme est une suite finie et non ambiguë d'instructions et d’opérations
  	  permettant de résoudre une classe de problèmes.
      
3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?
	
        - En informatique, une variable est un symbole (habituellement un nom) qui renvoie à une position de mémoire
  	  dont le contenu peut prendre successivement différentes valeurs pendant l'exécution d'un programme.
        - En mathématiques et en logique, une variable marque un rôle dans une formule, un prédicat ou un algorithme.
      
        - Une variable en PHP est préfixée par un symbole dollar $.
        - Le nom est sensible à la casse. Les noms de variables suivent les mêmes règles de nommage que les autres entités PHP.
        - Un nom de variable valide doit commencer par une lettre ou un souligné (_), suivi de lettres, chiffres ou soulignés .
        - Examples: $var = 'Bob'; $Var = 'Joe';.
      
4.	Qu’est-ce que la portée d’une variable ?
	
	- La portée d'une variable est la zone de code où elle a été déclarée et peut être utilisée.
        - En programmation, une variable peut avoir une portée locale ou une portée globale.
        - La portée variable générale s'applique à tous les blocs de code, y compris les classes.
        -  En JS: lle sera accessible dans les blocs intérieurs.
        - Pour contrôler l'accès aux variables et aux fonctions, il est possible d'utiliser
           des niveaux de contrôle : public, protected, package-protected et private.
   
5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?
	
        - Une constante est une variable dont la valeur ne peut pas être modifiée.
        - Tenter de modifier la valeur d’une constante provoque une erreur.
       
6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation
        - Une superglobale PHP est une variable PREDEFINIE, disponible partout et tout le temps dans un script.
  	 Il en existe 8 :
         - $_GET
         - $_POST
         - $_REQUEST
         - $_COOKIE
         - $_SESSION
         - $_SERVER
         - $_FILES
         - $_ENV

 	 
7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ?
        Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)

	 - $string = "Bonjour";
         - $number = 13;
         - $float = 12.34;
         - $boolean = true;
         - $array = ["azerty", 2, 45.4, "uiop"]
         - $undefined = undefined;
         - $dateTime = new Date('1995-07-03')
 
8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?

	    Oui, il existe différents types de tableaux.

          - Il existe les tableaux simples de variables tel que :
            array(1, 2, 3, "a", "b", "c")
          - Et il existe les tableaux "associatifs" avec la forme clé => valeur, où l'on attribue à chaque clé une valeur :
            array("nom" => "Louërat", "prenom" => "floris", "age" => 28) 


9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles

	xxx

10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?

	- strlen('phrase').
 - 
11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP

	xxx
   
12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP
    
        xxx
    
13.	Quelle est la différence entre les instructions « require » et « include » en PHP

        xxx
   	
14.	Comment effectuer une redirection en PHP ?
    
        xxx
   	
15.	Définir la partie « front-end » et « back-end » d’une application

	- Le front-end est la partie visible d'une application ou d'un site web, la partie où l'on se concentre justement sur le UX - UI.
        - Le back-end est la partie que l'utilisateur ne voit pas, la partie invisible, côté serveur, qui peut être la base de donnée,
          les requêtes envoyées au serveur


16.	Définir le contrôle de version ? Qu’est-ce que Git ?

         xxx
17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples

    
----------------------------------------------------------------------------------------------------------------------------------------
II. Front-end
----------------------------------------------------------------------------------------------------------------------------------------
1.	Définir HTML

	-  HyperText Markup Language. Il sert à donner une structure au projet à l'aide de balises.

2.      Définir CSS

        - Cascading Styles Sheet. Il permet quant à lui de modifier le style de chaque élément
	
3.	Définir Javascript
	
        - Javascript, aussi appelé JS, est le langage qui a rendu possible le « dynamisme côté client » de toutes les applications web.
        - Depuis, grâce à Node.js, il peut également être utilisé côté serveur, ce qui en fait le seul langage
  	 pouvant être utilisé en frontend et en backend. ( à compléter...)
  	- JavaScript est un langage de programmation permettant d'ajouter des scripts pour rendre l'application plus responsive.
   	
4.	Définir JSON. Dans quel contexte ce format est-il utilisé ?

        - JSON est une structure utilisée pour conserver des données, utilisé donc en base de donnée.

	
5.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?

	- Je pense que oui, en envoyant un exécutable en PHP via le JavaScript?

6.	Qu’est-ce qu’un sélecteur CSS ?

        - une classe, identifiant, ou balsie permettant d'identifier un élément dans le HTML pour y attribuer des styles.

7.	Quelle balise HTML permet de créer un lien hypertexte ?

        - <a href='lienhypertexte'>le lien</a>

8.	Qu’est-ce qu’une requête AJAX ?

        xxx
9.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?

	 - "." pour sélectionner une classe et "#" pour un identifiant.
    
10.	Définir le responsive design.

	- Le responsive design s'adapte aux différents types et tailles d'appareils pour que l'utilisateur ait une meilleure expérience
    
11.	Qu’est-ce que le templating ?

          xxx
   	
12.	Qu’est-ce qu’une fonction anonyme en Javascript ?

	- Une fonction anonyme en JavaScript est une fonction qui est définie sans nom.
        -  Ces fonctions sont souvent utilisées pour créer des fonctions qui ne seront pas réutilisées ailleurs ou pour passer une fonction en tant qu’argument à une autre fonction. 
        - Voici un exemple simple :
          setTimeout(function() {
             console.log('Ceci est une fonction anonyme');
          }, 1000);
        - Dans cet exemple, setTimeout utilise une fonction anonyme qui affiche un message dans la console après un délai d’une seconde.
        - La fonction est exécutée une fois et n’a pas besoin d’être nommée car elle n’est pas utilisée ailleurs.
          
        - Autre exemple forEach
        - forEach prend en paramètre une fonction dite "callback (ou fonction de rappel) qui sera  exécuté à chaque tour de boucle.
        - Dans cette fonction anonyme, chaque "li" sera représenté par la variable passée en argument "element" (qui peut etre nommée autrement si besoin)
        -     let listElements = list.querySelectorAll("li")
              // pour modifier des éléments du DOM (la propriété style de chaque élément en effectuant un boucle forEach( sur  la NodeList))
              listElements.forEach(function(element){
                  element.style.color = "red"
              })

13.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?

	- Pour ajouter un élément à la fin du tableau indexé on utilise la méthode .push(newElement) de la classe Array par example:
          tableauIndexe.push(2);
        - Nous ne pouvons pas ajouter seulement un élément au tableau associatif, on peut ajouter une/des pairs (duos) clef/valeur, par example:
          tabAssoc.cle1 = "Valeur1";
              
14.	Qu’est-ce qu’un « media query » ?

        - C'est un moyen utilisé en CSS afin d'attribuer des styles en fonction du type ou de la taille de l'appareil de l'utilisateur.
   	
15.	Qu’est-ce qu’un pseudo élément en CSS ?

          xxx

16.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent

	  xxx Un frameWork CSS 
  
17.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes.

        -  xxx GET et POST. Un permet d'envoyer des données au serveur et l'autre de

--------------------------------------------------------------------------------------------------------------------------------
III. UX UI
--------------------------------------------------------------------------------------------------------------------------------
1.	Quelle est la différence entre UX Design et UI Design ?

        - UI (User Interface) se concentre sur l'interface, l'aspect visuel pour l'utilisateur.
  	- UX (User eXperience) se concentre sur l'experience, les interactions de l'utilisateur avec les diffrents objets.
	
2.	Qu’est-ce qu’un wireframe ?
 
        xxx
	
3.	Qu’est-ce qu’un prototype ?

        xxx
4.	Qu’est-ce que la hiérarchie visuelle en UI Design ?

        xxx	
5.	Qu’est-ce que l’accessibilité en UX Design ?

        xxx
  	
6.	Qu’est-ce qu’une grille de mise en page ?

        xxx
  	
7.	Qu’est-ce que la notion d’affordance en UX Design ?

        xxx
  	
8.	Qu’est-ce qu’un « mobile first design » ?

        - C'est quand on vise à adapter notre application pour mobile en priorité,
  	  et ensuite on mettra les @mediaQueries par exemple, pour les autres écrans.

-----------------------------------------------------------------------------------------------------
IV. Programmation orientée objet (POO)
------------------------------------------------------------------------------------------------------
1.	Donner une définition de la programmation orientée objet

        xxx
  	
3.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?

	- Une classe est un ensemble d'attributs et se déclare avec un constructor.

3.	Qu’est-ce qu’un objet ?

        xxx
  	
4.	Définir la notion de propriété / attribut / méthode

        xxx
  		
5.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité

        xxx
  	
6.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?

        xxx
7.	Qu’est-ce que l’encapsulation ?

        xxx
  		
8.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple

        xxx
  	
9.	Définir l’opérateur de résolution de portée

        xxx
  	
10.	Définir une méthode / propriété statique

        xxx
   	
11.	Définir le polymorphisme en POO

        xxx
   	
12.	Définir une méthode / classe abstraite ?

        xxx
   	
13.	Définir le chaînage de méthodes

        xxx
   	
14.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »

        xxx
   	
15.	Qu’est-ce qu’un « autoload » ?

	- C'est une fonction qui va aller chercher toutes les classes existantes dans les autres fichiers php :
          spl_autoload_register(function ($class_name) {   require 'classes/'. $class_name .'.php';}   );
        
16.	Comment appelle-t-on en français les « getters » et les « setters » ?

        - Les getters renvoient la valeur de la variable et les setters permettent de la changer.
   	
17.	Qu’est-ce que la sérialisation en PHP ?

        xxx
   	
----------------------------------------------------------------------------------------------------------------------
V. Architecture 
----------------------------------------------------------------------------------------------------------------------
1.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur.
         Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence

	  xxx
  	
2.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern.

	- Un design pattern est un patron d'architecture ce qui permet quelques avantages :
          respecter des méthodes de conception professionnellement reconnues ;
          développer plus rapidement en suivant des modèles architecturaux ayant fait elurs prevues ;
          permettre au code d'être relu plus facilement par un autre développeur sensibilisé aux pattenrs utilisés.
          Exemple : Factory, Composite, Iterator, Observer, Singleton, Strategy, Template.
   
3.	Qu’est-ce que l’architecture MVC ?
    
        - C'est un patron de conception concernant l'agencement du code, segmenté en trois sections :
   	  modèle, vue, controlleur.
	
4.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?

        - Modèle : cette partie gère ce qu'on appelle la logique métier du site.
  	  Elle comprend notamment la gestion des données qui sont stockées, mais aussi tout le code qui prend des décisions autour de ces données.
  	  Son objectif est de fournir une interface d'action la plus simple possible au contrôleur.
  	  On y trouve donc entre autres des algorithmes complexes et des requêtes SQL.
  	
        - Vue : cette partie se concentre sur l'affichage.
  	  Elle ne fait presque aucun calcul et se contente de récupérer des variables pour savoir ce qu'elle doit afficher.
  	  On y trouve essentiellement du code HTML mais aussi quelques boucles et conditions PHP très simples,
  	   pour afficher par exemple une liste de messages.
  	
        - Contrôleur : cette partie gère les échanges avec l'utilisateur. C'est en quelque sorte l'intermédiaire entre l'utilisateur,
  	  le modèle et la vue. Le contrôleur va recevoir des requêtes de l'utilisateur. Pour chacune, il va demander au modèle d'effectuer certaines actions
  	  (lire des articles de blog depuis une base de données, supprimer un commentaire) et de lui renvoyer les résultats
  	  (la liste des articles, si la suppression est réussie).
  	  Puis il va adapter ce résultat et le donner à la vue.
  	  Enfin, il va renvoyer la nouvelle page HTML, générée par la vue, à l'utilisateur.
  	
5.	Quels sont les avantages de l’architecture MVC ?

         xxx
6.	Existe-t-il des variantes à l’architecture MVC ?
   
         - Modèle-Vue-Présentateur (MVP)
         - Modèle-Vue-VueModèle (MVVM)
         - Modèle-Adaptateur-Vue (MAV)
         - Modèle-Vue-Contrôleur-Frontière (MVCF)
         - Modèle-Interactions-Vues-État (MIVES)
  	
7.	Qu’est-ce qu’une API ? Définir l’architecture REST

         - C'est une interface de traitement d'applications entre un serveur web et un navigateur web.
  	   L'architecture REST (Representational State Transfer) définit les principes REST par 4 contrôles d'interface,
  	   notamment l'identification des ressources, la gestion des ressources via des représentations,
  	   l'activation des communications autodescriptives et la transformation de l'hypermédia en moteur de l'état de l'application.

---------------------------------------------------------------------------------------------------------------------------------------
VI. Modélisation - Base de données
---------------------------------------------------------------------------------------------------------------------------------------
1.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise

        - C'est le processus de création d'une représentation visuelle ou d'un plan
   	  qui définit les systèmes de collecte et de gestion de l'information de toute organisation.
          La méthode Merise est une méthode d'analyse, de conception et de réalisation de systèmes d'informations.
   	
2.	Quelles sont les 3 étapes principales de la méthode Merise ?

	 - a. Analyse, conception et réalisation   - Cette réponse OK.
         - b. Planification, exécution et contrôle
         - c. Création, modification et suppression
           

3.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?

        - Le MCD fournit une description graphique pour représenter des modèles de données
  	   sous la forme de diagrammes pouvant contenir des entités ou des associations.
  	
4.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?

        - C'est une représentation structurée et normalisée des données d'un système d'information,
  	  conçue pour être directement implémentable dans une base de données relationnelle.
  	
5.	Donner la définition des mots suivants :
        a.	Entité
        b.	Relation
        c.	Cardinalité
        d.	Clé primaire / clé étrangère

        a. Entité : Une entité est un objet ou un concept identifiable qui peut être représenté dans une base de données. Exemple : 'Livre' et 'Auteur'
        b. Relation : Une relation c'est une association entre les différentes entités. Elle représente la manière
  	   dont les données sont liées les unes aux autres. Exemple : 'Livre' et 'Auteur', un livre est écrit par un auteur.
        c. Cardinalité : Sert à compter le nombre minimum et maximum de possibilités que chaque classe contient dans la relation liant deux ou plusieurs objets.
        d. Clé primaire : garanti l'unicité d'un enregistrement dans une table;
           Clé étrangère : garanti le lien avec une autre table.
           Clé primaire dans table associative : c'est l'association des clés étrangères qui fait que la table associatve est la clé primaire.
  	
6.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?

	 xxx
   
7.	Qu’est-ce qu’une base de données ?

        - Une base de données est un outil qui permet de collecter et d'organiser des informations.
  	
8.	Définir les notions suivantes : 
       - a. SQL b.MySQL c.SGBD (donner 2 exemples de SGBD)

        - a. SQL : Structured Query Language, c'est un langage informatique normalisé servant à exploiter des bases de données relationnelles.
        - b. MySQL : MySQL est un système de gestion de bases de données relationnelles.
        - c. SGBD (donner 2 exemples de SGBD) : Système de gestion de base de données, c'est un logiciel système permettant aux utilisateurs et programmeurs
  	  de créer et de gérer des bases de données, exemple : MySQL, Oracle et SQL Server.
  	
9.	Dans une base de données, les données sont stockées dans des ___. Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___

        - 
10.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?
11.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?
12.	A quoi sert une vue dans une base de données ?
13.	Qu’est-ce que l’intégrité référentielle dans une base de données ?
14.	Quelles sont les fonctions d’agrégation en SQL ?
15.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
16.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table
b.	Modifier un enregistrement dans une table
c.	Supprimer un enregistrement dans une table
d.	Supprimer la base de données
e.	Filtrer les résultats d’une requête SQL
f.	Trier les résultats d’une requête SELECT
g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
h.	Concaténer 2 chaînes de caractères 
17.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

---------------------------------------------------------------------------------------------------------------------------
VII. Symfony
--------------------------------------------------------------------------------------------------------------------------
84.	Qu’est-ce que Symfony ?

        - Symfony est un framework PHP "open source" utilisé par les développeurs pour créer
   	  des sites ou applications web complexes, robustes, fiables, évolutifs, maintenables et performants.
   	
85.	Sur quel langage de programmation et design pattern repose Symfony ?

	 - Le langage de programmation sur lequel repose Symfony est le PHP.
           Le design pattern sur lequel repose Symfony est le modèle de conception MVC (Modèle-Vue-Contrôleur).
           Les données de l'application (le modèle) sont séparées de l'interface utilisateur (la vue) et de la logique de contrôle (le contrôleur),
           ce qui permet une meilleure organisation du code et une meilleure maintenabilité de l'application.
    
86.	Quelle est la dernière version en date de Symfony ?

	 - La dernière version en date de Symfony est là 7.0.5 (Stable Release, 6.4.5 pour la LTS (Long-Term Support)).
    
87.	Qu’est-ce qu’un bundle ?

        - Un bundle est une offre groupée, un ensemble de produits vendus ensemble.
   	
88.	Quel est le moteur de template utilisé par défaut dans Symfony ?

        - Le moteur de template par défaut est Twig. c'est un moteur de template flexible, rapide et sécurisé, spécialement conçu pour être utilisé avec PHP.
   	  Il est simple à utiliser et a une bonne capacité à séparer efficacement la logique de présentation de la logique métier dans les applications web.
   	
89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91.	Que permet le bundle Maker au sein de Symfony ? 
92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?
    
------------------------------------------------------------------------------------------------------------------------
VIII. Sécurité
------------------------------------------------------------------------------------------------------------------------
94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?
95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
97.	Définir l’attaque par force brute et l’attaque par dictionnaire
98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
100.	Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
101.	Qu’est-ce qu’une politique de mots de passe forts ?
102.	Qu’est-ce que l’hameçonnage ?
103.	Définir la « validation des entrées »

-----------------------------------------------------------------------------------------------------------------------
IX. RGPD
------------------------------------------------------------------------------------------------------------------------
104.	Qu’est-ce que le RGPD ?

        - C'est le Règlement Général de la Protection des Données.
          
106.	Quel est son objectif principal ?
107.	Quelle est la date d’entrée en vigueur du RGPD ?
108.	Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
109.	En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
110.	Quel est le consentement valide selon le RPGD ?
111.	Qu’est-ce qu’une politique de confidentialité ?
112.	Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
113.	Quels sont les droits des utilisateurs selon le RGPD ?
114.	Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO
1.	Qu’est-ce que le SEO ?
     
      - Le SEO (Search Engine Optimization) est l'acronyme qui signifie « Optimisation pour les moteurs de recherche » en français.
    	
2.	Quel est l’objectif principal du SEO ?

        - C'est un ensemble de techniques permettant d'améliorer le positionnenement d'un site web dans les moteurs de recherche (Google, Bing, Yahoo, etc.)
           afin de le rendre visible auprès des internautes.
          
3.	Existe-t-il plusieurs types de référencement ? Lesquels ?

        - Les trois différents types de référencement sont le SEO sur-page, le SEO hors-page et le SEO technique.
  	
4.	Qu’est-ce que la densité de mots-clés en SEO ?
   
5.	Qu’est-ce qu’une balise « alt » ?

      - La balise ALT, également connue sous le nom d'« attribut ALT », correspond au texte alternatif d'une image ou d'un visuel sur une page Internet.
        Il fait partie des champs possibles à remplir en codage HTML et permet de donner une description de l'image ou du visuel
        si ce dernier n'apparaît pas à l'écran.
        
6.	Qu’est-ce que la balise « meta description » ?

        - La Meta Description est une des balises HTML les plus connues en référencement.
  	  Elle permet de fournir une description aux moteurs de recherche pour l’affichage des résultats au sein des SERP ou aux applications web
  	  ayant besoin d’un petit résumé rapide. De plus, lorsqu’elle est de qualité, elle peut inciter l’internaute à cliquer sur votre site
  	  ce qui augmente le trafic naturel.
  	
7.	Qu’est-ce que le « nofollow » en SEO ?

        - Un lien nofollow est un lien inséré par l'éditeur sur un contenu de son site internet.
  	  Ce lien a la particularité de donner l'indication aux moteurs de recherche de ne pas suivre son contenu et
  	  donc de ne pas le prendre en compte pour le référencement naturel du site.
  	
8.	Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
9.	Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
10.	Quelle est la recommandation pour les URL d'un site web bien référencé ?
11.	Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
12.	Qu'est-ce que l'optimisation des images pour le référencement ?
13.	Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps
127.	Qu’est-ce que la gestion de projet ?	
128.	Qu’est-ce qu’une méthode Agile de gestion de projet ? 
129.	Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
130.	A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131.	Qu’est-ce que la planification itérative ?
132.	Citer 3 méthodes Agiles dans le cadre d’un projet informatique
133.	Qu’est-ce qu’une réunion de revue de projet ?
134.	Qu’est-ce qu’un livrable dans un projet ? 
135.	Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
136.	Qu’est-ce que le DevOps et quel est son objectif principal ?
137.	Qu’est-ce que l’intégration continue ? 
138.	Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
139.	Qu’est-ce qu’un test unitaire ? 
140.	Quelle est l'unité de code testée lors d'un test unitaire ?
141.	Quelles sont les caractéristiques d'un bon test unitaire ?
142.	Qu'est-ce qu'une assertion dans un test unitaire ?
 
## English
1)	What does JavaScript enable you to do on a website ?
a.	Add interactive behavior and dynamic content - OK
b.	Define the layout and design of web pages
c.	Handle server-side operations


3)	Which programming language is primarily used for server-side web development ?
a.	PHP
b.	JavaScript
c.	HTML

4)	What is the purpose of a web browser ?
a.	To render and display web pages
b.	To execute serve-side code
c.	To manage databases

5)	What is the difference between GET and POST methods in HTTP ?
a.	GET retrieves data from a server, while POST submits data to a server
b.	GET submits data to a server, while POST retrieves data from a server
c.	GET and POST methods are interchangeable

6)	What is the purpose of version control systems (e.g., Git) in web development ?
a.	To track changes and manage collaborative development
b.	To optimize website loading speed
c.	To handle server-side scripting

7)	What is the purpose of a framework in web development ?
a.	To provide a structured environment for building web applications
b.	To handle network protocols and data transfer
c.	To create visual designs and layouts for websites

8)	What does NoSQL stand for ?
a.	Not Only SQL
b.	Non-Structured Query Language
c.	New Object-Oriented Language

9)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models
