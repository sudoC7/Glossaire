# Glossaire
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

## Général
1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte 
-   MAMP(pour Mac) et WAMP + LAMP (pour Windows)

2.	Qu’est-ce qu’un algorithme ?  
-   Un algorithme est un ensemble de règles données permettant d'accomplir une tâche précis   

3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?
-   Une variable est une valeur a qui on associe un nom pour mieux l'identifier, Une variable en PHP commence par le signe $ : $var

4.	Qu’est-ce que la portée d’une variable ?
-   C'est l'accessibilité de la variable, elle peut être dans la fonction ou global dans les fichiers 

5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?
-   La constante une fois déclaré avec une valeur donnée elle n'est plus modifiable, alors qu'une variable peut être modifiée 

6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation 
-   Une superGlobal est une variable accessible dans n'importe quel script PHP , il en existe 9, quelques exemples : $_GET(utilisé pour les URL) $_POST(utilisé pour les formulaires) $_COOKIE(stock les données du navigateur  $_SESSION(regroupe les données transmît des supGlobal $_get $_post et $_cookie)

7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)
-   Voici les types primitifs en PHP : const, string, float, int, bool, array, null, avec quelques exemples d'utilisation  : int $var , bool bolean , array tableau

8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?
-   Oui, il y'a des "tableaux indexés : array('a', 'b', 'c', 'd')", tableaux associatifs : array('a'=>1, 'b'=>'text', 'c'=>2, 'd'=>12), tableaux multidimentionnelle sont des tableaux qui contiennent d'autres tableaux, tableaux dynamique et tableaux constante.

9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles
-   

10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?
-   strlen()

11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP
-   La session est un moyen simple pour stocker les données de chaque utilisateur individuellement en utilisant un identifiant unique, la fonction qui permet de démarrer une session $_SESSION

12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP
-   Contient les données stockées du navigateur client,  

13.	Quelle est la différence entre les instructions « require » et « include » en PHP
-   Les deux permettents de charger les fichiers, la seule différence entre les deux c'est que "require" affichera une erreur si le fichier n'existe alors que "include" n'affichera rien comme avertissement.

14.	Comment effectuer une redirection en PHP ?
-   Faut utiliser la fonction header() et elle permet de renvoyer l'internaut d'une page a l'autre 

15.	Définir la partie « front-end » et « back-end » d’une application
-   La partie Front-End est la partie visuel de l'application visible et consultable par le client, La partie Back-End est la partie invisible de l'application où les données et le réseau sont est gérée   


16.	Définir le contrôle de version ? Qu’est-ce que Git ?
-   Désigne la pratique a suivre et a gérer les changements apportées au code d'un logiciel, Git est un logiciel de gestion de versions décentralisé 

17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples
-   Content Management System, c'est un logiciel en ligne qui permet de crée, modifier, et gérer facilement des sites en ligne, sans avoir besoin de connaissance en langage informatique, WordPress. TYPO3


## Front-end
18.	Définir HTML
-   C'est un langage de balisage informatique, il permet construire la squelette du site 

19.	Définir CSS
-   C'est un langage de feuille de style pour la structure du HTML, il permet décorer la structure du site 

20.	Définir Javascript
-   C'est le seul langage utilisé en BACK et FRONT, en back il est utilisé côté serveur et en front pour l'intéractivité et le dynamisme du site 

21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 
-   JSON (JavaScript Object Notation) est un format de données léger et facile à lire, basé sur du texte, qui est couramment utilisé pour l'échange de données sur le web.

22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
-   Oui, il peut être interpréter avec le moteur Node.js. Il est souvent utilisé pour créer des applications web côté serveur, des API, des outils en ligne de commande, etc.

23.	Qu’est-ce qu’un sélecteur CSS ?
-   Un sélecteurs est utilisé pour cibler un élément HTML

24.	Quelle balise HTML permet de créer un lien hypertexte ?
-   La balise <a> permet de crée un lien hypertexte 

25.	Qu’est-ce qu’une requête AJAX ?
-   Technique de développement web qui permet d'actualiser une partie d'une page sans la recharger entièrement

