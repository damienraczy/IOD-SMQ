---
id: PROC-001
titre: Gestion des informations documentées
type: Procédure
propriétaire:
  - - Responsable Qualité
version: 0.1
statut: Brouillon
date_creation: 2025-12-08
date_revision:
tags:
  - iso9001
  - qualité
  - administration
vc-id: 01_DRAFT_PROC-001 Gestion des documents_md
---

# Gestion des informations documentées

> [!summary] Résumé
> **Objet :** Cette procédure définit les règles de création, validation, diffusion et archivage des documents du Système de Management de la Qualité (SMQ).
> **Pilote :** Responsable Qualité.

## 1. Objet et domaine d'application
Cette procédure décrit la méthodologie pour gérer le cycle de vie des documents chez IOD (création, mise à jour, retrait). Elle garantit que l'information disponible est toujours valide, lisible et approuvée.

* **Inclus :** Tous les documents internes du SMQ (Politiques, Procédures, Instructions, Formulaires, Enregistrements).
* **Exclu :** Les documents externes non liés au SMQ (ex : documentations techniques fournisseurs non critiques).

## 2. Références et définitions
### 2.1 Documents de référence
* Norme ISO 9001:2015 §7.5 (Informations documentées).

### 2.2 Définitions
* **Information documentée** : Donnée nécessaire pour être contrôlée et maintenue par l'organisme.
* **Brouillon (Draft)** : Document en cours de rédaction, non applicable.
* **Publié** : Document validé et applicable officiellement.
* **Archive** : Version périmée d'un document, conservée pour historique.

## 3. Responsabilités
* **Le Responsable Qualité (RQ) :** Est le garant de l'architecture documentaire. Il valide les documents avant publication et gère l'archivage.
* **Les Pilotes de processus :** Rédigent et tiennent à jour les documents de leur périmètre.
* **Les Collaborateurs :** Consultent uniquement les documents du dossier "02_PUBLIE" et signalent toute erreur ou besoin d'évolution.

## 4. Description du processus

### 4.1 Architecture du système (Obsidian & OneDrive)
Le système documentaire est organisé en quatre dossiers principaux sur le serveur (OneDrive) :

1.  **00_ADMIN** : Ressources techniques, templates et images (Accès restreint : RQ).
2.  **01_DRAFT** : Zone de travail. Tous les documents en cours de création ou de modification sont ici.
3.  **02_PUBLIE** : Zone officielle. Contient uniquement les documents validés en version "vigueur". C'est le seul dossier que le personnel doit consulter.
4.  **03_ARCHIVES** : Historique des anciennes versions.

### 4.2 Cycle de vie d'un document

#### Étape 1 : Création
1.  Le rédacteur crée une nouvelle note dans le dossier **01_DRAFT**.
2.  Il insère le modèle approprié (ex: `t_PROC-000` pour une procédure) via la commande Obsidian.
3.  Il renseigne l'en-tête (Frontmatter) :
    * `statut: Brouillon`
    * `version: 0.1`
4.  Il rédige le contenu.

#### Étape 2 : Revue et Validation
1.  Le document est relu par le pilote compétent ou le RQ.
2.  Une fois le contenu approuvé, le rédacteur modifie l'en-tête pour validation :
    * `statut: Validé`
    * `version: 1.0` (pour la première publication)
    * `date_revision: AAAA-MM-JJ`

#### Étape 3 : Publication (Mise en vigueur)
1.  Le Responsable Qualité déplace physiquement le fichier du dossier **01_DRAFT** vers le dossier **02_PUBLIE** (dans le sous-dossier adéquat : *Stratégie, Processus, ou Procédures*).
2.  Dès cet instant, le document est applicable.

#### Étape 4 : Modification et Versionning
Lorsqu'un document publié doit être modifié :
1.  Le RQ déplace le fichier de **02_PUBLIE** vers **01_DRAFT**.
2.  Avant modification, il crée une copie de sauvegarde dans **03_ARCHIVES** en ajoutant le numéro de version au nom du fichier (ex: `PROC-001_v1.0.md`).
3.  Le document original dans **01_DRAFT** est modifié.
4.  Le numéro de version est incrémenté dans l'en-tête (ex: 1.0 -> 1.1 pour mineur, ou 2.0 pour majeur).
5.  Après validation, le fichier retourne dans **02_PUBLIE**.

## 5. Règles de nommage et format
* **Format :** Tous les documents sont au format Markdown (`.md`).
* **Codification :**
    * `STRAT-XXX` : Documents stratégiques (Politique, Contexte).
    * `PROC-XXX` : Procédures.
    * `INST-XXX` : Instructions de travail.
    * `ENR-XXX` : Formulaires vierges.

## 6. Enregistrements associés
* L'historique des modifications est tracé directement en bas de chaque document dans la section "Historique".
* Les anciennes versions sont conservées dans le dossier `03_ARCHIVES`.

---
## Historique des modifications

| Version | Date | Auteur | Nature de la modification |
| :---: | :---: | :--- | :--- |
| 0.1 | 2025-12-08 | RQ | Création initiale de la procédure |
