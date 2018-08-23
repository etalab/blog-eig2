---
layout: post
modal-id: Le RNCS et l'Opendata
author: Pierre Camilleri, Christophe Ninucci
twitter: ChrisNinucci
description: Pour tous ceux qui manipulent des données financières, sachez que les bilans annuels déposés après le 1er janvier 2017 sont offerts en open data par l'INPI. Le format des données n'est aujourd'hui pas le plus attrayant, mais nous avons décidé dans le cadre de notre défi EIG de développer des outils permettant leur exploitation optimale par le plus grand nombre.
---



# Le RNCS en open data
Le RNCS (ou Registre National du Commerce et des Sociétés, aussi communément appelé registre InfoGreffe) est une base de données qui contient tous les comptes annuels des entreprises les ayant publiés, sur la base des dépôts obligatoires (mais avec des dispenses pour les plus petites entreprises) auprès des greffes de tribunaux de commerces. En fait de comptes annuels, on y trouve les bilans et comptes de résultats ainsi que les immatriculations, modifications et radiations des entreprises (RNCS IMR).  Ce registre de données publiques a été ouvert par décret en 2015, et rendu accessible début 2017. 

Le défi [« signaux faibles »](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/signauxfaibles/) est friand de données économique sur les entreprises et à ce titre le RNCS est une source de choix. L'institut national de la propriété intellectuelle (INPI) fournit  depuis le premier trimestre 2017 un service d'open data et offre ainsi gratuitement l'accès à l'ensemble des données économiques publiques des entreprises déposées depuis le premier janvier 2017.  Ces données sont [disponibles sur simple demande] (https://www.inpi.fr/fr/nationales/l-inpi-lance-l-ouverture-des-donnees-du-registre-du-commerce-et-des-societes). L'open data de l'INPI ne se limite d'ailleurs pas au RNCS mais distribue également toutes les données en rapport avec son métier premier, à savoir [les marques et les brevets](https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=JORFTEXT000029378451&categorieLien=id)

L'ouverture des données du RNCS fait suite au [décret n° 2015-1905 du 30 décembre 2015](https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=JORFTEXT000031741407) qui précise des modalités de transmission et de mise à disposition de ces données publiques. Ce texte a d'ailleurs donné lieu à une bataille juridique avec les greffes qui [n'a pas suffi à empêcher la confirmation de l'INPI dans son rôle de diffuseur](https://www.legifrance.gouv.fr/affichCodeArticle.do?cidTexte=LEGITEXT000005634379&idArticle=LEGIARTI000031821154&dateTexte=).

# Un accès aux données facile mais...
L'accès aux comptes annuels est entièrement gratuit, sous réserve d'acceptation d'une [licence à compléter](https://www.inpi.fr/sites/default/files/licence_rncs_comptes_annuels_mars_2017_0.pdf) et à renvoyer par mail à licences@inpi.fr. Suite à l'acceptation de la licence par l'INPI sont fournis des identifiants par retour de mail qui ouvrent l'accès à un serveur FTPS dont la structure est expliquée dans la [documentation](https://www.inpi.fr/fr/sites/default/files/doc_tech_comptes_annuels_decembre_2017_v1.4.pdf) qui est parfaitement à jour et fonctionnelle.

![Aperçu du dépot](/img/filezillaRncs.png)

Toutefois un [article Décodex du Monde](https://www.lemonde.fr/les-decodeurs/article/2018/06/22/comment-infogreffe-a-garde-la-main-sur-les-donnees-legales-des-entreprises_5319408_4355770.html) souligne que " les échantillons présentés [...] sont incompréhensibles pour un citoyen non averti, et relativement inexploitables sans un important retraitement pour une entreprise qui déciderait de les proposer à la consultation". Les fichiers, au [format XML](https://fr.wikipedia.org/wiki/Extensible_Markup_Language), ressemblent à l'échantillon présenté ci-dessous: 

![screenshot XML](/img/screenXML.png)

Ces fichiers sont effectivement difficiles à traiter dans un outil comme excel, toutefois il est à noter qu'il s'agit d'un format standard depuis plus de 20 ans et que de nombreuses librairies permettent de l'exploiter dans tous les langages de programmation. Autre écueil qui peut être rencontré pour exploiter ce format est l'utilisation d'une codification plutôt riche qu'il convient d'analyser avec la [documentation](https://www.inpi.fr/sites/default/files/doc_tech_comptes_annuels_decembre_2017_v1.4.pdf) fournie.

Un autre frein surprenant que nous avons rencontré consiste en un quota de téléchargement de 1Go par jour. Ainsi, le téléchargement de la base complète nécessite de s'y prendre à plusieurs reprises, ce qui devient une réelle gène à l'usage lorsqu'on met en perspective la structure du FTP qui ne permet pas d'identifier où trouver les fichiers correspondant à une entreprise sans en télécharger tout le contenu. Toutefois il est à noter que le volume total des fichiers présents dans les répertoires flux et historique représentent 2,2Go que l'on pourra donc obtenir en 3 sessions.

## Faciliter l'accès à l'information
Ce sont des données qui offrent des informations précieuses d'intelligence économique. L'accès à de telles informations était essentiellement payant avant  l'ouverture des données par l'INPI. Cette dernière sert la transparence financière des entreprises françaises, mais également un usage big data, sur l'intégralité des données, là où les services payants facturaient souvent à l'entreprise consultée, et donc limitaient l'exploitation de la base complète. Même si aujourd'hui, l'historique des comptes annuels est absent de la base offerte en open data, cette base de données se pose comme concurrente directe des alternatives payantes que sont par exemple la base Diane (Bureau Van Dijk, aujourd'hui filiale de Moody's Corporation), Ellisphère ou  Societe.com; offres payantes auxquelles souscrivent même les administrations françaises. 

Il nous semblait donc nécessaire de permettre un meilleur accès à l'information que les données contiennent pour faciliter leur réutilisation par le plus grand nombre. Nous avons  donc décidé dans le cadre de notre projet de développer des outils open source, qui contribuent à une mise en œuvre efficace de la politique d'open data menée par l'état français.

Dans le cadre de notre défi EIG, qui s'intègre dans la start-up d'État [Signaux Faibles](https://beta.gouv.fr/startup/signaux-faibles.html), nous utilisons en effet les données financières pour détecter des entreprises potentiellement fragiles, en vue de leur accompagnement par les services de l'État. L'anticipation des difficultés permet de mobiliser plus de leviers d'actions que lorsque les difficultés sont avérées, comme par exemple le renforcement des fonds propres. Pour cela nous croisons, entre autre, l'historique des données financières  avec les défaillances constatées par le passé (redressements et liquidations judiciaires) dans des algorithmes d'[apprentissage automatique](https://fr.wikipedia.org/wiki/Apprentissage_automatique). Même s'il nous manque l'historique de ces données pour totalement nous affranchir des sources de données payantes, nous sommes assurés que leur mise à jour future ne générera aucune dépense supplémentaire. Cela illustre comment l'ouverture des données ouvre la porte au développement de nouveaux services aux entreprises. 

Pour rendre ces données facilement accessibles plusieurs contraintes doivent être levées:
- Le format de fichier est un frein à l'exploitation pour tous les utilisateurs qui ne sauraient pas interpréter le format XML
- Les fichiers zip contenus sur le FTP ne permettent pas de discerner où trouver les informations relatives à une entreprise
- La codification des informations contenues dans les fichiers oblige à des aller-retours entre la documentation et les fichiers, rendant l'exploitation laborieuse

Pour répondre à ces contraintes, les outils proposés devront donc:
- Permettre la lecture et la transformation des fichiers dans un format plus habituel (csv)
- Gérer la réplication et la mise à jour d'un dépôt local pour permettre un accès rapide et illimité des données
- Permettre l'indexation de ce dépôt pour offrir une recherche dans les fichiers (par SIRET ou nom a minima)
- Traduire la codification des fichiers des comptes annuels avec des libellés en langage humain
- Être faciles à installer et à exploiter pour ne pas limiter la diffusion de ces outils à un public trop technique
- Prendre en compte les identifiants fournis par l'INPI et respecter le contrat de licence des utilisateurs

Nous pensons répondre à toutes ces contraintes en produisant une suite de 5 modules:
- **gorncs**: un module qui aura la tâche de traiter les opérations de maintien du dépôt et d'exploitation du format de fichier
- **gorncs-api**: un applicatif qui publiera une API REST sur votre réseau local pour exploiter les données
- **gorncs-cli**: un outil en ligne de commande pour effectuer des opérations de traitement de masse inconfortables via une API
- **rncs-ui**: une application web pour consulter facilement les données des entreprises
- **rrncs**: un module R pour importer les données du dépôt sous R

Nous intégrons dans nos contraintes que ce lot d'outil doit pouvoir être installé facilement par n'importe qui et offrir l'accès le plus large possible aux données mises à disposition par l'INPI. Notre réflexion se porte également sur d'autres sources de données à l'exploitation peu aisée telles que le BODACC qui met à disposition un historique conséquent au format XML sur data.gouv.fr et qui pourrait faire l'objet d'une intégration future dans la suite d'outil proposée ci-dessus.