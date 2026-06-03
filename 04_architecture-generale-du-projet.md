# 04 — Architecture générale du projet

**Projet :** Orphée: Walk Straight
**Chemin :** `orphee-walk-straight/04_architecture-generale-du-projet.md`
**Statut :** Document de cadrage architectural
**Version :** 0.1
**Usage :** Dossier pré-CCTT / note d’intention / alignement interne
**Portée :** Architecture conceptuelle, pédagogique, technique et de gouvernance du projet

---

## 1. Fonction du document

Ce document présente l’architecture générale du projet **Orphée: Walk Straight**.

Il ne décrit pas encore les contenus de cours, les procédures détaillées, les budgets, ni les ententes administratives. Ces éléments sont traités dans d’autres fichiers du dossier.

Sa fonction est de clarifier :

* les composantes du projet;
* leur rôle respectif;
* leurs limites;
* leurs relations;
* les flux entre formation, production, gouvernance, transfert et mémoire;
* la manière dont le projet peut évoluer vers une logique de laboratoire collégial ou de CCTT.

Le projet doit rester lisible pour trois publics :

1. **public institutionnel** : cégep, ministères, partenaires régionaux;
2. **public opérationnel** : formateurs, étudiants, personnel, experts, organismes;
3. **public technique** : développeurs, architectes, responsables de plateformes, contributeurs.

---

## 2. Définition courte du projet

**Orphée: Walk Straight** est un projet de formation numérique inclusive, multilingue et distribuée.

Il vise à développer, tester et transférer des méthodes de formation à distance permettant à des apprenants de produire des contenus, outils, plans, livres, modules pédagogiques, présentations, documents multimédias et ressources numériques utiles.

Le projet est conçu pour fonctionner dans des contextes où l’accès à la formation est limité par :

* la distance;
* la faible connectivité;
* l’isolement territorial;
* les murs institutionnels;
* les contraintes matérielles;
* les barrières linguistiques;
* les parcours scolaires ou sociaux non linéaires.

Le premier pilote doit se faire avec une **cohorte hybride locale** autour de Baie-Comeau : étudiants, personnel intéressé, acteurs communautaires, experts invités et partenaires régionaux.

Les premiers terrains spécialisés de transfert visés sont :

1. les milieux isolés, notamment les villages de la Basse-Côte-Nord;
2. les milieux contraints, dont le milieu carcéral.

---

## 3. Principe architectural central

Le projet ne repose pas sur une seule plateforme.

Il repose sur une architecture distribuée composée de plusieurs couches :

```text
Vision et cadre culturel
        ↓
Campus de formation
        ↓
Production pédagogique
        ↓
Gouvernance collective
        ↓
Structuration du savoir
        ↓
Rendu multilingue
        ↓
Portabilité offline
        ↓
Transfert vers milieux isolés ou contraints
        ↓
Mémoire et amélioration continue
```

La logique générale est alignée avec le cycle kOA :

```text
Connaître → Choisir → Agir → Se souvenir → Mieux connaître
```

Dans la documentation kOA, le kOA Digital Ecosystem est défini comme une infrastructure sociotechnique qui transforme les contributions en connaissance, la connaissance en orientation collective, l’orientation en action coordonnée et l’expérience en mémoire active. 

---

## 4. Architecture en une phrase

**Orphée: Walk Straight utilise un campus de formation, une couche de gouvernance collective, des outils de structuration du savoir, des outils de production multilingue et des formats offline pour rendre la formation avancée accessible aux publics éloignés, empêchés ou contraints.**

Formule opérationnelle :

```text
Apprendre → Produire → Valider → Traduire → Distribuer → Transférer → Améliorer
```

Formule pédagogique :

```text
Former par la production.
Reconnaître par les preuves.
Transférer par les usages.
Gouverner par la délibération.
Mémoriser par les archives.
```

---

## 5. Couches principales

### 5.1 Couche 1 — Cadre conceptuel

**Rôle :** donner l’orientation générale du projet.

Cette couche comprend :