26.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?
-   "#container * {}"<--- l'étoile permet de sélectionner tous les éléments de l'identifiant, ".container * {}"<--- Permet de selectionner tous les éléments du class spécifique 

27.	Définir le responsive design
-   Ajuste automatiquement l’affichage d’une page web à la taille d’écran du terminal utilisé.

28.	Qu’est-ce que le templating ?
-   Le templating fait référence à la pratique de créer des modèles de pages ou de composants réutilisables qui définissent la structure et le design visuel des sites web. 

29.	Qu’est-ce qu’une fonction anonyme en Javascript ?
-   C'est une fonction sans nom associé, exemple -->

  let addition = function(a, b) {
    return a + b;
  };
 
30.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?
-   C'est la méthode push(), il permet d'ajouter un élément a la fin d'un tableau

31.	Qu’est-ce qu’un « media query » ?
-   Media queries est un module CSS3 permettant d'adapter le contenu d'une page web aux caractéristiques de l'appareil de l'utilisateur.

32.	Qu’est-ce qu’un pseudo élément en CSS ?
-   C'est un mot-clé ajouté à un sélecteur qui permet de mettre en forme certaines parties de l'élément ciblé par la règle

33.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent
-   C'est un framework de CSS qui organise et gère la mise en page d'un site web

34.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes
-   Méthode GET : Cette méthode envoie les données du formulaire en tant que paramètres de l'URL dans la requête HTTP
-   Méthode POST : Cette méthode envoie les données du formulaire dans le corps de la requête HTTP.



## UX UI
35.	Quelle est la différence entre UX Design et UI Design ?
-   L'UI Design se concentre sur l'aspect visuel et interactif d'un produit ou d'un service numérique. L'UX Design se concentre sur l'expérience globale de l'utilisateur lors de l'interaction avec un produit ou un service numérique.

36.	Qu’est-ce qu’un wireframe ? 
-   Un wireframe est une représentation visuelle simplifiée et structurée d'une interface utilisateur ou d'une page web.

37.	Qu’est-ce qu’un prototype ? 
-   Un prototype est une déclaration anticipée d'une fonction ou d'une méthode avant sa définition complète

38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?
-   C'est un principe de design qui fait référence à la manière dont les éléments sont disposés dans un design
39.	Qu’est-ce que l’accessibilité en UX Design ? 

40.	Qu’est-ce qu’une grille de mise en page ?
-   Elle permet de découper le format dans sa largeur et dans sa hauteur en plusieurs parties égales 

41.	Qu’est-ce que la notion d’affordance en UX Design ?
-   L'affordance consiste à accorder plus ou moins d'importance à des fonctionnalités, à des boutons ou des pictogrammes, et plus généralement à faire des choix

42.	Qu’est-ce qu’un « mobile first design » ?
-   Le "mobile-first design" est une approche de conception web qui consiste à concevoir d'abord une version optimisée pour les appareils mobiles, puis à élargir cette conception pour s'adapter aux écrans de taille plus grande, tels que les tablettes et les ordinateurs de bureau.

IV. Programmation orientée objet (POO)

43.	Donner une définition de la programmation orientée objet 
-   La programmation orientée objet (POO) est un paradigme de programmation qui repose sur le concept d'objets, qui sont des entités regroupant à la fois des données (appelées propriétés ou attributs) et des fonctions (appelées méthodes) qui agissent sur ces données.

44.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?
-   Une classe en programmation est une structure de données qui permet de définir un ensemble de variables et de fonctions qui représentent un concept ou une entité. Pour déclarer une classe, on utilise le mot-clé "class" exemple : class MaClasse {..Contenue de la classe..}
45.	Qu’est-ce qu’un objet ?
-   Un objet est une instance d'une classe 

46.	Définir la notion de propriété / attribut / méthode
-   propriété : est un élément de description d'un objet, attribut : est une variable d'une classe, méthode :  est une fonction qui est à l'intérieur d'une classe 

47.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité

48.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?

49.	Qu’est-ce que l’encapsulation ?

50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple

51.	Définir l’opérateur de résolution de portée

52.	Définir une méthode / propriété statique

53.	Définir le polymorphisme en POO

54.	Définir une méthode / classe abstraite ?

55.	Définir le chaînage de méthodes

56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »

