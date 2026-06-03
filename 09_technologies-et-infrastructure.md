# 09 — Technologies et infrastructure

**Projet :** Orphée: Walk Straight
**Statut :** Document de travail
**Chemin :** `orphee-walk-straight/09_technologies-et-infrastructure.md`

---

## 1. Fonction du document

Ce document définit l’infrastructure technologique du projet **Orphée: Walk Straight**.

Il précise :

* les outils principaux;
* leur rôle dans l’architecture;
* les principes techniques;
* les modes de déploiement;
* les exigences multilingues;
* les exigences low-tech et offline-capable;
* les garde-fous en matière d’IA, de sécurité et de gouvernance;
* les besoins particuliers pour les milieux isolés et contraints.

Ce document ne décrit pas encore l’ensemble des contenus pédagogiques.
Il ne remplace pas le modèle pédagogique.
Il sert à stabiliser la couche technique qui rend le projet transférable.

---

## 2. Résumé stratégique

**Orphée: Walk Straight** repose sur une infrastructure de formation numérique appliquée, multilingue, sobre et distribuée.

Le projet vise à permettre à des apprenants de :

* apprendre à distance;
* produire des contenus utiles;
* structurer des savoirs;
* créer des plans, livres, guides, présentations, modules et ressources multimédias;
* utiliser l’IA de manière encadrée;
* documenter leurs productions;
* contribuer à une mémoire collective;
* transférer leurs compétences vers d’autres contextes.

L’infrastructure doit fonctionner dans des environnements variés :

* cégep;
* formation continue;
* communauté locale;
* villages éloignés;
* milieux à faible connectivité;
* milieux fermés ou contraints;
* contexte carcéral éventuel.

Le projet ne doit donc pas dépendre uniquement d’un accès cloud stable, d’outils coûteux ou de plateformes centralisées.

---

## 3. Principe directeur

L’infrastructure doit suivre cette règle :

> **Le système doit rester utile même lorsque la connexion, les ressources, les compétences techniques ou l’accès institutionnel sont limités.**

Autrement dit :

* cloud si disponible;
* local si nécessaire;
* offline si requis;
* exportable toujours;
* compréhensible par des non-spécialistes;
* gouvernable par les milieux qui l’utilisent.

Cette logique rejoint l’orientation kOA : une infrastructure n’est pas seulement une plateforme, mais un écosystème technosocial qui relie connaissance, choix, action et mémoire. 

---

## 4. Architecture générale

L’architecture du projet est organisée en six couches.

```text
1. Accès
2. Formation
3. Production
4. Structuration
5. Gouvernance
6. Mémoire et transfert
```

### 4.1 Accès

La couche d’accès permet aux participants d’entrer dans le système.

Elle peut prendre plusieurs formes :

* site web public;
* portail de formation;
* Moodle;
* dossier local;
* clé USB;
* paquet HTML/PDF;
* serveur local;
* kiosque contrôlé;
* poste informatique supervisé.

L’accès ne doit pas être confondu avec le projet lui-même.
Un kiosque, un site ou une plateforme n’est qu’un point d’entrée.

---

### 4.2 Formation

La couche formation permet de livrer les parcours pédagogiques.

Elle comprend :

* modules;
* consignes;
* exercices;
* exemples;
* évaluations;
* portfolios;
* badges ou preuves de compétence;
* rétroactions;
* ressources multimédias.

La formation doit être pratique, appliquée et orientée vers la production.

---

### 4.3 Production

La couche production permet aux participants de créer des livrables concrets :

* plans de livres;
* architectures de cours;
* guides;
* procédures;
* fiches pédagogiques;
* présentations;
* capsules;
* glossaires;
* banques d’exemples;
* quiz;
* documents multimédias;
* contenus traduits ou adaptés;
* ressources destinées à d’autres apprenants.

Le participant n’est pas seulement consommateur de formation.
Il devient progressivement producteur de ressources utiles.

---

### 4.4 Structuration

La couche structuration sert à transformer des contenus bruts en objets réutilisables.