* kOA comme cadre de pensée;
* Orphée comme nom de projet;
* Walk Straight comme principe d’avancement;
* l’inclusion numérique comme valeur;
* la formation à distance comme moyen;
* la production de savoirs comme méthode;
* le CCTT comme trajectoire institutionnelle possible.

Dans le canon UCKK, la hiérarchie distingue clairement kOA comme mouvement, UCKK comme école ou cité d’apprentissage, le kOA Digital Ecosystem comme infrastructure numérique, King Klown comme figure narrative, les Assemblées comme légitimité collective et les Archives comme mémoire. 

Cette distinction doit être préservée dans Orphée: Walk Straight.

Le projet ne doit donc pas confondre :

```text
kOA ≠ UCKK
UCKK ≠ Konnaxion
Konnaxion ≠ Moodle
Orphée ≠ tout kOA
Projet CCTT ≠ université accréditée
```

---

### 5.2 Couche 2 — Campus de formation

**Composante principale :** UCKK / UCKK-Moodle
**Rôle :** héberger les parcours, modules, activités, ressources, évaluations, preuves et portfolios.

Le campus de formation sert à :

* organiser les parcours;
* publier les modules;
* attribuer des activités;
* recueillir les productions;
* suivre les compétences;
* documenter les preuves;
* soutenir les microcertifications;
* exporter des traces ou portfolios.

Dans la doctrine UCKK-Moodle, UCKK-Moodle est défini comme l’implémentation campus Moodle de UCKK. Il ne doit pas être présenté comme tout le mouvement kOA ni comme tout Konnaxion. 

Pour Orphée, cela signifie :

```text
UCKK-Moodle = campus pédagogique
Konnaxion = gouvernance collective optionnelle
kOA = cadre conceptuel
Orphée = projet appliqué pré-CCTT
```

---

### 5.3 Couche 3 — Production pédagogique

**Rôle :** transformer les apprenants en producteurs de contenus et d’outils.

Le projet ne repose pas sur la simple consommation de cours.

Les participants apprennent à produire :

* architectures de plans;
* plans de livres;
* modules de formation;
* présentations Gamma;
* scripts de narration;
* guides pratiques;
* fiches pédagogiques;
* quiz;
* glossaires;
* supports visuels;
* contenus multimédias;
* procédures;
* documents accessibles;
* paquets de formation offline.

Cette couche est centrale pour le projet.

Elle permet de dire :

> Les apprenants ne reçoivent pas seulement une formation; ils apprennent à produire des ressources qui peuvent former d’autres personnes.

---

### 5.4 Couche 4 — Gouvernance collective

**Composante principale :** Konnaxion / Ethikos
**Rôle :** soutenir la consultation, la priorisation, l’amélioration continue et la mémoire des décisions.

Konnaxion ne doit pas être le produit principal du projet.

Il doit être présenté comme une couche de gouvernance pédagogique et collective.

Il peut servir à :

* choisir les prochains modules à produire;
* prioriser les besoins des milieux;
* recueillir les rétroactions;
* documenter les désaccords;
* consulter les experts;
* faire émerger les besoins communautaires;
* structurer les décisions;
* garder une trace des arbitrages;
* améliorer les contenus au fil du temps.

La règle canonique UCKK-Moodle / Konnaxion est utile pour Orphée : Konnaxion peut produire des lectures ou signaux Smart Vote, mais les décisions d’Assemblée appartiennent au flux institutionnel humain, et les Archives conservent les décisions, sources, contestations et traces. 

Principe à respecter :

```text
Konnaxion informe.
Les humains décident.
Les archives prouvent.
Le campus applique.
```

---

### 5.5 Couche 5 — Structuration du savoir

**Composante principale :** SenTient
**Rôle :** aider à transformer des contenus bruts en connaissances structurées.

SenTient peut soutenir :

* l’extraction d’entités;
* la désambiguïsation;
* la relation entre concepts;
* le classement de ressources;
* la préparation de graphes de connaissances;
* la structuration de corpus pédagogiques;
* la vérification partielle de cohérence;
* la liaison entre contenus, sources et concepts.

