---
layout: post
modal-id: Pérenniser un projet EIG - Retour sur le séminaire avec les DSI ministériels
author: L'équipe EIG (Bastien et Mathilde)
twitter: etalab
description: Mercredi 16 mai, entrepreneurs d'intérêt général et mentors venaient à la rencontre de leurs correspondants dans les directions des systèmes d'informations de leurs ministères. A l'occasion d'un atelier au Liberté Living Lab, ils ont réalisé un plan d'actions de pérennisation de leurs défis.
---

Les designers, datascientistes et développeurs du programme EIG produisent des livrables de nature très variée : des applications web, des interfaces de visualisation de données avec Rshiny ou Dataiku DSS, des bibliothèques logicielles, des guides d'exploitation, des manuels utilisateurs, des supports de formations internes, etc. Après leurs 10 mois d'immersion dans l'administration, l'enjeu est de **pérenniser ces livrables** au sein de leurs ministères d'accueil. Alors que nous sommes quasiment à mi-parcours de la Promotion 2, nous avons consacré un après-midi à un plan d'actions de pérennisation, partagé avec les DSI des ministères.

## Que veut dire « pérenniser » dans tous ces cas ?

Car, rappelons-le, la mission des EIG est double : il y a bien sûr la mise en oeuvre d'une solution technique à un problème identifié par l'administration, mais cette mise en oeuvre doit d'autre part être l'occasion pour l'administration d'aborder le numérique autrement : **mettre l'utilisateur au centre, tester tôt pour échouer tôt, ne pas hésiter à tester des technologies récentes, mettre autour de la table des services qui n'ont parfois pas l'habitude de se parler, favoriser une approche organique et en contact direct avec les métiers, etc.**

En étant ambitieux, la pérennisation concerne autant **le passage en production des livrables que l'élan de transformation numérique impulsé par la présence des EIG**. 

![La pyramide de la pérennisation imaginée par Bastien en amont de la session](/img/dsi-pyramide-perennisation.jpg)
*la pyramide de la pérennisation construite par Bastien en amont de la session*

**C'est pourquoi nous avons proposé de classer les enjeux de pérennisation selon trois axes :** 

- **Le déploiement (ou la mise en production)** : vers quel service se tourner pour réserver un nom de domaine ? Faut-il faire valider les briques open source sur lesquelles reposent les produits, et si oui, comment ? Mon administration propose-t-elle de faire tourner des services en production sous docker ? Etc. 

- **La transmission (ou le transfert de connaissances)** : ai-je donné tous les éléments à mon service pour qu'il gère la maintenance applicative des logiciels en place ? Ai-je donné le pourquoi et le comment de telle chaîne de traitement des données ? Est-ce que nous avons partagé nos supports de formation de telle façon qu'une autre personne pourra les reprendre ? 

- **La fiabilisation (ou résilience)** : si j'ai mis en oeuvre des méthodes de travail particulières (« agiles », mais pas que), qui est en mesure de continuer à les mettre en oeuvre ? Quelles sont les mesures à prendre si le livrable tombe en panne ? Si j'ai établi un point de contact avec des utilisateurs, qui sera le point de contact lorsque je ne serai plus dans le service ? Qui sera mainteneur pour les bibliothèques logicielles que j'ai publiées sur le Web ? 

Cette classification ne prétend pas couvrir toutes les actions réelles, elle permet aux équipes EIG d'identifier les difficultés à anticiper, de faire perdurer les produits et les valeurs instillés par les EIG. 

## Les bonnes pratiques de pérennisation : échanger régulièrement avec sa DSI, anticiper et s'adapter 

Avant d'élaborer ce plan d'actions de pérennisation par équipe de défis, Nicolas Joron, chef du bureau des études et du pilotage (qui gère la DSI du ministère de la Culture) et Patrick Chauffeton, chargé des référentiels techniques et sujets hébergement au sein de la DSI du Minitère de la Transition écologique et solidaire, ont partagé leur expérience en DSI ministérielle et quelques bonnes pratiques de pérennisation.