57.	Qu’est-ce qu’un « autoload » ?

58.	Comment appelle-t-on en français les « getters » et les « setters » ?

59.	Qu’est-ce que la sérialisation en PHP ? 

## Architecture 
60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence
61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
62.	Qu’est-ce que l’architecture MVC ?
63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
64.	Quels sont les avantages de l’architecture MVC ?
65.	Existe-t-il des variantes à l’architecture MVC ?
66.	Qu’est-ce qu’une API ? Définir l’architecture REST

## Modélisation - Base de données
67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise
68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
a.	Analyse, conception et réalisation
b.	Planification, exécution et contrôle
c.	Création, modification et suppression
69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?
71.	Donner la définition des mots suivants :
a.	Entité
b.	Relation
c.	Cardinalité
d.	Clé primaire / clé étrangère
72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?
73.	Qu’est-ce qu’une base de données ?
74.	Définir les notions suivantes : 
a.	SQL
b.	MySQL
c.	SGBD (donner 2 exemples de SGBD)
75.	Dans une base de données, les données sont stockées dans des ___. Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___
76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?
77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?
78.	A quoi sert une vue dans une base de données ?
79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?
80.	Quelles sont les fonctions d’agrégation en SQL ?
81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
82.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table
b.	Modifier un enregistrement dans une table
c.	Supprimer un enregistrement dans une table
d.	Supprimer la base de données
e.	Filtrer les résultats d’une requête SQL
f.	Trier les résultats d’une requête SELECT
g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
h.	Concaténer 2 chaînes de caractères 
83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

## Symfony
84.	Qu’est-ce que Symfony ?
85.	Sur quel langage de programmation et design pattern repose Symfony ? 
86.	Quelle est la dernière version en date de Symfony ?
87.	Qu’est-ce qu’un bundle ? 
88.	Quel est le moteur de template utilisé par défaut dans Symfony ?
89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91.	Que permet le bundle Maker au sein de Symfony ? 
92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

## Sécurité
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

## RGPD
104.	Qu’est-ce que le RGPD ?
105.	Quel est son objectif principal ?
106.	Quelle est la date d’entrée en vigueur du RGPD ?
107.	Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
108.	En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
109.	Quel est le consentement valide selon le RPGD ?
110.	Qu’est-ce qu’une politique de confidentialité ?
111.	Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
112.	Quels sont les droits des utilisateurs selon le RGPD ?
113.	Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO
114.	Qu’est-ce que le SEO ? 
115.	Quel est l’objectif principal du SEO ?
116.	Existe-t-il plusieurs types de référencement ? Lesquels ?
117.	Qu’est-ce que la densité de mots-clés en SEO ?
118.	Qu’est-ce qu’une balise « alt » ?
119.	Qu’est-ce que la balise « meta description » ?
120.	Qu’est-ce que le « nofollow » en SEO ?
121.	Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
122.	Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
123.	Quelle est la recommandation pour les URL d'un site web bien référencé ?
124.	Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
125.	Qu'est-ce que l'optimisation des images pour le référencement ?
126.	Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

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
a.	Add interactive behavior and dynamic content <--- √
b.	Define the layout and design of web pages
c.	Handle server-side operations <--- √
2)	Which programming language is primarily used for server-side web development ?
a.	PHP <--- √
b.	JavaScript <--- √
c.	HTML <-- X
3)	What is the purpose of a web browser ?
a.	To render and display web pages <--- √
b.	To execute serve-side code
c.	To manage databases
4)	What is the difference between GET and POST methods in HTTP ?
a.	GET retrieves data from a server, while POST submits data to a server
b.	GET submits data to a server, while POST retrieves data from a server
c.	GET and POST methods are interchangeable
5)	What is the purpose of version control systems (e.g., Git) in web development ?
a.	To track changes and manage collaborative development
b.	To optimize website loading speed
c.	To handle server-side scripting
6)	What is the purpose of a framework in web development ?
a.	To provide a structured environment for building web applications
b.	To handle network protocols and data transfer
c.	To create visual designs and layouts for websites
7)	What does NoSQL stand for ?
a.	Not Only SQL
b.	Non-Structured Query Language
c.	New Object-Oriented Language
8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models