Elle comprend :

* classification;
* indexation;
* métadonnées;
* découpage en modules;
* glossaires;
* relations entre concepts;
* versions;
* provenance;
* niveaux de confiance;
* liens entre ressources.

Cette couche est importante pour le multilingue, l’offline et la réutilisation.

SenTient peut jouer un rôle dans cette couche, car il est conçu comme un moteur de réconciliation d’entités et d’extraction de relations permettant de passer de textes non structurés vers des graphes de connaissance structurés. 

---

### 4.5 Gouvernance

La couche gouvernance sert à décider collectivement :

* quels contenus prioriser;
* quels modules améliorer;
* quels besoins traiter;
* quelles ressources valider;
* quelles règles appliquer;
* quelles erreurs corriger;
* quels terrains de transfert explorer.

Konnaxion / Ethikos intervient ici comme outil de consultation, de priorisation, de délibération, d’amélioration continue et de mémoire décisionnelle.

Dans l’architecture UCKK-Moodle, Konnaxion doit rester un système externe optionnel, intégré par contrat, et non une dépendance obligatoire du campus pédagogique. 

---

### 4.6 Mémoire et transfert

La couche mémoire conserve :

* les productions;
* les versions;
* les décisions;
* les corrections;
* les rétroactions;
* les preuves de compétence;
* les apprentissages;
* les procédures validées;
* les résultats de pilote.

La mémoire permet le transfert vers d’autres contextes.

Sans mémoire, chaque cohorte recommence à zéro.
Avec mémoire, chaque cohorte améliore le système.

---

## 5. Composantes principales

### 5.1 UCKK.org

**Rôle :** vitrine pédagogique et point d’entrée public.

UCKK.org sert à présenter :

* la vision éducative;
* les parcours;
* les ressources;
* les projets;
* les productions;
* les principes de formation;
* les liens vers les outils.

UCKK.org ne doit pas être présenté comme une université accréditée.
Il doit être présenté comme une vitrine expérimentale de formation appliquée.

---

### 5.2 UCKK-Moodle

**Rôle :** campus pédagogique structuré.

UCKK-Moodle sert à gérer :

* cours;
* cohortes;
* rôles;
* permissions;
* activités;
* compétences;
* preuves;
* badges;
* rapports;
* archives;
* parcours.

La documentation UCKK-Moodle le définit comme l’implémentation campus de UCKK dans Moodle, avec une distribution pédagogique complète, des plugins coordonnés, des rôles, des capacités et des mécanismes de gouvernance. 

UCKK-Moodle est la composante la plus compatible avec un projet collégial, car Moodle est déjà un environnement connu dans le monde de la formation.

---

### 5.3 Konnaxion / Ethikos

**Rôle :** gouvernance collective.

Konnaxion / Ethikos sert à :

* consulter;
* prioriser;
* structurer les décisions;
* documenter les désaccords;
* suivre les améliorations;
* garder une mémoire de gouvernance;
* relier les contributions aux décisions.

Dans Orphée: Walk Straight, Konnaxion ne doit pas être vendu comme plateforme totale.

Formulation correcte :

> **Konnaxion / Ethikos est un outil de gouvernance pédagogique et d’amélioration collective.**

Il ne remplace pas Moodle.
Il ne remplace pas les enseignants.
Il ne remplace pas le cégep.
Il ne décide pas à la place des humains.

---

### 5.4 initkOA.org / links

**Rôle :** bibliothèque de références et corpus de départ.

`initkoa.org/links` sert à organiser :

* ressources;
* textes;
* références;
* outils;
* exemples;
* corpus pédagogique;
* liens vers les composantes publiques;
* matériaux de formation.

Cette bibliothèque doit être progressivement structurée pour devenir :

* navigable;
* annotée;
* classée par parcours;
* utilisable offline;
* traduisible;
* intégrable à Moodle ou à des paquets de formation.

---

### 5.5 SemantiK Architect

**Rôle :** production multilingue structurée.

SemantiK Architect peut soutenir :