SenTient est décrit comme un moteur de réconciliation d’entités et d’extraction de relations capable de relier du texte non structuré à des graphes de connaissances. Son architecture combine plusieurs couches : repérage rapide, analyse sémantique et structuration. 

Dans Orphée, SenTient n’est pas nécessaire au premier jour.

Il représente une capacité avancée pour :

* organiser de grands corpus;
* préparer des parcours multilingues;
* relier les ressources à des concepts;
* faciliter la production de formations structurées.

---

### 5.6 Couche 6 — Rendu multilingue

**Composante principale :** SemantiK Architect
**Rôle :** produire ou soutenir le rendu multilingue structuré de contenus.

SemantiK Architect peut servir à :

* générer des formulations multilingues;
* produire des phrases à partir de structures sémantiques;
* stabiliser des patrons de formulation;
* éviter la traduction improvisée;
* soutenir les langues moins bien desservies;
* produire des variantes linguistiques contrôlées;
* aider à construire des ressources pédagogiques multilingues.

SemantiK Architect est décrit comme un système NLG multilingue centré sur un planificateur, capable de produire du texte structuré et traçable à partir d’entrées sémantiques, avec une architecture qui sépare ce qui est dit de la manière dont cela est rendu dans une langue donnée. 

Dans Orphée, SemantiK Architect soutient la vision :

> rendre les savoirs accessibles au-delà des barrières linguistiques, sans dépendre uniquement de traductions opaques ou instables.

---

### 5.7 Couche 7 — Portabilité offline

**Composante possible :** Kristals / paquets de savoir / exports offline
**Rôle :** rendre les contenus utilisables en contexte de faible connectivité.

Le projet vise des milieux où l’accès stable au web ne peut pas être présumé.

La couche offline doit permettre :

* l’export PDF;
* l’export HTML léger;
* les paquets téléchargeables;
* les bibliothèques locales;
* les versions imprimables;
* les capsules vidéo compressées;
* les présentations autonomes;
* les modules consultables sans connexion;
* la conservation locale des preuves et ressources.

Dans la documentation kOA, les Kristals sont présentés comme des artefacts de connaissance portables, vérifiables et utilisables en contexte dégradé ou offline. 

Pour Orphée, le principe est :

```text
Un contenu utile doit pouvoir survivre à une mauvaise connexion.
```

---

### 5.8 Couche 8 — Transfert vers les milieux

**Rôle :** adapter la formation à différents contextes.

Les terrains de transfert ne sont pas tous identiques.

Le projet distingue :

```text
Pilote local
    → cohorte hybride à Baie-Comeau

Terrain isolé
    → Basse-Côte-Nord, villages éloignés, faible connectivité

Terrain contraint
    → milieu carcéral, accès contrôlé, sécurité renforcée
```

Chaque terrain exige une adaptation :

| Terrain                     | Adaptation principale                                                   |
| --------------------------- | ----------------------------------------------------------------------- |
| Cohorte hybride locale      | tester la méthode, produire les premiers contenus                       |
| Basse-Côte-Nord             | formats offline, multilingue, accompagnement à distance                 |
| Milieu carcéral             | sécurité, volontariat, accès contrôlé, absence de contact non supervisé |
| Organismes communautaires   | simplicité, transfert, documentation, autonomie                         |
| Formation continue          | compétences pratiques, reconnaissance, portfolio                        |
| International / multilingue | adaptation linguistique, contenus légers, distribution locale           |

---

## 6. Schéma général

