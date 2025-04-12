---
title: Manifesto (French)
permalink: /fr/manifesto
nav_order: 3
---

# Manifeste de la Continuum Architecture

## Page de garde — *Continuum Architecture — Manifeste*

**Continuum Architecture — Manifeste**  
**Pour une architecture relationnelle, vivante et contextuelle**

* * *

**Version 1.0**  
**12 avril 2025**  
Document fondateur de la réflexion contextuelle en architecture logicielle  
Rédigé par **M. Stone**

* * *

> Ce manifeste propose un changement de posture fondamental :  
> penser le logiciel non comme un objet technique,  
> mais comme un événement orchestré entre un domaine et un contexte,  
> dans un instant donné, sous l’impulsion d’une intention.

* * *

(M. Stone est la signature architecturale de l'auteur Evens Pierre, utilisée pour véhiculer les idées de l'architecture Continuum sous une forme universelle et intemporelle.)

* * *

## Table des matières

- [Page de garde — Continuum Architecture — Manifeste](#page-de-garde-continuum-architecture-manifeste)
- [Table des matières](#table-des-matires)
- [1\. Préambule — Une industrie à repenser](#1-prambule-une-industrie-repenser)
- [2\. Définir les fondations — Domaine, Contexte, Application](#2-dfinir-les-fondations-domaine-contexte-application)
  - [Domaine](#domaine)
  - [Contexte](#contexte)
  - [Application](#application)
- [3\. Réhabiliter le contexte](#3-rhabiliter-le-contexte)
  -   [1\. La dimension de setup](#1-la-dimension-de-setup)
  -   [2\. La dimension d’intégration](#2-la-dimension-dintgration)
  -   [3\. La dimension d’initialisation](#3-la-dimension-dinitialisation)
- [4\. La posture du domaine dans le continuum](#4-la-posture-du-domaine-dans-le-continuum)
  -   [Le domaine face à l’incertitude](#le-domaine-face-lincertitude)
  -   [La dimension fonctionnelle du domaine](#la-dimension-fonctionnelle-du-domaine)
  -   [Un domaine humble, mais puissant](#un-domaine-humble-mais-puissant)
- [5\. Le continuum — Domaine et contexte sont indissociables](#5-le-continuum-domaine-et-contexte-sont-indissociables)
  -   [L’intention : la forme exprimée du besoin](#lintention-la-forme-exprime-du-besoin)
  -   [Une causalité claire : cause → effet](#une-causalit-claire-cause-effet)
  -   [Le principe d’incertitude contextuelle](#le-principe-dincertitude-contextuelle)
  -   [Le contexte comme superposition](#le-contexte-comme-superposition)
  -   [Le contexte est relatif, non absolu](#le-contexte-est-relatif-non-absolu)
  -   [Indépendants à la conception, indissociables à l’exécution](#indpendants-la-conception-indissociables-lexcution)
  -   [Les quatre dimensions fondamentales du continuum](#les-quatre-dimensions-fondamentales-du-continuum)
  -   [Note mathématique](#note-mathmatique)
  -   [Illustration concrète — Du concept à la mise en œuvre](#illustration-concrte-du-concept-la-mise-en-uvre)
  -   [Vers une nouvelle génération de cadres logiciels](#vers-une-nouvelle-gnration-de-cadres-logiciels)
- [6\. Principes fondateurs de la Continuum Architecture](#6-principes-fondateurs-de-la-continuum-architecture)
  -   [1\. Une application est un acte, pas un objet](#1-une-application-est-un-acte-pas-un-objet)
  -   [2\. L’intention est la forme causale de l’usage](#2-lintention-est-la-forme-causale-de-lusage)
  -   [3\. Le contexte est relatif, structuré et médié](#3-le-contexte-est-relatif-structur-et-mdi)
  -   [4\. Le domaine est autonome, abstrait, et orienté intention](#4-le-domaine-est-autonome-abstrait-et-orient-intention)
  -   [5\. L’architecture est une orchestration relationnelle](#5-larchitecture-est-une-orchestration-relationnelle)
  -   [6\. Le système est testable, évolutif et observable](#6-le-systme-est-testable-volutif-et-observable)
  -   [7\. Le continuum est un style architectural universel](#7-le-continuum-est-un-style-architectural-universel)
- [7\. Conclusion](#7-conclusion)
- [8\. Appel à l’action — Une nouvelle culture du logiciel](#8-appel-laction-une-nouvelle-culture-du-logiciel)
- [9\. Signature et licence](#9-signature-et-licence)
- [Postface — Ce manifeste comme point d’ancrage](#postface-ce-manifeste-comme-point-dancrage)

## 1\. Préambule — Une industrie à repenser

Depuis des décennies, l’industrie du logiciel avance à grands pas, portée par des progrès technologiques fulgurants. Mais dans cette course à la performance, à l’innovation et à la scalabilité, un élément fondamental a été relégué dans l’ombre : **le contexte.**

Nous avons appris à penser en termes de “domaines métier”, de “logiques d’affaires”, d’“entités” et de “comportements”, comme s’ils pouvaient exister dans l’absolu, indépendamment de leur environnement. Nous avons modélisé le monde dans des abstractions solides, souvent figées, sans interroger suffisamment le cadre dans lequel ces abstractions prennent vie. Nous avons construit des architectures qui se heurtent souvent à des difficultés lorsqu’elles rencontrent des variations concrètes : changement de plateforme, modification des exigences, migration de déploiement, évolution des usages.

**Trop souvent, nous confondons le code avec l'application.**  
Mais une application n’est pas une somme de fichiers. Ce n’est pas un framework. Ce n’est pas un serveur ou une interface.

> Une application est un acte : l’acte d’appliquer un savoir-faire (le **domaine**) à une situation concrète (le **contexte**), pour résoudre un problème réel.

**À partir de cette définition restaurée**, le terme “application” sera utilisé dans ce manifeste dans son sens originel et intentionnel.

Pour désigner ce que l’on appelait traditionnellement “application” dans l’industrie (c’est-à-dire un ensemble de fichiers, un programme, une interface, un backend ou un frontend), nous utiliserons désormais le terme **“système logiciel”**, ou “**système**” tout court pour faire simple.

> Une application est un acte.  
> Un système est la structure qui réunit un domaine et un contexte pour rendre cet acte possible.

C’est en partant de ce constat que la **Continuum Architecture** est née. Elle est une réponse directe à une série de dysfonctionnements systémiques :

- Une approche trop centrée sur le domaine, incapable de s’adapter élégamment à la diversité des contextes ;
- Une sur-ingénierie qui confond structure et rigidité, et qui sacralise des modèles figés ;
- Une industrie qui valorise la généralité abstraite au détriment de la spécificité concrète,  
l’universalité figée au détriment de l’usage contextualisé.

Nous croyons qu’il est temps de redéfinir ce que nous appelons une **application**.  
Nous croyons qu’il est temps de réhabiliter le **contexte** comme acteur de premier plan dans la conception logicielle.  
Nous croyons que le futur de l’architecture logicielle repose sur une compréhension fine de l’articulation entre **domaine et contexte**, sur leur **mise en relation fluide et adaptative**, sur ce que nous appelons **le continuum**.

Ce manifeste pose les bases de cette vision.

Chaque concept évoqué ici — domaine, contexte, application, système — sera défini précisément dans les sections suivantes, pour construire une fondation claire et partagée.

## 2\. Définir les fondations — Domaine, Contexte, Application

### **Domaine**

Le **domaine** est la **numérisation d’un besoin métier**, qu’il soit **opérationnel, organisationnel, économique ou social**.  
Il incarne la **logique métier**, c’est-à-dire la manière dont une activité humaine — vendre, soigner, organiser, apprendre, interagir — peut être **représentée et automatisée** dans un système informatique.

Il comprend les règles, les processus, les structures de données, les décisions, les comportements attendus — tout ce qui définit **ce que doit produire l’application pour répondre à un objectif métier**.

Le domaine est **abstrait par nature** : il n’est ni lié à une technologie, ni à un support d’exécution. Il **modélise un savoir-faire** que l’on souhaite rendre opérant à travers le logiciel.  
*(Ce savoir-faire peut prendre la forme de modules, de règles, de services ou d’interfaces — c’est une logique métier abstraite, indépendante de toute plateforme.)*

Mais ce savoir-faire, à lui seul, **n’est rien**. Il ne devient réel qu’au moment où il est **appliqué dans un contexte**.

> Le domaine est la réponse à un besoin.  
> Le contexte est la situation dans laquelle cette réponse prend vie.

* * *

### **Contexte**

Le **contexte** est plus qu’un environnement d’exécution. Il est **ce qui donne sens**.

Une même information, une même action, un même comportement peuvent avoir des significations radicalement différentes selon le contexte dans lequel ils apparaissent.  
Un mot, un geste, une donnée, un code source : **ce n’est pas leur nature intrinsèque qui compte, mais le cadre dans lequel ils s’inscrivent.**  
*(Le contexte ne se limite donc pas à un environnement technique — il inclut aussi les usages, les intentions, les contraintes et les acteurs en présence.)*

> C’est **le contexte qui transforme une donnée en information**, une règle en décision, une fonction en application.  
> Une phrase aussi simple que *“Il pleut”* n’a de sens que si l’on sait *où*, *quand*, *pour qui*.  
> En informatique, une instruction comme `x = 5` n’est qu’un octet isolé tant qu’on ne connaît pas *dans quel programme, à quel moment, pour quel usage* elle s’inscrit.

Dans un système logiciel, le contexte désigne **la situation réelle** dans laquelle le domaine va opérer. Cela inclut :

- Le **canal** (web, mobile, API, CLI…)
- Le **runtime** (navigateur, serveur, edge, cloud…)
- Les **utilisateurs** (leurs besoins, leurs rôles, leur culture)
- Les **contraintes techniques** (latence, sécurité, scalabilité…)
- Les **intégrations externes** (bases de données, services, capteurs…)
- Et tout élément **susceptible de modifier le sens et l’usage du domaine.**  
*(Autrement dit, tout n’est pas “contexte” — seuls les éléments qui influencent directement l’exécution, la signification ou la portée du domaine le sont.)*

Le contexte est **instable par nature**, souvent partiellement connu, parfois imprévisible. Et pourtant, c’est **lui qui détermine ce qu’il faut faire, comment, et pourquoi**.

Le domaine n’a de réalité opérationnelle **que dans un contexte donné**.  
Sans contexte, la logique métier reste théorique, **abstraite, non activée**.  
C’est pourquoi, dans la Continuum Architecture, le contexte n’est pas un paramètre secondaire : **c’est un citoyen de première classe.**  
*(Nous détaillerons dans la section suivante les différentes formes du contexte — externe, interne — ainsi que leur rôle dans l’architecture.)*

* * *

### **Application**

Le mot **application** vient du latin *applicatio*, du verbe *applicāre*, qui signifie :  
**« mettre en contact, situer près de, porter sur. »**

Ce sens originel est essentiel. Il révèle une vérité que l’industrie du logiciel a trop souvent oubliée :

> Une application n’est pas un objet, mais un **mouvement**, un **geste fondamental** : celui de **mettre un domaine en contact avec un contexte.**

La véritable question à poser n’est donc pas *"qu’est-ce qu’une application ?"*, mais **"qu’est-ce qui est mis en contact ?"**  
Et la réponse est simple : **le domaine et le contexte.**

Une **application** est l’acte d’appliquer un **savoir structuré (le domaine)** à une **situation réelle (le contexte)** dans le but de résoudre un problème.

> **Application = Domaine × Contexte → Résolution**  
> *(Cette formule sera précisée plus loin dans le manifeste — voir section 5, “Note mathématique”.)*

Ce geste rend les deux entités **indissociables** :

- Le domaine n’a **aucune valeur** sans un contexte pour le recevoir.
- Et le contexte n’a **aucune structure** sans un domaine pour s’y inscrire.

C’est la définition même d’un **continuum** :  
Une frontière floue, une interaction constante, une **interdépendance fonctionnelle**.

Une application ne fait pas “exister” un domaine, elle lui **offre un lieu pour s’exprimer**.  
Elle ne se contente pas d’exécuter un code : elle **met en scène une relation**, avec tout ce que cela implique de finesse, de temporalité, d’adaptation.

Une **bonne architecture logicielle** est précisément cela :

> **Une mise en scène réussie de la rencontre entre domaine et contexte.**  
> Elle orchestre cette rencontre dans toutes ses dimensions :

- **Techniques** (infrastructure, langages, protocoles)
- **Humaines** (utilisateurs, rôles, accessibilité)
- **Temporelles** (synchronisation, latence, durée de vie)
- **Économiques** (coût, rentabilité, valeur)

C’est cette vision qui fonde la **Continuum Architecture**.  
Nous ne concevons plus des objets logiciels fermés, mais des **relations orchestrées, vivantes et situées**.  
C’est cela, véritablement, **concevoir une application**.

## 3\. Réhabiliter le contexte

Le **contexte** est sans doute **l’un des grands oubliés de l’architecture logicielle contemporaine**.

Pendant des années, nous avons construit des modèles de domaines solides, des services bien encapsulés, des pipelines bien typés… mais **rarement des modèles explicites du contexte**.  
Nous l’avons relégué à la périphérie du système, traité comme un détail d’exécution, une variable d’environnement, un décor mouvant auquel on s’adapte “à la volée”.

> Pourtant, c’est le contexte qui détermine le sens, la portée, la faisabilité, la valeur même d’un domaine.

La **Continuum Architecture** propose de **repenser le contexte** en le structurant selon deux axes complémentaires :

- Le **contexte externe** : tout ce qui est **extérieur au système logiciel** — la plateforme, les utilisateurs, les événements, les requêtes, les bases de données, les services tiers.
- Le **contexte interne** : ce qui est **modélisé à l’intérieur** du système — le référentiel dans lequel le domaine s’exprime, raisonne et agit.

Le **contexte externe** est brut, variable, incertain, déterminé par des forces sur lesquelles le système n’a aucun contrôle.

> *On ne peut pas empêcher la pluie de tomber, mais on peut prendre son parapluie.*  
> L’architecture ne peut pas forcer l’environnement à se conformer à elle. Elle doit le **comprendre**, l’**accueillir**, et s’**en abstraire intelligemment**.

C’est ici qu’intervient la **dimension d’intégration**, qui fait le lien entre le contexte externe et le système logiciel.  
Elle n’est ni purement interne, ni strictement externe — c’est une **zone de médiation**, structurée par l’architecture.  
Elle est incarnée par un **adaptateur**, **conscient des deux contextes**, qui transforme une entrée extérieure en **intention**.

> L’**intention** est la **forme exprimée du besoin** : elle représente ce que l’acteur attend du système, dans un langage que celui-ci peut traiter.  
> *(Par exemple : “Créer un compte utilisateur à partir d’un formulaire web” est une intention — elle traduit un besoin humain en action déclenchable par le système.)*

L’adaptateur **normalise l’intention** et la transmet à la **dimension d’initialisation**, qui est seule responsable d’orchestrer l’exécution du domaine.

Le contexte interne, dans la Continuum Architecture, est structuré selon **trois dimensions fondamentales**.  
*(Chaque dimension du contexte interne joue un rôle spécifique dans l’orchestration du système — de sa configuration initiale jusqu’à l’activation du domaine face à une intention.*  
*Ce modèle en trois dimensions est une base minimale : il peut être étendu ou adapté selon les besoins spécifiques de l’application.)*

* * *

### **1\. La dimension de setup**

C’est le socle initial.  
Son rôle est de **construire un blueprint du système**, c’est-à-dire une représentation unifiée de tous ses éléments internes : modules, services, configurations, dépendances — qu’ils soient définis par l’utilisateur (développeur) ou issus de bibliothèques tierces.  
Ce blueprint peut être construit de manière **déclarative (par introspection)** ou **manuelle**, et constitue la **base d’enregistrement** de tous les composants nécessaires à la vie du système.  
*(Ce blueprint est une structure unifiée représentant tous les éléments internes nécessaires au fonctionnement du système — comme un registre de services, de modules, ou de configurations.)*

* * *

### **2\. La dimension d’intégration**

C’est le **point de contact avec l’extérieur**.  
Elle capte les entrées du contexte externe (événements, requêtes, signaux), les **traduit en intentions**, et les transmet à la suite du processus applicatif.  
C’est la **porte d’entrée de l’intention**, mais **elle ne déclenche pas directement l’exécution du domaine**.

* * *

### **3\. La dimension d’initialisation**

C’est le **cœur opérant du système**.  
C’est ici que le **domaine est chargé, préparé, activé**, en fonction du **blueprint** et de l’**intention** reçue.  
C’est à ce niveau que le **contexte interne croise réellement le domaine**, que la fonctionnalité prend vie, que la logique métier est instanciée, et que le besoin est comblé.

* * *

> Ce modèle tridimensionnel permet de **rendre le contexte interne visible, structuré et pilotable**, et de **maintenir une séparation forte avec le contexte externe**, tout en assurant une continuité fonctionnelle et intentionnelle.

* * *

Réhabiliter le contexte, ce n’est pas simplement le “prendre en compte”.  
C’est **le modéliser comme une entité vivante**, avec ses flux, ses formes, ses tensions — et faire de l’architecture logicielle **l’art d’orchestrer cette complexité**, avec lucidité, élégance et adaptabilité.

## 4\. La posture du domaine dans le continuum

Dans la Continuum Architecture, le **domaine** n’est pas marginalisé — il est **repositionné**.  
*(Rappelons ici que le mot “application” désigne l’acte d’appliquer un domaine à un contexte — pas un système ou un programme. Cette précision est essentielle pour bien comprendre la posture du domaine dans ce cadre.)*

Pendant des années, la plupart des efforts en architecture logicielle ont porté sur la **structuration du domaine** :

- Clean Architecture
- DDD (Domain-Driven Design)
- Onion, Hexagonal, Ports & Adapters…

Et à juste titre. Ces approches ont **posé des fondations solides**, notamment en matière de :

- Séparation des responsabilités
- Isolation du code métier
- Testabilité
- Ubiquitous language

Nous n’avons **aucune raison de les rejeter.**  
Au contraire : la Continuum Architecture **reconnaît leur valeur** et s’appuie sur elles.

Mais elle ajoute une chose essentielle :

> Le domaine ne fonctionne pas dans un vide.

* * *

### Le domaine face à l’incertitude

On entend souvent que le domaine ne doit “rien savoir du contexte”, voire qu’il doit “l’ignorer complètement”.  
Mais cette idée, poussée à l’extrême, mène à une impasse logique :

> **Comment un domaine pourrait-il s’exécuter dans un environnement dont il ne connaît ni la structure, ni les intentions, ni les contraintes ?**  
> **Comment transformer une intention en réponse si l’on prétend que l’intention vient de nulle part ?**

La Continuum Architecture propose une réponse nuancée et réaliste :

> Le domaine ne doit pas ignorer son contexte d’exécution.  
> Il doit rester **incertain** à son égard — non pas par ignorance, mais pour préserver son autonomie.  
> C’est cette **incertitude assumée** qui définit l’interface entre le **domaine et le contexte**.

Le domaine établit donc une **interface claire et abstraite** pour **recevoir des intentions** et **produire des effets**,  
sans savoir **qui**, **comment** ou **d’où** ces intentions proviennent.  
*(Cette interface peut prendre la forme de fonctions, de classes, ou de services exposés — elle définit les points d’entrée et de sortie formels du domaine, indépendamment de l’environnement technique.)*

* * *

### La dimension fonctionnelle du domaine

Cette interface est ce que la Continuum Architecture appelle **la dimension fonctionnelle**.  
*(Le mot “fonctionnelle” est ici utilisé dans le sens de **fonctionnalités métier**, pas dans le sens du paradigme de programmation fonctionnelle.)*

> Une couche claire, explicite, qui regroupe :
> 
> - Les **fonctionnalités exposées** par le domaine
> - Les **services internes** du domaine
> - Les **contrats d’entrée et de sortie** à travers lesquels il interagit avec le contexte

C’est cette dimension qui permet au domaine :

- De **préserver son autonomie**
- D’**accepter l’incertitude** comme un principe structurant
- Et de **rester opérationnel** dans des contextes multiples

* * *

### Un domaine humble, mais puissant

Nous ne mettons pas l’accent sur le domaine parce qu’il aurait perdu sa valeur —  
mais parce que **l’essentiel du travail d’abstraction y a déjà été fait**.

Le vrai déséquilibre aujourd’hui est ailleurs :

- On a souvent **surdéfini le domaine**,
- Et **ignoré le contexte**,
- Ou **laissé le lien entre les deux à des implémentations implicites**.

La Continuum Architecture **ne remplace pas le travail accompli sur le domaine** —  
elle **le réinscrit dans une dynamique relationnelle**,  
et lui donne **un environnement structuré, orchestré, cohérent** dans lequel s’exprimer.

Le domaine ne disparaît pas : il s’inscrit dans une dynamique nouvelle —  
**une relation orchestrée avec un contexte structuré**,  
dans laquelle il retrouve toute sa puissance expressive.

## 5\. Le continuum — Domaine et contexte sont indissociables

Le cœur de toute application n’est ni le domaine, ni le contexte.  
C’est la **relation vivante qui les unit**.  
*(C’est pourquoi l’application, dans ce manifeste, ne désigne jamais un objet technique : elle est l’acte émergent issu de cette relation, dans un instant donné.)*

Un lien de dépendance mutuelle, d’ajustement permanent, de résonance.

> C’est cette relation que la Continuum Architecture place au centre de toute conception logicielle : un **continuum.**

Le domaine ne peut fonctionner sans un contexte qui le **porte**.  
Le contexte ne prend forme que parce qu’un domaine vient **s’y inscrire**.  
L’un est le sens, l’autre est la situation. Ensemble, ils forment **l’application**.

* * *

### L’intention : la forme exprimée du besoin

Toute application commence par une **intention**.  
L’intention est le **désir d’un acteur** de provoquer un effet, de combler un besoin, de déclencher une action.  
Elle est produite à partir du **contexte externe**, et prend la forme d’une **cause abstraite** — un événement, une requête, une interaction — **interprétée et rendue intelligible par le système**.

> L’intention ne s’adresse pas directement au domaine.  
> Elle traverse le **contexte**, en passant par un **adaptateur**, et devient **compréhensible pour le système**.

Dans la Continuum Architecture, l’intention est **normalisée par la dimension d’intégration**, puis transmise à la dimension d’initialisation, qui active le domaine **au moment opportun**, selon les règles établies dans le blueprint.

* * *

### Une causalité claire : cause → effet

Il n’existe qu’une seule relation entre le **contexte externe** et le **système logiciel** :

> **Cause → Effet**  
> Une intention exprimée provoque une réaction du domaine, traduite en réponse.

*(Cette causalité n’est jamais directe : elle passe toujours par une médiation — l’adaptateur — qui transforme la cause brute en intention exploitable.)*

Mais cette causalité ne doit pas induire une dépendance.  
Le domaine **n’observe pas directement la cause**.  
Il **réagit à son abstraction**, orchestrée par le système.

C’est là toute la puissance du **principe d’incertitude contextuelle**.

* * *

### Le principe d’incertitude contextuelle

Ce principe stipule que :

> *Le domaine ne peut pas, en même temps, connaître de manière exacte son contexte d’exécution et évoluer indépendamment de lui.*

S’il connaît trop précisément le contexte, il lui devient **couplé**, rigide, non réutilisable.  
S’il l’ignore totalement, il **échoue à répondre** aux intentions.  
La solution : l’abstraction, la médiation, l’incertitude volontaire, orchestrée par le système.

* * *

### Le contexte comme superposition

Du point de vue du système, le **contexte externe est en état de superposition**.  
Toutes les plateformes, requêtes et sources d’entrée **existent en potentiel du point de vue du système**, tant qu’aucune d’elles n’a encore été intégrée, sélectionnée, ou effondrée.

C’est au **moment du runtime**, dans la **dimension d’intégration**, que l’intention est effondrée, normalisée, stabilisée, et devient un contexte interne **exploitable**.

> Cet effondrement contextuel — cette **décohérence** — est le point de rencontre entre le réel brut et le système logique.

* * *

### Le contexte est relatif, non absolu

Le contexte n’a de sens que **relativement à un référentiel**.  
Il ne peut être interprété **qu’à travers le point de vue du système**.

> Le **contexte** est relatif à un référentiel, tout comme la réalité l’est à l’observateur.

C’est pourquoi **le contexte interne est nécessaire** :  
Il constitue **ce référentiel stable**, dans lequel les intentions peuvent être comprises, et les logiques activées.

* * *

### Indépendants à la conception, indissociables à l’exécution

Le **domaine** et le **contexte** peuvent — et doivent — être **conçus indépendamment**.  
Ils relèvent de disciplines différentes, de cycles de vie différents, de responsabilités différentes.

Mais ils ne peuvent **exister en acte** qu’à travers leur **rencontre**.  
C’est cette **rencontre, orchestrée dans un instant donné**, qui **fait naître l’application**.

> L’application n’est pas un objet figé.  
> C’est **un événement**, un **point d’interaction**, un **moment de convergence**.

À ce titre, domaine et contexte forment un **continuum**, à la manière de l’espace et du temps.  
Indépendants dans la théorie, **mais indissociables dans la réalité.**  
Leur interaction produit quelque chose de nouveau :

> une dynamique, une intention réalisée, une réalité numérique vivante.

C’est **dans ce point de jonction**, cette **orchestration consciente de leur interaction**, que réside **le vrai rôle de l’architecture**.

> **Concevoir une application, c’est concevoir un événement dans le continuum.**  
> **Autrement dit, l’architecture est ce qui rend possible la rencontre contrôlée entre domaine et contexte dans un instant donné.**

* * *

### Les quatre dimensions fondamentales du continuum

Au final, la Continuum Architecture repose sur **quatre dimensions fondamentales** :

- **Trois contextuelles** : `setup`, `integration`, `initialization` — qui modélisent la structure du contexte interne et orchestrent la rencontre avec l’extérieur ;
- **Une fonctionnelle** : qui héberge le domaine, ses services, et son interface d’exploitation.

Le domaine est donc une **dimension à part entière**, mais nous choisissons de ne pas en faire un sujet central, car les architectures existantes (DDD, Clean Architecture, Hexagonal, etc.) l’ont déjà largement exploré.  
Notre attention se porte plutôt sur l’**orchestration du domaine dans le contexte** — car c’est là que réside le **véritable angle mort** de l’architecture logicielle contemporaine.

* * *

### Note mathématique

En termes mathématiques, on peut voir une application comme un **produit cartésien** :

> **Application = Domaine × Contexte**

Ce produit ne représente pas simplement un ensemble de composants, mais un **couple (contexte, domaine)** dont l’interaction produit un **résultat**.

En ce sens, lorsque certains affirment *« cette application est un produit »*, ils sont plus précis qu’ils ne le pensent :  
C’en est véritablement un — un **produit dynamique** entre un **savoir structuré (le domaine)** et une **situation réelle (le contexte)**, donnant lieu à une **résolution**.

* * *

### Illustration concrète — Du concept à la mise en œuvre

La Continuum Architecture propose une vision conceptuelle forte, mais elle s’ancre aussi dans des réalités concrètes, observables dans tout système logiciel moderne.

Voici comment ses concepts fondamentaux peuvent se **traduire en implémentation** :

- Le **contexte externe** peut être incarné par l’**environnement d’exécution** du système : un navigateur, un serveur bare-metal, une fonction cloud (Lambda), un terminal CLI, un capteur IoT…
- Le **contexte interne**, lui, est souvent **implémenté sous la forme d’un framework** : un environnement structurant qui orchestre la configuration (setup), les points d’entrée (intégration), et l’exécution du domaine (initialisation).
- Le **domaine** représente la **logique métier** pure : des services, règles, modules ou modèles définis par l’équipe applicative, indépendants du cadre technique.
- L’**intention**, enfin, peut se manifester par une **requête HTTP**, une interaction utilisateur, un événement système, une ligne de commande… Elle est l’expression causale d’un besoin, structurée pour être interprétée.

> Le rôle du système est alors de capter cette intention, de l’interpréter à travers son contexte interne, et d’activer le domaine pour produire un effet.

* * *

### Vers une nouvelle génération de cadres logiciels

La Continuum Architecture ne se limite donc pas à organiser la relation entre un domaine et un contexte.  
Elle propose un **style architectural pour construire les systèmes eux-mêmes** —  
des **environnements capables de porter des applications** au sens fort du terme :  
des actes intentionnels et contextuels.

> Le continuum n’est pas uniquement un modèle pour concevoir des relations entre domaines et contextes,  
> c’est une architecture pour construire des **systèmes capables de porter des applications** —  
> c’est-à-dire : des frameworks.

Dans un monde où chaque framework impose sa propre logique implicite, le continuum offre une **grille de lecture universelle**, intentionnelle, et extensible.  
Il permet de bâtir des cadres logiciels **fondés sur la relation**, plutôt que sur la structure seule —  
des systèmes conçus pour **mettre en scène des applications**, avec élégance, clarté et adaptabilité.

## 6\. Principes fondateurs de la Continuum Architecture

### 1\. **Une application est un acte, pas un objet**

L’application n’est pas un artefact technique.  
Elle est l’**acte vivant** d’appliquer un domaine à un contexte pour produire une résolution.  
Elle naît d’une **intention exprimée**, se manifeste dans un **instant donné**, et s’éteint une fois l’effet accompli.

Ce n’est ni un fichier, ni un service, ni une interface.  
C’est une **rencontre orchestrée entre un savoir-faire (le domaine) et une situation (le contexte)**.

* * *

### 2\. **L’intention est la forme causale de l’usage**

Toute application est déclenchée par une **intention** : un besoin formulé dans un langage que le système peut comprendre.

L’intention est une **cause abstraite**, produite à partir du contexte externe, normalisée par un adaptateur, et transmise au domaine.  
Elle est le **point de départ** de toute exécution, de toute dynamique, de toute architecture.

Le système ne réagit pas à des événements bruts, mais à des **intentions interprétées**.

* * *

### 3\. **Le contexte est relatif, structuré et médié**

Le **contexte externe** est instable, imprévisible, en superposition —  
il devient exploitable uniquement lorsqu’il est **interprété à travers un contexte interne**.

Ce **contexte interne**, structuré en dimensions (`setup`, `integration`, `initialization`), sert de **référentiel stable** pour comprendre, transformer et activer les intentions.

Le contexte n’est pas un environnement passif.  
Il est **acteur**, **filtre**, **cadre d’interprétation**.  
Il est toujours **relatif à un système** qui l’observe.

* * *

### 4\. **Le domaine est autonome, abstrait, et orienté intention**

Le domaine **n’ignore pas son environnement**.  
Il agit avec une **incertitude maîtrisée**, encadrée par une interface abstraite.

Il ne s’exécute que lorsqu’il reçoit une intention compatible, portée par le contexte interne.  
Sa structure est indépendante de la plateforme, du transport, et de l’infrastructure.

> Il n’est pas isolé du contexte —  
> Il est **incertain vis-à-vis de lui**, et structuré pour y répondre.

* * *

### 5\. **L’architecture est une orchestration relationnelle**

L’architecture n’est pas qu’une pile de couches.  
C’est une **intelligence organisatrice** qui orchestre la rencontre entre domaine et contexte, dans un **point d’interaction contrôlé**.

Elle structure le système en **dimensions claires** :

- Configuration (`setup`)
- Réception des intentions (`integration`)
- Activation métier (`initialization`)
- Exposition fonctionnelle (`domaine`)

Elle ne relie pas des blocs : elle **met en scène une dynamique vivante et intentionnelle**.

* * *

### 6\. **Le système est testable, évolutif et observable**

La séparation entre contexte externe, contexte interne, intention et domaine rend le système :

- **Testable par dimension**
- **Évolutif sans fracture**
- **Observable en continu**

Chaque intention, chaque effet, chaque échec peut être **suivi, compris, reproduit**.  
Le système devient un **instrument interprétable**, pas une boîte noire.

* * *

### 7\. **Le continuum est un style architectural universel**

Le continuum ne définit pas seulement une manière de construire des applications.  
Il propose un style pour concevoir **des systèmes capables d’orchestrer des applications** :  
des **frameworks orientés relation**, contextuels, adaptables, intentionnels.

Dans une industrie saturée de structures figées, la Continuum Architecture recentre l’attention sur **la dynamique d’usage**, **la souplesse contextuelle**, et **l’intelligibilité du code vivant**.

> Ce n’est pas une architecture de composants.  
> C’est une architecture de **rencontres**.

## 7\. Conclusion

Ce manifeste ne propose pas un nouveau cadre à la mode.  
Il propose un **changement de perspective fondamental** :  
replacer le **contexte** au centre de la conception logicielle.

Pendant trop longtemps, nous avons conçu des logiciels comme des structures figées,  
coupées de leur environnement réel, incapables de s’adapter, d’évoluer ou de dialoguer avec l’usage.

Nous avons pensé le système comme une mécanique interne, autonome,  
alors qu’il n’est, en réalité, qu’un **espace d’interaction entre ce que l’on sait et ce que l’on affronte.**

Ce manifeste propose une réponse simple mais structurante :  
penser le logiciel non plus comme un objet,  
mais comme un **événement situé**,  
une **relation orchestrée** entre un **domaine** et un **contexte**,  
dans un **instant donné**, provoquée par une **intention**.

La Continuum Architecture est à la fois :

- Une **grille de lecture** : pour comprendre les systèmes dans leur dynamique réelle ;
- Une **structure d’exécution** : pour articuler les intentions, les dimensions et les effets ;
- Un **style architectural** : pour construire des systèmes capables de porter des applications vivantes.

> C’est un appel à repenser ce que signifie **construire un système**.  
> Non plus autour de blocs techniques, mais autour de **relations orchestrées** entre ce que l’on sait (le domaine) et ce que l’on vit (le contexte).  
> Non plus pour répondre à une spécification figée, mais pour **accueillir l’incertitude, l’usage, l’évolution.**

C’est une invitation à imaginer et construire des systèmes **plus souples**, **plus lisibles**, **plus vivants**.  
Des systèmes **orientés contexte**.  
Des systèmes **humains**.

## 8\. Appel à l’action — Une nouvelle culture du logiciel

La Continuum Architecture **n’est pas une méthode**.  
Ce n’est pas un cadre rigide, ni un outil prêt à l’emploi.  
Elle ne vous dira pas *comment structurer vos fichiers* ou *quel outil adopter*.

> C’est un **changement de regard**, un **changement de posture**, un **changement de culture**.

Elle nous invite à penser le logiciel comme un **espace d’interaction vivante**,  
où un **domaine** rencontre un **contexte**,  
dans un **instant donné**, sous l’impulsion d’une **intention**.

Non comme une solution fermée, mais comme une **rencontre orchestrée**.  
Non comme un code isolé, mais comme un **acte vivant, situé, intentionnel**.

* * *

Nous appelons donc :

- Les **développeurs** à modéliser le **contexte** avec autant de soin que le domaine.
- Les **architectes** à structurer le système autour des **intentions** et des **points de convergence**.
- Les **formateurs** à enseigner la **séparation entre contexte externe et contexte interne**.
- Les **concepteurs de frameworks** à rendre **explorables et explicites** les dimensions cachées du contexte.
- Les **équipes produit** à interroger leurs **modèles mentaux**, leurs **outils**, leurs **habitudes**.
- Et l’**industrie entière** à redonner au contexte la place qu’il mérite : **au cœur**.

* * *

Si vous concevez une **CLI**, un **backend**, une **application mobile**, un **microservice**,  
si vous développez des **modèles IA**, des **architectures serverless**, des **systèmes événementiels**,  
si vous bâtissez des **frameworks**, des **plateformes**, ou des **environnements d’exécution**…

> Alors vous êtes concerné par la question du **contexte**.  
> Et vous avez le pouvoir de **transformer votre manière d’architecturer le logiciel**.

* * *

Ce manifeste n’est qu’un **point de départ**.

Le reste dépend de ce que nous allons :  
**implémenter, transmettre, enseigner, documenter, partager, faire évoluer.**

Le **continuum** n’est pas une fin.  
C’est un **socle**, un **langage**, un **champ de transformation**.

> Il ne s’agit pas de suivre un nouveau standard.  
> Il s’agit de **changer notre manière de concevoir la technologie**.  
> Et peut-être, d’en changer **la culture**.

## 9\. Signature et licence

Ce manifeste a été rédigé par **Evens Pierre**,  
sous la signature architecturale de **M. Stone**,

d’années de réflexion, de conception, et de pratique autour de l’architecture logicielle contextuelle.

Il a été finalisé le **12 avril 2025**,  
et publié sous la licence **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

Cela signifie que :

- Vous êtes libres de le **partager**, le **reproduire**, le **traduire**, l’**adapter**
- Y compris à des fins **commerciales**
- À condition de **créditer l’auteur original** et de **lier vers la licence**

Licence complète : [Attribution 4.0 International — Creative Commons](https://creativecommons.org/licenses/by/4.0/)

* * *

**Pour toute question, retour ou contribution**,  
merci d’utiliser l’espace collaboratif dédié sur GitHub :  
[https://github.com/evens-stone/continuum-manifesto/issues](https://github.com/evens-stone/continuum-manifesto/issues)

## Postface — *Ce manifeste comme point d’ancrage*

Ce manifeste n’est pas né d’un brainstorming passager.  
Il est le fruit d’un long travail d’observation, d’expérience, de confrontation au réel.

Il est né de systèmes que l’on croyait bien conçus mais qui s’effondraient au moindre changement de contexte.  
De frameworks puissants mais opaques.  
D’architectures solides mais figées.  
De besoins exprimés que l’on ne savait plus entendre.

Il est né aussi d’une intuition :  
Et si le problème n’était pas dans **le code**, mais dans **notre manière de penser le code** ?  
Et si la solution résidait dans ce que nous avons trop longtemps mis de côté :  
le **contexte** ?

* * *

Ce texte n’a pas vocation à imposer un nouveau dogme.  
Il a vocation à **révéler ce qui était déjà là**, mais que nous n’avions pas encore su nommer.

Il est une **structure mentale**, une **boussole conceptuelle**, un **socle commun pour penser différemment**.

* * *

La suite appartient à celles et ceux qui décideront de porter cette vision dans le réel.  
Dans les outils.  
Dans les équipes.  
Dans la documentation.  
Dans la pédagogie.  
Dans les lignes de code.

Si vous vous reconnaissez dans cette manière de concevoir le logiciel —  
alors ce manifeste est à vous.