* génération de textes structurés;
* rendu multilingue;
* adaptation de ressources;
* grammaires contrôlées;
* production cohérente de contenus;
* soutien aux langues moins bien servies;
* séparation entre intention structurée et surface linguistique.

La documentation technique de SemantiK Architect décrit une architecture dépendant notamment de Grammatical Framework, de Python, d’un environnement Linux/WSL et d’une organisation modulaire autour de backend, frontend, données, schémas et outils. 

Dans Orphée: Walk Straight, SemantiK Architect doit être présenté comme une brique de production multilingue, non comme une exigence immédiate pour tous les pilotes.

---

### 5.6 SenTient

**Rôle :** structuration du savoir.

SenTient peut soutenir :

* extraction d’entités;
* réconciliation;
* extraction de relations;
* structuration de documents;
* lien vers graphes de connaissance;
* désambiguïsation;
* indexation de corpus.

Il peut devenir utile lorsque le projet accumule beaucoup de contenus, de guides, de livres, de modules et de ressources multilingues.

Au début, SenTient doit rester une composante avancée.
Il ne doit pas bloquer le pilote initial.

---

### 5.7 Outils IA généralistes

**Rôle :** assistance à la production.

Les outils IA peuvent servir à :

* résumer;
* reformuler;
* proposer des plans;
* corriger;
* structurer;
* générer des exemples;
* créer des quiz;
* transformer un document en module;
* aider à la traduction;
* proposer des scripts de capsules;
* vérifier la cohérence d’un contenu.

L’IA doit être encadrée par des procédures.

Règle :

> **L’IA assiste la production, mais ne valide pas l’autorité du contenu.**

Les productions doivent être relues, testées et validées humainement.

---

### 5.8 Gamma et outils de présentation

**Rôle :** production multimédia rapide.

Gamma et les outils similaires peuvent être utilisés pour :

* présentations;
* supports visuels;
* capsules;
* modules courts;
* documents de vulgarisation;
* ateliers;
* résumés pédagogiques.

Ils sont utiles pour former rapidement des apprenants à produire du matériel diffusable.

Toutefois, les contenus produits doivent être exportables dans des formats plus durables :

* PDF;
* HTML;
* Markdown;
* images;
* texte brut;
* documents imprimables.

---

### 5.9 Formats sobres

**Rôle :** durabilité, accessibilité, offline.

Les formats prioritaires sont :

* Markdown;
* HTML statique;
* PDF;
* EPUB;
* CSV;
* JSON;
* images compressées;
* audio léger;
* vidéo compressée;
* paquets ZIP;
* dossiers synchronisables.

Le projet doit éviter de dépendre uniquement de formats propriétaires ou de plateformes non exportables.

---

## 6. Modes de déploiement

L’infrastructure doit pouvoir être déployée selon plusieurs modes.

### 6.1 Mode public web

Utilisé pour :

* vitrine;
* démonstration;
* accès général;
* partage de ressources;
* communication publique;
* documentation.

Exemples :

* UCKK.org;
* initkOA.org;
* pages publiques;
* documentation ouverte.

---

### 6.2 Mode cohorte locale

Utilisé pour le premier pilote.

Caractéristiques :

* petit groupe;
* accès accompagné;
* ateliers;
* production concrète;
* outils en ligne disponibles;
* suivi humain;
* collecte de rétroactions;
* documentation des procédures.

Ce mode est le plus approprié pour la première expérimentation avec :

* étudiants;
* personnel intéressé;
* acteurs communautaires;
* experts invités;
* partenaires locaux.

---

### 6.3 Mode hybride

Utilisé lorsque certains participants sont sur place et d’autres à distance.

Caractéristiques :

* rencontres synchrones;
* activités asynchrones;
* documents partagés;
* livrables communs;
* suivi par Moodle ou équivalent;
* gouvernance par Konnaxion/Ethikos;
* production collaborative.

---

### 6.4 Mode basse connectivité

Utilisé pour les villages isolés ou les régions mal desservies.

Caractéristiques :