```text
                              ┌────────────────────────────┐
                              │      Cadre kOA / Orphée     │
                              │  Vision, principes, limites │
                              └──────────────┬─────────────┘
                                             │
                                             ▼
┌──────────────────────────────────────────────────────────────────┐
│                         Campus pédagogique                        │
│                         UCKK / Moodle                             │
│      Parcours, modules, activités, preuves, portfolios, badges     │
└───────────────────────────────┬──────────────────────────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────────────────────────┐
│                    Production pédagogique appliquée                │
│  Plans, livres, modules, présentations, guides, quiz, multimédia   │
└───────────────────────────────┬──────────────────────────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────────────────────────┐
│                  Gouvernance collective / Ethikos                 │
│     Consultation, priorisation, décisions humaines, amélioration   │
└───────────────────────────────┬──────────────────────────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────────────────────────┐
│                   Structuration et rendu du savoir                 │
│        SenTient, SemantiK Architect, corpus, sources, concepts     │
└───────────────────────────────┬──────────────────────────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────────────────────────┐
│                     Distribution sobre et offline                 │
│       PDF, HTML léger, paquets locaux, Kristals, exports           │
└───────────────────────────────┬──────────────────────────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────────────────────────┐
│                         Terrains de transfert                     │
│       Basse-Côte-Nord, milieux isolés, milieux contraints          │
└───────────────────────────────┬──────────────────────────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────────────────────────┐
│                    Archives et amélioration continue               │
│       traces, preuves, versions, rétroactions, leçons apprises     │
└──────────────────────────────────────────────────────────────────┘
```

---

## 7. Flux opérationnel

### 7.1 Flux normal d’un module

```text
1. Besoin identifié
2. Sujet priorisé
3. Plan de module rédigé
4. Contenu produit
5. Contenu révisé
6. Activités créées
7. Évaluation définie
8. Module publié
9. Cohorte teste
10. Rétroactions collectées
11. Module corrigé
12. Version archivée
13. Version exportée
14. Module transféré vers un autre milieu
```

---

### 7.2 Flux de production par apprenant

```text
1. L’apprenant reçoit une consigne claire
2. Il consulte les ressources
3. Il produit un artefact
4. Il documente sa démarche
5. Il applique une grille qualité
6. Il reçoit une rétroaction
7. Il corrige
8. Il publie ou soumet
9. Sa production devient une preuve
10. La preuve entre dans son portfolio
```

---

### 7.3 Flux de gouvernance

```text
1. Un besoin ou problème est soumis
2. Les participants réagissent
3. Les experts commentent
4. Les options sont structurées
5. Une recommandation est formulée
6. Une décision humaine est prise
7. La décision est archivée
8. Le plan d’action est appliqué
9. Le résultat est évalué
10. La mémoire du projet est mise à jour
```

---

## 8. Règles de séparation

Pour éviter la confusion, les règles suivantes sont obligatoires.

### 8.1 kOA

kOA est le cadre large.

Il ne doit pas être présenté comme le CCTT lui-même.

### 8.2 Orphée: Walk Straight

Orphée est le projet appliqué.

Il sert à structurer un dossier de formation numérique inclusive et de transfert.

### 8.3 UCKK

UCKK est l’espace pédagogique expérimental.

Il peut héberger des parcours, mais ne doit pas être présenté comme université accréditée.

### 8.4 Moodle / UCKK-Moodle

Moodle est le campus de formation.

Il porte les cours, activités, preuves et parcours.

### 8.5 Konnaxion / Ethikos

Konnaxion sert à la gouvernance collective.

Il ne décide pas à la place des personnes ou institutions.

### 8.6 SemantiK Architect

SemantiK Architect sert au rendu multilingue structuré.

Il n’est pas un LMS, ni un système de gouvernance.

### 8.7 SenTient

SenTient sert à structurer et relier le savoir.

Il n’est pas le campus, ni l’outil de décision.

### 8.8 Kristals / paquets offline

Les paquets offline servent à transporter, vérifier et utiliser des savoirs hors ligne.

Ils ne remplacent pas l’évaluation humaine ou pédagogique.

---

## 9. Modes de fonctionnement

### 9.1 Mode local pilote

Utilisé pour la première cohorte hybride.

Caractéristiques :

* accès web normal;
* outils publics;
* expérimentation rapide;
* faible contrainte;
* documentation systématique;
* apprentissage par production.

Objectif :

> valider la méthode avant les transferts spécialisés.

---

### 9.2 Mode territorial isolé

Utilisé pour la Basse-Côte-Nord ou d’autres milieux éloignés.

Caractéristiques :

