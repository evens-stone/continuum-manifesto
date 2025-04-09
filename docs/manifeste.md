# Manifeste de la Continuum Architecture

Je Ceci représente le manifeste de la **Continuum Architecture**

- [1\. Préambule — Une industrie à repenser](#1-prambule-une-industrie-repenser)
- [2\. Définir les fondations — Domaine, Contexte, Application](#2-dfinir-les-fondations-domaine-contexte-application)
-   [Domaine](#domaine)
-   [Contexte](#contexte)
-   [Application](#application)
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
- [6\. Principes fondateurs de la Continuum Architecture](#6-principes-fondateurs-de-la-continuum-architecture)
- [7\. Appel à l’action — Une nouvelle culture du logiciel](#7-appel-laction-une-nouvelle-culture-du-logiciel)
- [8\. Signature et licence](#8-signature-et-licence)

## 1\. Préambule — Une industrie à repenser

Depuis des décennies, l’industrie du logiciel avance à grands pas, portée par des progrès technologiques fulgurants. Mais dans cette course à la performance, à l’innovation et à la scalabilité, un élément fondamental a été relégué dans l’ombre : **le contexte.**

Nous avons appris à penser en termes de “domaines métier”, de “logiques d’affaires”, d’“entités” et de “comportements”, comme s’ils pouvaient exister dans l’absolu, indépendamment de leur environnement. Nous avons modélisé le monde dans des abstractions solides, souvent figées, sans interroger suffisamment le cadre dans lequel ces abstractions prennent vie. Nous avons construit des architectures qui prétendent être universelles, mais qui échouent dès qu’elles sont confrontées à des variations concrètes : changement de plateforme, modification des exigences, migration de déploiement, évolution des usages.

**Trop souvent, nous confondons le code avec l'application.**  
Mais une application n’est pas une somme de fichiers. Ce n’est pas un framework. Ce n’est pas un serveur ou une interface. Une application est un **acte** : l’acte d’appliquer un savoir-faire (le **domaine**) à une situation concrète (le **contexte**), pour résoudre un problème réel.

**À partir de cette définition restaurée, le terme “application” sera utilisé dans ce manifeste dans son sens originel et intentionnel.**

Pour désigner ce que l’on appelait traditionnellement “application” dans l’industrie (c’est-à-dire un ensemble de fichiers, un programme, une interface, un backend ou un frontend), nous utiliserons désormais le terme “système logiciel” ou “**système**” tout court pour faire simple.

> Une application est un acte.
> 
> Un système est ce qui permet son exécution

C’est en partant de ce constat que la **Continuum Architecture** est née. Elle est une réponse directe à une série de dysfonctionnements systémiques :

- Une approche trop centrée sur le domaine, incapable de s’adapter élégamment à la diversité des contextes ;
- Une sur-ingénierie qui confond structure et rigidité, et qui sacralise des modèles figés ;
- Une industrie qui valorise la généralité abstraite au détriment de la spécificité concrète,  
l’universalité figée au détriment de l’usage contextualisé.

Nous croyons qu’il est temps de redéfinir ce que nous appelons une **application**.  
Nous croyons qu’il est temps de réhabiliter le **contexte** comme acteur de premier plan dans la conception logicielle.  
Nous croyons que le futur de l’architecture logicielle repose sur une compréhension fine de l’articulation entre **domaine et contexte**, sur leur **mise en relation fluide et adaptative**, sur ce que nous appelons **le continuum**.

Ce manifeste pose les bases de cette vision.

## 2\. Définir les fondations — Domaine, Contexte, Application

### **Domaine**

Le **domaine** est la **numérisation d’un besoin métier**, qu’il soit **opérationnel, organisationnel, économique ou social**.  
Il incarne la **logique métier**, c’est-à-dire la manière dont une activité humaine — vendre, soigner, organiser, apprendre, interagir — peut être **représentée et automatisée** dans un système informatique.

Il comprend les règles, les processus, les structures de données, les décisions, les comportements attendus — tout ce qui définit **ce que doit produire l’application pour répondre à un objectif métier**.

Le domaine est **abstrait par nature** : il n’est ni lié à une technologie, ni à un support d’exécution. Il **modélise un savoir-faire** que l’on souhaite rendre opérant à travers le logiciel.

Mais ce savoir-faire, à lui seul, **n’est rien**. Il ne devient réel qu’au moment où il est **appliqué dans un contexte**.

> Le domaine est la réponse à un besoin.  
> Le contexte est la situation dans laquelle cette réponse prend vie.

### **Contexte**

Le **contexte** est plus qu’un environnement d’exécution. Il est **ce qui donne sens**.

Une même information, une même action, un même comportement peuvent avoir des significations radicalement différentes selon le contexte dans lequel ils apparaissent.  
Un mot, un geste, une donnée, un code source : **ce n’est pas leur nature intrinsèque qui compte, mais le cadre dans lequel ils s’inscrivent.**

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

Le contexte est **instable par nature**, souvent partiellement connu, parfois imprévisible. Et pourtant, c’est **lui qui détermine ce qu’il faut faire, comment, et pourquoi**.

Le domaine n’a de réalité opérationnelle **que dans un contexte donné**.  
Sans contexte, la logique métier reste théorique, **abstraite, non activée**.  
C’est pourquoi, dans la Continuum Architecture, le contexte n’est pas un paramètre secondaire : **c’est un citoyen de première classe**.

### **Application**

Le mot **application** vient du latin *applicatio*, du verbe *applicāre*, qui signifie :  
**« mettre en contact, situer près de, porter sur. »**

Ce sens originel est essentiel. Il révèle une vérité que l’industrie du logiciel a trop souvent oubliée :

> Une application n’est pas un objet, mais un **mouvement**, un **geste fondamental** : celui de **mettre un domaine en contact avec un contexte**.

La véritable question à poser n’est donc pas *"qu’est-ce qu’une application ?"*, mais **"qu’est-ce qui est mis en contact ?"**  
Et la réponse est simple : **le domaine et le contexte.**

Une **application** est l’acte d’appliquer un **savoir structuré (le domaine)** à une **situation réelle (le contexte)** dans le but de résoudre un problème.

> **Application = Domaine × Contexte → Résolution**

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

## 3\. **Réhabiliter le contexte**

Le **contexte** est sans doute **l’un des grands oubliés de l’architecture logicielle contemporaine**.

Pendant des années, nous avons construit des modèles de domaines solides, des services bien encapsulés, des pipelines bien typés… mais **rarement des modèles explicites du contexte**.  
Nous l’avons relégué à la périphérie du système, traité comme un détail d’exécution, une variable d’environnement, un décor mouvant auquel on s’adapte “à la volée”.

> Pourtant, c’est le contexte qui détermine le sens, la portée, la faisabilité, la valeur même d’un domaine.

La Continuum Architecture propose de **repenser le contexte** en le structurant selon deux axes complémentaires :

- Le **contexte externe** : tout ce qui est **extérieur à l’application** — la plateforme, les utilisateurs, les événements, les requêtes, les bases de données, les services tiers.
- Le **contexte interne** : ce qui est **modélisé à l’intérieur** de l’application — le référentiel dans lequel le domaine s’exprime, raisonne et agit.

Le **contexte externe** est brut, variable, incertain, déterminé par des forces sur lesquelles l’application n’a aucun contrôle.

> *On ne peut pas empêcher la pluie de tomber, mais on peut prendre son parapluie.*  
> L’architecture ne peut pas forcer l’environnement à se conformer à elle. Elle doit le **comprendre**, l’**accueillir**, et s’**en abstraire intelligemment**.

C’est ici qu’intervient la **dimension d’intégration**, **le médium entre le contexte interne et le contexte externe**.  
Elle est incarnée par un **adaptateur**, **conscient des deux contextes**, qui transforme une entrée extérieure en **intention**.

> L’**intention** est la **forme exprimée du besoin** : elle représente ce que l’acteur attend de l’application, dans un langage que celle-ci peut traiter.

Il **normalise l’intention** et la transmet à la **dimension d’initialisation**, qui est seule responsable d’orchestrer l’exécution du domaine.

Le contexte interne, dans la Continuum Architecture, est structuré selon **trois dimensions fondamentales** :

#### **1\. La dimension de setup**

C’est le socle initial.  
Son rôle est de **construire un blueprint de l’application**, c’est-à-dire une représentation unifiée de tous ses éléments internes : modules, services, configurations, dépendances — qu’ils soient définis par l’utilisateur(développeur) ou issus de bibliothèques tierces.  
Ce blueprint peut être construit de manière **déclarative(par introspection) ou manuelle**, et constitue la **base d’enregistrement** de tous les composants nécessaires à la vie de l’application.

#### **2\. La dimension d’intégration**

C’est le **point de contact avec l’extérieur**.  
Elle capte les entrées du contexte externe (événements, requêtes, signaux), les **traduit en intentions**, et les transmet à la suite du processus applicatif.  
C’est la **porte d’entrée de l’intention**, mais **elle ne déclenche pas directement l’exécution du domaine**.

#### **3\. La dimension d’initialisation**

C’est le **cœur opérant de l’application**.  
C’est ici que le **domaine est chargé, préparé, activé**, en fonction du **blueprint** et de l’**intention** reçue.  
C’est à ce niveau que le **contexte interne croise réellement le domaine**, que la fonctionnalité prend vie, que la logique métier est instanciée, et que le besoin est comblé.

* * *

> Ce modèle tridimensionnel permet de **rendre le contexte interne visible, structuré et pilotable**, et de **maintenir une séparation forte avec le contexte externe**, tout en assurant une continuité fonctionnelle et intentionnelle.

Réhabiliter le contexte, ce n’est pas simplement le “prendre en compte”.  
C’est **le modéliser comme une entité vivante**, avec ses flux, ses formes, ses tensions — et c’est faire de l’architecture logicielle **l’art d’orchestrer cette complexité**, avec lucidité, élégance et adaptabilité.

## 4\. **La posture du domaine dans le continuum**

Dans la Continuum Architecture, le **domaine** n’est pas marginalisé — il est **repositionné**.

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

### **Le domaine face à l’incertitude**

On entend souvent que le domaine ne doit "rien savoir du contexte", voire qu’il doit "l’ignorer complètement".  
Mais cette idée, poussée à l’extrême, mène à une impasse logique :

> **Comment un domaine pourrait-il s’exécuter dans un environnement dont il ne connaît ni la structure, ni les intentions, ni les contraintes ?**  
> **Comment transformer une intention en réponse si l’on prétend que l’intention vient de nulle part ?**

La Continuum Architecture propose une réponse nuancée et réaliste :

> Le domaine **ne connaît pas** le contexte,  
> mais il est **conscient de son incertitude** vis-à-vis de lui.  
> Et c’est précisément **cette incertitude** qui fonde **l’interface** entre les deux.

Le domaine établit donc une **interface claire et abstraite** pour **recevoir des intentions** et **produire des effets**,  
sans savoir **qui**, **comment** ou **d’où** ces intentions proviennent.

> Il ne traite pas le contexte comme une ignorance totale,  
> mais comme une **zone d’incertitude maîtrisée**, **encapsulée**, **contractuelle**.

* * *

### **La dimension fonctionnelle du domaine**

Cette interface est ce que la Continuum Architecture appelle **la dimension fonctionnelle** :

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

### **Un domaine humble, mais puissant**

Nous ne mettons pas l’accent sur le domaine parce qu’il aurait perdu sa valeur —  
mais parce que **l’essentiel du travail d’abstraction y a déjà été fait**.

Le vrai déséquilibre aujourd’hui est ailleurs :

- On a souvent **surdéfini le domaine**,
- Et **ignoré le contexte**,
- Ou **laissé le lien entre les deux à des implémentations implicites**.

La Continuum Architecture **ne remplace pas le travail accompli sur le domaine** —  
elle **le réinscrit dans une dynamique relationnelle**,  
et lui donne **un environnement structuré, orchestré, cohérent** dans lequel s’exprimer.

## 5\. **Le continuum — Domaine et contexte sont indissociables**

Le cœur de toute application n’est ni le domaine, ni le contexte.  
C’est la **relation vivante qui les unit.**  
Un lien de dépendance mutuelle, d’ajustement permanent, de résonance.

> C’est cette relation que la Continuum Architecture place au centre de toute conception logicielle : un **continuum.**

Le domaine ne peut fonctionner sans un contexte qui le **porte**.  
Le contexte ne prend forme que parce qu’un domaine vient **s’y inscrire**.  
L’un est le sens, l’autre est la situation. Ensemble, ils forment **l’application.**

* * *

### **L’intention : la forme exprimée du besoin**

Toute application commence par une **intention**.  
L’intention est le **désir d’un acteur** de provoquer un effet, de combler un besoin, de déclencher une action.  
Elle est **portée par le contexte externe**, et prend la forme d’une **cause** : un événement, une requête, une interaction, une commande.

> L’intention ne s’adresse pas directement au domaine.  
> Elle traverse le **contexte**, en passant par un **adaptateur**, et devient **compréhensible pour l’application**.

Dans la Continuum Architecture, l’intention est **normalisée par la dimension d’intégration**, puis transmise à la dimension d’initialisation, qui active le domaine **au moment opportun**, selon les règles établies dans le blueprint.

* * *

### **Une causalité claire : cause → effet**

Il n’existe qu’une seule relation entre le **contexte externe** et le **système applicatif** :

> **Cause → Effet**  
> Une intention exprimée provoque une réaction du domaine, traduite en réponse.

Mais cette causalité ne doit pas induire une dépendance.  
Le domaine **n’observe pas directement la cause**.  
Il **réagit à son abstraction**, orchestrée par l’adaptateur.  
C’est là toute la puissance du **principe d’incertitude contextuelle**.

* * *

### **Le principe d’incertitude contextuelle**

Ce principe stipule que :

> *Le domaine ne peut pas, en même temps, connaître de manière exacte son contexte d’exécution et évoluer indépendamment de lui.*

S’il connaît trop précisément le contexte, il lui devient **couplé**, rigide, non réutilisable.  
S’il l’ignore totalement, il **échoue à répondre** aux intentions.  
La solution : l’abstraction, la médiation, l’incertitude volontaire, orchestrée par le système.

* * *

### **Le contexte comme superposition**

Du point de vue de l’application, le **contexte externe est en état de superposition**.  
Toutes les plateformes, requêtes, sources d’entrée **existent en potentiel** — tant que l’application n’a pas encore exécuté la logique.  
C’est au **moment du runtime**, dans la **dimension d’intégration**, que l’intention est effondrée, normalisée, stabilisée, et devient un contexte interne **exploitable**.

> Cet effondrement contextuel — cette **décohérence** — est le point de rencontre entre le réel brut et le système logique.

* * *

### **Le contexte est relatif, non absolu**

Le contexte n’existe jamais “en soi”.  
Il est toujours **perçu depuis un point de vue** : celui de l’application.

> Le contexte est **relatif à un référentiel**, tout comme la réalité l’est à l’observateur.

C’est pourquoi **le contexte interne est nécessaire** :  
Il constitue **ce référentiel stable**, dans lequel les intentions peuvent être comprises, et les logiques activées.

* * *

### **Indépendants à la conception, indissociables à l’exécution**

Le **domaine** et le **contexte** peuvent — et doivent — être **conçus indépendamment**.  
Ils relèvent de disciplines différentes, de cycles de vie différents, de responsabilités différentes.

Mais ils ne peuvent **exister en acte** qu’à travers leur **rencontre.**  
C’est cette **rencontre, orchestrée dans un instant donné**, qui **fait naître l’application.**

> L’application n’est pas un objet figé.  
> C’est **un événement**, un **point d’interaction**, un **moment de convergence**.

À ce titre, domaine et contexte forment un **continuum**, à la manière de l’espace et du temps.  
Indépendants dans la théorie, **mais indissociables dans la réalité.**  
Leur interaction produit quelque chose de nouveau :

> une dynamique, une intention réalisée, une réalité numérique vivante.

C’est **dans ce point de jonction**, cette **orchestration consciente de leur interaction**, que réside **le vrai rôle de l’architecture**.

> Concevoir une application, c’est concevoir un **événement dans le continuum**.  
> Et l’architecture en est **le champ gravitationnel**.

* * *

### Les quatre dimensions fondamentales du **continuum**

Au final, la Continuum Architecture repose sur **quatre dimensions fondamentales** :

- Trois **contextuelles** : `setup`, `integration`, `initialization` — qui modélisent la structure du contexte interne et orchestrent la rencontre avec l’extérieur ;
- Une **fonctionnelle** : qui héberge le domaine, ses services, et son interface d’exploitation.

Le domaine est donc **une dimension à part entière**, mais nous choisissons de **ne pas en faire un sujet central**, car **les architectures existantes** (DDD, Clean Architecture, Hexagonal, etc.) **l’ont déjà largement exploré.** Notre attention se porte plutôt sur **l’orchestration** du domaine **dans le contexte** — car c’est là que réside le véritable angle mort de l’architecture logicielle contemporaine.

### **Note mathématique**

En termes mathématiques, on peut voir une application comme un **produit cartésien** :

> `Application = Domaine × Contexte`

Ce produit ne représente pas simplement un ensemble de composants, mais un **couple (contexte, domaine)** dont l’interaction produit un résultat.

En ce sens, lorsque certains affirment *« cette application est un produit »*, ils sont plus précis qu’ils ne le pensent :  
C’en est véritablement un — un produit dynamique entre un savoir structuré (le domaine) et une situation réelle (le contexte), donnant lieu à une résolution.

## 6\. **Principes fondateurs de la Continuum Architecture**

La Continuum Architecture repose sur un constat simple :

> Une application est l’acte d’appliquer un domaine à un contexte pour résoudre un problème.

De cette vision découle une nouvelle manière de penser l’architecture logicielle, fondée sur l’**orchestration consciente** du domaine et du contexte.

Voici ses **principes fondateurs** :

* * *

1. **Le domaine et le contexte sont modélisés séparément, mais conçus pour se rencontrer.**
2. Le domaine est autonome, le contexte est ouvert, et leur point de contact est orchestré. L’un n’est pas subordonné à l’autre.
3. **L’application naît d’un événement : la rencontre du domaine et du contexte.**
4. Ce n’est pas un objet mais un phénomène. Elle existe lorsqu’une intention s’exprime dans un contexte et active une logique métier.
5. **L’intention est le point de départ de toute exécution.**
6. C’est la forme exprimée du besoin, transmise par le contexte externe, captée et normalisée par un adaptateur.
7. **Le domaine est une dimension fonctionnelle, mais pas l’unique priorité.**
8. La Continuum Architecture reconnaît la richesse des architectures orientées domaine, mais recentre l’attention sur **l’orchestration dynamique du domaine dans un contexte donné.**
9. Ce n’est pas le domaine qui fait l’application, mais **la manière dont il est appliqué.**
10. **Le domaine reste incertain du contexte, mais non ignorant.**
11. C’est cette incertitude maîtrisée qui lui permet d’évoluer librement, tout en étant prêt à s’exécuter lorsqu’une intention traverse le contexte.
12. **Le contexte externe est subi, le contexte interne est structuré.**
13. Le premier est chaotique, multiforme, imprévisible. Le second est stable, cohérent, piloté par l’architecture.
14. **L’adaptateur est la conscience de l’application.**
15. Il transforme les causes brutes en intentions compréhensibles. Il relie deux mondes sans les confondre.
16. **Le contexte interne est structuré selon trois dimensions : setup, intégration, initialisation.**
17. Chacune joue un rôle spécifique dans la mise en scène de l’application et permet sa dynamisation.
18. **La causalité entre contexte et domaine est médiée, jamais directe.**
19. Le domaine ne reçoit jamais une requête brute : il répond à une intention orchestrée.
20. **L’application est relative à un référentiel.**
21. Le contexte est perçu depuis un point de vue. Le logiciel est un observateur : il organise le réel à partir de son propre cadre d’interprétation.
22. **Concevoir une architecture, c’est orchestrer une interaction.**
23. Pas accumuler des blocs. Pas choisir des couches. Mais organiser l’espace d’une rencontre, dans toutes ses dimensions : techniques, humaines, économiques, temporelles.
24. Enfin c’est à l’architecture, non au domaine, de gérer la tension entre la réalité brute et la logique métier. Cela inclut la création du contexte interne, la normalisation des entrées, et la cohérence des interactions.
25. **Le temps est une dimension de l’architecture.**
26. Le contexte change. Les intentions évoluent.
27. Une architecture doit être pensée non seulement dans l’espace (composants, couches), mais aussi dans le temps : durée de vie, synchronisation, instanciation dynamique.

## 7\. **Appel à l’action — Une nouvelle culture du logiciel**

La Continuum Architecture n’est pas une méthode.  
Ce n’est pas un cadre rigide, ni un outil prêt à l’emploi.  
C’est un **changement de regard**, un **changement de posture**, un **changement de culture.**

Elle nous invite à concevoir le logiciel non comme un empilement de couches, mais comme un **espace d’interaction** entre un domaine et un contexte.  
Non comme une solution fermée, mais comme une **rencontre orchestrée**.  
Non comme un code isolé, mais comme un **acte vivant, situé, intentionnel.**

Nous appelons donc :

- Les **développeurs** à modéliser le contexte avec autant de soin que le domaine.
- Les **architectes** à organiser le logiciel autour des intentions et des points de convergence.
- Les **formateurs** à enseigner la séparation entre contexte externe et interne.
- Les **concepteurs de frameworks** à rendre explicites les dimensions du contexte.
- Les **équipes** à questionner leurs modèles, leurs outils, leurs habitudes.
- Et l’**industrie entière** à redonner au contexte la place qu’il mérite : au cœur.

Si vous créez une CLI, un backend, une application mobile, un microservice ou un framework open source…  
Si vous déployez des modèles IA, des architectures serverless, des systèmes événementiels ou des infrastructures cloud natives…  
Alors **vous êtes concerné par la question du contexte**.  
Et **vous avez le pouvoir de transformer votre manière d’architecturer le logiciel**.

* * *

> Ce manifeste est la **théorie.**  
> **Stone.js** est sa **concrétisation tangible.**  
> Il s’agit d’un framework open source, conçu dès le départ pour incarner chaque principe du continuum :

- Adaptateurs conscients du contexte
- Pipelines d’exécution intentionnelle
- Séparation stricte entre domaine, contexte externe et contexte interne
- Dynamisation via blueprint, injection, orchestration

Des applications concrètes ont déjà été développées avec Stone.js, notamment :

- Des **CLI dynamiques** capables de s’adapter à différents environnements d’exécution
- Des **backends universels** déployables en Node, AWS Lambda ou edge functions sans modifier le code métier
- Des **applications frontales** utilisant le même domaine dans des contextes web, mobile ou serverless
- Des **démos pédagogiques** illustrant la puissance du découplage intentionnel et de la modélisation contextuelle

**Explorez, testez, contribuez** :

> [https://stonejs.com](https://stonejs.com)

Il ne s’agit pas d’ajouter une couche de complexité.  
Il s’agit de **voir avec plus de lucidité ce qui a toujours été là** :

> Le logiciel est un art de l’intention exécutée dans un contexte.

## 8\. **Signature et licence**

Ce manifeste a été rédigé par **Mr Stone**,  
créateur de **Stone.js**,  
conçu à partir d’années de réflexion, de conception, et de pratique autour de l’architecture logicielle contextuelle.

Il a été finalisé le **9 avril 2025**,  
et publié sous la licence **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

Cela signifie que :

- Vous êtes libres de le partager, le reproduire, le traduire, l’adapter.
- Même à des fins commerciales.
- À condition de **créditer l’auteur original** et de **lier vers la licence**.

> Licence complète : [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)

* * *

**Pour toute question, retour, ou contribution :**  
Vous pouvez explorer, discuter et expérimenter autour de la Continuum Architecture sur :