Pour Nicolas Joron, l'enjeu principal est d'être en mesure de détecter rapidement les aspects d'un projet numérique qui demanderont à la DSI de s'adapter une fois le projet prêt à être déployé. C'est pour cette raison que les mentors du défi Gobelins (rattaché au ministère de la Culture) ont eu le réflexe d'associer directement la DSI dans l'élaboration du défi et le recrutement des EIG. Des réunions ont lieu régulièrement entre DSI et EIG. Par ailleurs, dans un système d'information contraint, il est important d'inscrire au mieux les projets dans le cadre de cohérence technique, qui est bien sûr adaptable. En effet, les EIG apportent des langages nouveaux et enrichissent ainsi ce cadre de cohérence et la montée en compétences des DSI ministérielles.

![L'équipe EIG-mentor-DSI du MCC](/img/dsi-equipe-culture.jpg)
*Nicolas Joron, Hélène Cavalié, Laurie Chapotte et Ned Baldessin, une équipe EIG-mentor-DSI soudée !*

Pour Patrick Chauffeton, il est aussi crucial de travailler avec les équipes de développement dès le début d'un projet afin de partager les calendriers, apprendre mutuellement et s'entraider. Au ministère de la Transition écologique et solidaire, avec 300 systèmes d'information et une DSI de 500 personnes, l'activité est dense ! Définition des architectures, construction de référentiels techniques, cloud, etc... La bonne pratique : tester les projets au regard des référentiels et réaliser des audits de sécurité en amont !

## Quelques exemples d'actions de pérennisation prévues par les EIG

A partir de la pyramide de pérennisation, les équipes EIG-mentors-DSI ont identifié les différentes actions à mener, leurs niveaux d'urgence et d'importance et se sont alignées sur un calendrier d'actions. Cet "exercice" a été bénéfique selon les équipes : il permet en effet de penser la feuille de route globale des défis en fonction de cet enjeu de pérennisation, et ainsi de prioriser. Un aperçu des actions les plus mentionnées.

Pour la plupart des projets, deux actions semblent indispensables : **la documentation technique et la formation**. Par exemple, l'équipe [dataESR](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/dataesr/), prévoit de réaliser une documentation conséquente pour faciliter la prise en main des outils par l'équipe qui reprendra le devops. L'équipe imagine également la construction d'un système de rémontée des erreurs pour améliorer le service. L'équipe [Signaux Faibles](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/signauxfaibles/) doit également élaborer plusieurs guides (déploiement technique, exploitation, kit utilisateur) dans la mesure où Signaux Faibles a vocation à être déployer dans d'autres régions. L'équipe [Lab Santé](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/labsante/) pérennise en continu puisque des formations sont proposées à l'ensemble de la DREES sur les projets. 

![La matrice du défi Signaux Faibles](/img/20180517_SignauxFaibles.png)
*La feuille de route de pérennisation du défi Signaux Faibles, admirez le codage !*

Les enjeux **d'hébergement et de maintenance** sont également au coeur des actions. L'équipe [Prévisecours](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/previsecours/) a par exemple besoin d'anticiper le rapatriement du code sur le cloud, Bastien ([EIG Link](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/eiglink/)) doit prévoir le transfert de connaissances et la maintenace des différentes infrastructures mises à disposition (Github, serveur, etc.).

Au-delà de ces aspects techniques, les deux facteurs de pérennisation sont plutôt clairs : **la création d'une communauté et l'essaimage**. [SocialConnect](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/socialconnect/), qui transmettra le Carrefour des innovations sociales à un collectif associatif à l'issue de son développement, doit identifier une personnes qui animera la communauté et la communication autour du produit. [Archifiltre](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/archemse/) dispose de multiples opporunités pour faire vivre et enrichir leur produit - auprès d'autres ministères, dans des communautés d'archivistes, et même à l'étranger ! Pour [BaliseNAV](https://entrepreneur-interet-general.etalab.gouv.fr/defi/2017/09/26/balisenav/), il s'agira d'aller chercher des communautés de développeurs dans le ministère et auprès des navigateurs pour observer les usages de leurs outils.

*Petit clin d'oeil : la plupart des équipes défis sollicitent le recrutement d'un développeur comme action prioritaire*

A l'issue de cette session, plusieurs enseignements ont été retirés : les EIG connaissent mieux le métier et le quotidien des DSI ministérielles, les DSI ont exprimés leurs attentes et proposé des solutions de pérennisation aux équipes EIG. Et enfin, nous avons appris à utiliser d'Eisenhower (la preuve en image avec les sous-titres de Jean-Baptiste).

![La matrice du défi Signaux Faibles](/img/20180517_BrigadeNumerique2.png)
*la matrice d'Eisenhower : faire, déléguer, planifier, éliminer*

