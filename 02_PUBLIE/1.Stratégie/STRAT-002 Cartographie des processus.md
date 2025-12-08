---
vc-id: 01_DRAFT_STRAT-002 Cartographie des processus_md
---
id: STRAT-002
titre: Cartographie des processus
type: Stratégie
propriétaire: [[Direction Générale]]
version: 1.0
statut: Validé
date_creation: 2025-12-08
date_revision: 
tags:
  - iso9001
  - processus
  - cartographie
---

# Cartographie des processus IOD

## 1. Objet
Ce document identifie les processus nécessaires au système de management de la qualité d'IOD, leurs séquences et leurs interactions, conformément à l'ISO 9001:2015 §4.4.

## 2. Représentation graphique

```mermaid
graph TD
    %% Clients et Parties Intéressées
    C1[CLIENTS : Besoins & Exigences] --> COM
    C1 --> FORM
    
    %% Processus de Management
    subgraph MANAGEMENT [PILOTAGE]
        PM1(PM-01 Pilotage Stratégique)
        PM2(PM-02 Amélioration Continue & Qualité)
    end

    %% Processus de Réalisation
    subgraph REALISATION [CŒUR DE MÉTIER]
        direction LR
        RD(PR-01 R&D et Innovation Tech)
        COM(PR-02 Développement Commercial)
        EVAL(PR-03 Prestations d'Évaluation)
        FORM(PR-04 Formation)
        
        %% Flux
        RD -->|Outils & Méthodes validés| EVAL
        COM -->|Commandes / Fiches de poste| EVAL
        EVAL -->|Données d'analyse| RD
    end

    %% Processus Support
    subgraph SUPPORT [RESSOURCES]
        PS1(PS-01 Ressources Humaines / Experts)
        PS2(PS-02 IT & Infrastructure)
        PS3(PS-03 Administration & Finances)
    end

    %% Sorties
    EVAL --> C2[CLIENTS : Satisfaction & Résultats]
    FORM --> C2
    
    %% Liens Pilotage et Support
    PM1 --> REALISATION
    SUPPORT --> REALISATION
````

## 3\. Description des processus

### 3.1 Processus de Management (Pilotage)

Ils définissent la stratégie, fixent les objectifs et assurent la dynamique d'amélioration.

  * **PM-01 Pilotage Stratégique :** Définition de la vision, politique, revues de direction.
  * **PM-02 Amélioration Continue :** Gestion des audits, des non-conformités, et surveillance du système.

### 3.2 Processus de Réalisation (Chaîne de valeur)

Ils contribuent directement à la fourniture du service au client.

  * **PR-01 R\&D et Innovation Tech (Cœur scientifique) :**
      * *Finalité :* Concevoir et maintenir à jour les méthodes d'évaluation, les outils psychométriques et les solutions IA. Assurer la veille scientifique.
      * *Lien 8.3 (Conception) :* C'est ici que s'applique la maîtrise de la conception.
  * **PR-02 Développement Commercial :**
      * *Finalité :* Analyser les besoins clients (fiches de poste), établir les contrats et recueillir la satisfaction.
  * **PR-03 Prestations d'Évaluation (Cœur opérationnel) :**
      * *Finalité :* Réaliser l'évaluation des candidats (sourcing, tests, entretiens, rapports) en utilisant les outils fournis par la R\&D.
  * **PR-04 Formation :**
      * *Finalité :* Concevoir et dispenser les actions ponctuelles de formation.

### 3.3 Processus Support (Ressources)

Ils fournissent les ressources nécessaires au bon fonctionnement des autres processus.

  * **PS-01 Ressources Humaines / Experts :** Recrutement des consultants, maintien des compétences, gestion du vivier d'experts.
  * **PS-02 IT & Infrastructure :** Maintien de l'infrastructure informatique, sécurité des données (RGPD), déploiement des outils IA.
  * **PS-03 Administration & Finances :** Gestion administrative, facturation, achats.
	*   *Pilotage :* Direction Générale.
	  *   *Exécution (Corinne Mahault) :* Facturation client, suivi des encaissements, relations CAFAT, gestion administrative quotidienne.
	*   *Exécution (Comptable) :* Tenue des comptes, bilans, déclarations fiscales.

## 4\. Interactions clés

1.  **R\&D $\leftrightarrow$ Évaluation :** La R\&D fournit des méthodes validées ("Boîte blanche") à l'Évaluation. En retour, l'Évaluation fournit des données terrain pour entraîner les modèles (IA) et affiner les méthodes.
2.  **Commercial $\rightarrow$ Évaluation :** La qualité de la "Fiche de poste" (entrée) conditionne la pertinence de l'évaluation (sortie).

-----

## Historique des modifications

| Version |    Date    | Auteur    | Nature de la modification            |
| :-----: | :--------: | :-------- | :----------------------------------- |
|   1.0   | 2025-12-08 | Direction | Création de la cartographie initiale |