* faible connectivité possible;
* besoin de formats légers;
* accompagnement à distance;
* contenus multilingues;
* ressources imprimables;
* autonomie locale.

Objectif :

> prouver que le modèle fonctionne quand l’accès aux institutions et aux réseaux est limité.

---

### 9.3 Mode contraint sécurisé

Utilisé pour le milieu carcéral ou d’autres institutions fermées.

Caractéristiques :

* accès contrôlé;
* aucune navigation libre non autorisée;
* outils limités;
* validation humaine renforcée;
* participation volontaire;
* production encadrée;
* données non sensibles;
* aucune tâche à risque criminogène.

Objectif :

> adapter la formation numérique appliquée à un environnement sécurisé sans transformer les participants en main-d’œuvre contrainte.

---

## 10. Architecture CCTT visée

Le projet peut évoluer vers une structure de type CCTT si plusieurs conditions sont réunies :

* porteur collégial confirmé;
* besoin régional démontré;
* pilote documenté;
* partenaires preneurs identifiés;
* capacité de formation et transfert;
* spécialisation claire;
* complémentarité avec les CCTT existants;
* retombées mesurables;
* gouvernance institutionnelle acceptable.

L’hypothèse de spécialisation est :

> **formation numérique inclusive, multilingue, sobre et offline-capable, appliquée aux milieux éloignés, empêchés ou contraints.**

Le CCTT éventuel ne serait donc pas un CCTT carcéral.

Il serait un centre de transfert en :

* formation à distance appliquée;
* production pédagogique;
* technologies éducatives sobres;
* IA encadrée;
* multilinguisme;
* accessibilité;
* milieux isolés;
* milieux contraints.

---

## 11. Objets produits par l’architecture

Le projet doit produire des objets concrets.

### 11.1 Objets pédagogiques

* modules;
* cours;
* fiches;
* exercices;
* quiz;
* évaluations;
* parcours;
* glossaires;
* capsules;
* présentations;
* scripts;
* guides.

### 11.2 Objets de production

* procédures;
* modèles;
* gabarits;
* checklists;
* workflows;
* guides Gamma;
* guides d’architecture de livres;
* guides de production multimédia;
* modèles de portfolio.

### 11.3 Objets de gouvernance

* comptes rendus;
* décisions;
* votes consultatifs;
* priorités;
* rétroactions;
* rapports de test;
* demandes de correction;
* archives de versions.

### 11.4 Objets de transfert

* paquets offline;
* modules exportables;
* rapports de terrain;
* protocoles d’adaptation;
* documentation d’implantation;
* grilles de maturité;
* guides pour partenaires.

### 11.5 Objets de reconnaissance

* portfolios;
* preuves de compétence;
* badges internes;
* attestations éventuelles;
* journaux de progression;
* productions validées.

---

## 12. Risques architecturaux

### 12.1 Risque de confusion institutionnelle

Le projet peut être mal compris s’il est présenté comme une université parallèle ou un système total.

Réponse :

> utiliser un langage institutionnel sobre : projet de formation numérique inclusive, pilote collégial, hypothèse CCTT.

---

### 12.2 Risque de surcentralisation technique

Le projet peut devenir fragile s’il dépend d’un seul outil.

Réponse :

> maintenir une architecture modulaire : Moodle pour former, Konnaxion pour gouverner, SemantiK pour rendre multilingue, SenTient pour structurer, exports offline pour distribuer.

---

### 12.3 Risque de surpromesse

Le projet peut sembler trop vaste : université mondiale, IA, prison, Basse-Côte-Nord, CCTT, multilingue.

Réponse :

> commencer par une cohorte hybride locale et produire des preuves modestes mais solides.

---

### 12.4 Risque éthique en milieu carcéral

Le projet peut être perçu comme une exploitation de personnes incarcérées.

Réponse :

> maintenir le milieu carcéral comme terrain de transfert ultérieur, avec participation volontaire, production formative, encadrement, reconnaissance et absence de travail forcé.

---

### 12.5 Risque linguistique

Le multilinguisme peut devenir superficiel ou dépendre seulement de l’IA générative.

Réponse :