* contenus téléchargeables;
* paquets offline;
* faible bande passante;
* synchronisation différée;
* formats compressés;
* priorité au texte, audio léger et PDF;
* vidéo optionnelle;
* accès mobile possible.

---

### 6.5 Mode offline-capable

Utilisé lorsque la connexion est absente, instable ou volontairement limitée.

Caractéristiques :

* serveur local possible;
* Moodle local ou paquet statique;
* bibliothèque locale;
* exercices hors ligne;
* exports de productions;
* synchronisation manuelle;
* sauvegardes physiques;
* clés USB ou disques chiffrés;
* journaux d’activité exportables.

---

### 6.6 Mode milieu contraint

Utilisé pour les établissements fermés ou sensibles.

Caractéristiques :

* accès contrôlé;
* aucun accès libre au web;
* liste blanche de ressources;
* IA filtrée ou locale si disponible;
* validation humaine;
* supervision;
* journalisation;
* données non sensibles;
* absence de contact direct non supervisé avec l’extérieur;
* production volontaire et formative.

Ce mode peut être pertinent pour une transposition carcérale future, mais il ne doit pas être le premier pilote.

---

## 7. Principe offline-capable

Le projet n’a pas besoin d’être entièrement offline dès le départ.

Il doit cependant être conçu pour devenir offline-capable.

Cela signifie :

* les contenus doivent être exportables;
* les parcours doivent être lisibles sans plateforme complexe;
* les ressources doivent pouvoir être empaquetées;
* les dépendances cloud doivent être identifiées;
* les versions doivent être contrôlées;
* les productions doivent pouvoir être sauvegardées localement;
* les procédures doivent être exécutables avec peu d’outils.

Niveau minimal :

```text
Markdown + PDF + dossiers structurés + procédures + exports
```

Niveau intermédiaire :

```text
Moodle + paquets téléchargeables + bibliothèques locales + synchronisation différée
```

Niveau avancé :

```text
serveur local + IA locale/contrôlée + graphes de connaissance + gouvernance synchronisable
```

---

## 8. Principe multilingue

Le multilingue n’est pas un ajout esthétique.
Il est central.

Le projet vise des publics qui peuvent être :

* francophones;
* anglophones;
* allophones;
* autochtones;
* en francisation;
* peu alphabétisés;
* éloignés des institutions;
* situés dans d’autres pays ou régions.

L’infrastructure doit donc soutenir :

* glossaires;
* versions simplifiées;
* traductions assistées;
* adaptation culturelle;
* terminologie contrôlée;
* versions faciles à lire;
* versions imprimables;
* audio;
* contenus bilingues ou multilingues;
* production progressive par langue.

SemantiK Architect peut devenir une brique importante pour produire des rendus linguistiques cohérents, surtout lorsque le projet voudra dépasser la traduction libre et stabiliser des contenus dans plusieurs langues. 

---

## 9. Principe low-tech / technologies sobres

Le projet utilise l’expression institutionnelle :

> **technologies éducatives sobres**

plutôt que seulement :

> low-tech.

Une technologie sobre est :

* compréhensible;
* réparable;
* exportable;
* documentée;
* peu coûteuse;
* compatible avec des machines modestes;
* utilisable avec peu de bande passante;
* indépendante d’un fournisseur unique;
* adaptée aux capacités réelles des milieux.

Ce principe est essentiel pour :

* Basse-Côte-Nord;
* villages isolés;
* organismes sous-financés;
* milieux carcéraux;
* formation continue;
* projets internationaux;
* publics sans matériel récent.

---

## 10. IA encadrée

L’IA est un outil de production, pas une autorité.

### 10.1 Usages permis

L’IA peut aider à :

* générer des idées;
* structurer des plans;
* reformuler;
* vulgariser;
* produire des exemples;
* créer des quiz;
* transformer un contenu en activité;
* faire des brouillons;
* assister la traduction;
* créer des scripts;
* proposer des titres;
* analyser la cohérence d’un document.

### 10.2 Usages interdits ou à éviter

