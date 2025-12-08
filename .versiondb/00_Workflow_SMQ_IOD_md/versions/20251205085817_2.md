---
vc-id: 00_Workflow_SMQ_IOD_md
---
# 00_Workflow_SMQ_IOD : Procédure de Gestion Documentaire Qualité

Ce document décrit le workflow officiel (ISO 9001, Exigence 7.5) pour la création, la modification, la validation et la distribution des informations documentées du SMQ de IOD Ingénierie.

L'architecture repose sur trois outils principaux assurant légèreté, stabilité et traçabilité : **Obsidian** (Interface), **OneDrive** (Distribution), et **GitHub/Git** (Versionnement/Preuve).

---

## 1. Architecture des Outils et Rôles

| Outil                                                                  | Rôle Principal                                                                           | Preuve ISO 9001                 | Utilisation par       |
| :--------------------------------------------------------------------- | :--------------------------------------------------------------------------------------- | :------------------------------ | :-------------------- |
| **Obsidian**                                                           | Interface de lecture et d'édition. Assure la navigation et la lisibilité (Mode Lecture). | Lisibilité et Recherche (7.5.2) | Tous les utilisateurs |
| **Markdown (.md)**                                                     | Format de fichier source. Format léger et pérenne.                                       | Adéquation du support (7.5.2)   | Tous les utilisateurs |
| **OneDrive**                                                           | Distribution et synchronisation en temps réel des fichiers sources.                      | Disponibilité (7.5.3)           | Tous les utilisateurs |
| **[Version control](https://github.com/Yuichi-Aragi/Version-Control)** | Traçabilité des versions directement dans Obsidian.                                      | Maîtrise des versions (7.5.3)   | Rédacteurs et RQ      |

---

## 2. Étapes du Workflow de Documentation

### A. Phase de Rédaction et d'Édition (Rédacteurs) ✍️

Cette phase est dédiée à la création et à la mise à jour des procédures, politiques et enregistrements.

1.  **Ouverture :** Accédez au **Vault** via **Obsidian**.
2.  **Navigation :** Utilisez l'Explorateur d'Obsidian pour localiser le fichier `.md` basé sur la structure des clauses ISO (ex: `Cl.8/8.2.3_Revue_Contrat.md`).
3.  **Édition :** Travaillez en Markdown dans le mode Édition d'Obsidian. Utilisez les liens internes `[[Nom du Fichier]]` pour relier les documents entre eux.
4.  **Prévisualisation :** Vérifiez le rendu final en **Mode Lecture** pour garantir la qualité de la présentation.
5.  **Sauvegarde & synchronisation :** La sauvegarde enregistre le fichier `.md` localement. **OneDrive** assure la synchronisation automatique en ligne.

La consultation se passe dans un dossier en lecture seule.
L'édition se passe dans un dossier "draft".

### B. Phase de Validation et de Versionnement (Responsable Qualité) ✅

Avant d'être publiés, les documents sont à l'état "draft" et stockés dans le répertoire de travail "draft". 
On édite les documents dans le dossier "Draft", 
* **demande de revue** : On demande la validation d'un document particulier
* **revue** : le RQ examine les modifications apportées, il fournit un retour, avec l'acceptation, demande de modification, refus, explication…
* ***validation formelle** : Le RQ informe de la modification d du document et de sa date de mise en effet
* **publication**: le RQ enregistre les modifications dans la version de consultation.

### C. Phase de Consultation et Distribution (Utilisateurs Finaux) 📖

L'accès à la version valide de la documentation est assuré.

1.  **Accès :** Lancez **Obsidian** sur la machine synchronisée via OneDrive.
2.  **Recherche :** Utilisez l'Explorateur pour naviguer par Clause ou la Recherche globale d'Obsidian par mot-clé.
3.  **Consultation :** Consultez le document exclusivement en **Mode Lecture** pour une expérience optimale et non modifiable.
4.  **Version Officielle :** Seuls les fichiers synchronisés par OneDrive j'ai rendu accessible par le RQ sont considérés comme la version officielle et applicable (Exigence 7.5.3).