> développer des patrons, glossaires, structures sémantiques, validations humaines et outils comme SemantiK Architect.

---

### 12.6 Risque de perte de mémoire

Les pilotes peuvent produire de l’apprentissage sans laisser de traces réutilisables.

Réponse :

> archiver systématiquement les décisions, versions, preuves, rétroactions et corrections.

---

## 13. Principes de conception

### 13.1 Sobriété

Le système doit fonctionner avec des moyens réalistes.

La technologie doit réduire la dépendance, pas l’augmenter.

### 13.2 Modularité

Chaque composante doit pouvoir être utilisée sans rendre toutes les autres obligatoires.

### 13.3 Portabilité

Les contenus doivent pouvoir être exportés, partagés, imprimés, consultés et adaptés.

### 13.4 Traçabilité

Les productions, décisions et corrections doivent laisser des traces.

### 13.5 Accessibilité

Le système doit viser les publics éloignés, empêchés, marginalisés ou non desservis.

### 13.6 Gouvernance humaine

L’IA et les systèmes de vote ou lecture ne doivent pas remplacer la décision humaine.

### 13.7 Apprentissage par production

Les apprenants doivent produire des artefacts utiles, pas seulement consommer des contenus.

### 13.8 Transférabilité

Chaque pilote doit générer des méthodes réutilisables dans d’autres milieux.

---

## 14. Non-objectifs

Le projet ne vise pas, dans sa phase actuelle, à :

* créer immédiatement une université accréditée;
* créer immédiatement un CCTT reconnu;
* remplacer le Cégep de Baie-Comeau;
* remplacer Cégep à distance;
* remplacer les programmes existants;
* devenir un projet uniquement carcéral;
* imposer Konnaxion comme plateforme obligatoire;
* dépendre d’un accès Internet permanent;
* produire des diplômes publics;
* faire de l’IA autonome décisionnelle;
* former à des usages offensifs ou risqués.

---

## 15. Synthèse opérationnelle

La structure optimale du projet est :

```text
Premier pilote :
    cohorte hybride locale
    étudiants + personnel + communauté + experts invités

Méthode :
    formation pratique par production de contenus et outils

Infrastructure :
    UCKK/Moodle + Konnaxion/Ethikos + initkOA + SemantiK + SenTient + exports offline

Premier transfert :
    milieux isolés, notamment Basse-Côte-Nord

Second transfert :
    milieux contraints, dont le carcéral

Trajectoire :
    pilote → preuve → partenaires → laboratoire collégial → hypothèse CCTT
```

Phrase maîtresse :

> **Orphée: Walk Straight développe une infrastructure de formation numérique inclusive, multilingue et sobre, testée localement à Baie-Comeau, puis transférable vers les milieux isolés et contraints où l’accès au savoir est limité.**

---

## 16. Liens avec les autres fichiers du dossier

Ce fichier doit être lu avec :

```text
01_vision-et-positionnement.md
02_probleme-et-justification-territoriale.md
03_mission-cctt-et-hypothese-de-transfert.md
05_modele-pedagogique.md
06_pilote-cohorte-hybride-locale.md
07_terrains-specialises-de-transfert.md
08_gouvernance-ethikos-konnaxion.md
09_technologies-et-infrastructure.md
10_production-contenus-et-procedures.md
11_evaluation-portfolios-microcertifications.md
13_risques-ethique-acceptabilite.md
14_feuille-de-route.md
```

---

## 17. Résumé final

L’architecture générale d’Orphée: Walk Straight doit rester simple malgré l’ambition du projet.

Le cœur n’est pas l’IA.

Le cœur n’est pas la prison.

Le cœur n’est pas un logiciel unique.

Le cœur est :

> **une capacité de formation distribuée qui permet à des personnes et communautés d’apprendre en produisant, de produire en documentant, de documenter en gouvernant, et de transférer les savoirs vers les milieux où ils sont le moins accessibles.**

Formule finale :

```text
Apprendre.
Produire.
Prouver.
Gouverner.
Traduire.
Distribuer.
Transférer.
Se souvenir.
```