L’IA ne doit pas :

* valider seule une vérité;
* remplacer une évaluation humaine;
* produire des contenus non vérifiés;
* créer des données inventées;
* être utilisée pour contourner des règles;
* traiter des données sensibles sans cadre;
* permettre du contact non supervisé en milieu contraint;
* servir à des usages offensifs, frauduleux ou manipulatoires.

### 10.3 Règle de validation

Toute production assistée par IA doit passer par :

```text
production → révision humaine → test → correction → archivage
```

---

## 11. Sécurité et confidentialité

La sécurité doit être proportionnée au contexte.

### 11.1 Premier pilote local

Exigences minimales :

* comptes séparés;
* consentement des participants;
* pas de données sensibles inutiles;
* sauvegardes;
* distinction entre contenu public et contenu interne;
* droit de retrait des productions personnelles;
* clarté sur l’usage des outils IA.

### 11.2 Milieux isolés

Exigences supplémentaires :

* fonctionnement basse connectivité;
* sauvegardes locales;
* procédures imprimables;
* formation de relais locaux;
* gestion des versions;
* duplication des ressources essentielles.

### 11.3 Milieux contraints

Exigences renforcées :

* accès supervisé;
* aucune navigation libre;
* ressources préapprouvées;
* données fictives ou non sensibles;
* traçabilité;
* validation humaine;
* absence de messagerie libre;
* aucun contact non supervisé avec clients externes;
* aucun usage offensif de l’IA;
* participation volontaire.

---

## 12. Données et contenus

Le projet doit distinguer plusieurs types de données.

| Type                        | Exemple                                   | Sensibilité |
| --------------------------- | ----------------------------------------- | ----------- |
| Contenu public              | guides, modules, fiches                   | faible      |
| Contenu pédagogique interne | consignes, grilles, exercices             | moyenne     |
| Données d’apprenants        | progression, portfolios, rétroactions     | élevée      |
| Données de gouvernance      | décisions, votes, commentaires            | variable    |
| Données sensibles           | renseignements personnels, justice, santé | élevée      |
| Données de test             | exemples fictifs                          | faible      |

Règle :

> **Ne jamais utiliser de données sensibles lorsqu’une donnée fictive ou anonymisée suffit.**

---

## 13. Interopérabilité

L’infrastructure doit éviter l’enfermement dans un seul outil.

Les contenus doivent pouvoir circuler entre :

* Markdown;
* Moodle;
* PDF;
* HTML;
* Gamma;
* documents texte;
* tableurs;
* bibliothèques locales;
* archives;
* systèmes de gouvernance.

Principe :

> **Chaque production importante doit pouvoir être exportée dans au moins un format ouvert ou durable.**

---

## 14. Rôles techniques

### 14.1 Architecte du projet

Responsable de :

* cohérence générale;
* choix des outils;
* priorités techniques;
* documentation;
* alignement avec la vision.

### 14.2 Responsable pédagogique

Responsable de :

* objectifs d’apprentissage;
* progression;
* exercices;
* évaluations;
* compétences;
* qualité des contenus.

### 14.3 Responsable infrastructure

Responsable de :

* comptes;
* hébergement;
* sauvegardes;
* sécurité;
* accès;
* synchronisation;
* déploiements.

### 14.4 Responsable gouvernance

Responsable de :

* décisions;
* consultations;
* priorisation;
* procédures collectives;
* usage de Konnaxion/Ethikos.

### 14.5 Participants producteurs

Responsables de :

* suivre les procédures;
* produire des livrables;
* documenter leur démarche;
* corriger selon les rétroactions;
* construire leur portfolio.

### 14.6 Experts invités

Responsables de :

* offrir une rétroaction ciblée;
* valider certains contenus;
* proposer des améliorations;
* relier le projet à des besoins réels.

---

## 15. Infrastructure du premier pilote

Le premier pilote doit rester simple.

### 15.1 Configuration recommandée

```text
- UCKK.org comme vitrine
- initkOA.org/links comme bibliothèque de départ
- Konnaxion/Ethikos comme outil de gouvernance et priorisation
- Dossier partagé structuré pour les productions
- Outils IA généralistes pour assistance encadrée
- Gamma pour productions visuelles
- Markdown / PDF pour archivage sobre
- Tableur pour suivi minimal
- Portfolio individuel par participant
```

### 15.2 À éviter au premier pilote

Éviter de rendre obligatoire :

* serveur local complexe;
* IA locale complète;
* intégration complète Moodle;
* graphes de connaissance complets;
* automatisation avancée;
* système de badges entièrement automatisé;
* déploiement carcéral;
* déploiement multilingue complet.

Le pilote doit prouver la méthode avant de complexifier l’infrastructure.

---

## 16. Livrables techniques du premier pilote

Le premier pilote devrait produire :

1. un gabarit de module pédagogique;
2. un gabarit de plan de livre;
3. un gabarit de présentation Gamma;
4. un gabarit de fiche d’exercice;
5. un gabarit de procédure;
6. une structure de dossier standard;
7. une grille de qualité;
8. un modèle de portfolio;
9. un protocole d’usage de l’IA;
10. un protocole de gouvernance Konnaxion/Ethikos;
11. un paquet exportable de ressources;
12. un rapport d’expérimentation.

---

## 17. Déploiement vers la Basse-Côte-Nord

Pour les villages isolés de la Basse-Côte-Nord, l’infrastructure devra prioriser :

* contenus téléchargeables;
* accès mobile;
* documents imprimables;
* faibles besoins de bande passante;
* accompagnement local;
* relais communautaires;
* multilingue;
* synchronisation différée;
* autonomie des milieux;
* production locale de contenus.

Objectif :

> **Tester si une formation avancée peut rester utile même lorsque l’accès aux institutions et aux réseaux est limité.**

---

## 18. Déploiement futur en milieu carcéral

Pour le milieu carcéral, l’infrastructure devra prioriser :

* sécurité;
* volontariat;
* accès contrôlé;
* absence de navigation libre;
* ressources préapprouvées;
* formation pratique;
* production encadrée;
* données fictives;
* portfolios exportables;
* reconnaissance selon les règles des programmes en place;
* absence de travail forcé;
* continuité possible après la sortie, si applicable.

Le milieu carcéral n’est pas le premier pilote.
Il est un terrain spécialisé de transfert.

---

## 19. Non-objectifs

Le projet ne vise pas à :

* remplacer le cégep;
* créer immédiatement une université accréditée;
* remplacer Moodle;
* faire de Konnaxion une plateforme obligatoire;
* automatiser l’enseignement;
* remplacer les enseignants ou mentors;
* utiliser les participants comme main-d’œuvre gratuite;
* déployer l’IA sans encadrement;
* dépendre d’un fournisseur unique;
* tout construire avant de tester.

---

## 20. Critères de réussite technologique

L’infrastructure sera considérée comme efficace si elle permet :

* à une cohorte hybride de produire des contenus réutilisables;
* à des non-spécialistes de suivre les procédures;
* à des contenus d’être exportés en formats durables;
* à des ressources d’être adaptées en contexte de faible connectivité;
* à des décisions pédagogiques d’être documentées;
* à des productions d’être évaluées et améliorées;
* à des portfolios d’être constitués;
* à un transfert vers un autre milieu d’être envisageable;
* à la complexité technique de rester maîtrisée.

---

## 21. Synthèse

L’infrastructure d’Orphée: Walk Straight doit être :

```text
modulaire
sobre
multilingue
offline-capable
gouvernable
exportable
sécurisable
pédagogiquement utile
```

La formule centrale :

> **UCKK forme. Konnaxion gouverne. initkOA documente. SemantiK rend multilingue. SenTient structure. Les humains valident. Les archives transmettent.**

L’objectif n’est pas de construire une plateforme totale.

L’objectif est de construire une infrastructure de formation capable de fonctionner là où l’accès au savoir est limité par la distance, les murs, la langue, la connectivité ou les ressources.
