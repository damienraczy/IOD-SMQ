---
vc-id: To do_md
---
# Analyse de conformité à ISO 9001:2015

Excellente structuration générale. J'identifie des **forces significatives** mais aussi des **lacunes critiques** pour la certification.

## ✓ POINTS FORTS (Clauses bien couvertes)

|Clause ISO|Exigence|Couverture dans votre SMQ|
|:--|:--|:--|
|**5.2**|Politique Qualité|STRAT-001 complète et claire ✓|
|**4.4**|Cartographie processus|STRAT-002 avec flux et interactions ✓|
|**5.1 / 5.3**|Leadership et responsabilités|Rôles explicites dans chaque fiche processus ✓|
|**7.2**|Compétences|PS-01 + PROC-010 (habilitation, supervision, évaluation) ✓|
|**7.5**|Informations documentées|PROC-001 : architecture claire (DRAFT→PUBLIE→ARCHIVES) ✓|
|**8.2**|Exigences clients|PROC-020 : qualification demande + faisabilité ✓|
|**8.3**|Conception/développement|PR-01 : veille, prototypage, validation scientifique ✓|
|**8.5**|Production/prestation|PROC-030 : supervision systématique (relecture Gérant) ✓|
|**Gestion des risques**|Analyse risques/opportunités|Tableaux complets dans PR-01, PR-02, PR-03, PS-01 ✓|
|**Éthique & RGPD**|Conformité légale|REF-001 détaillé (confidententialité, protection données) ✓|

---

## ⚠️ LACUNES CRITIQUES (Exigences ISO manquantes ou incomplètes)

### **Clause 4.1 & 4.2 - Contexte et parties intéressées**

- **Manque :** Aucun document analysant le contexte externe/interne d'IOD
- **Attendu par ISO :**
    - Analyse SWOT ou contexte organisationnel
    - Identification des parties intéressées (clients, consultants, autorités, concurrence)
    - Analyse de leurs besoins (ex: clients → fiabilité; consultants → formations; CNIL → conformité)
- **Action :** Créer un document **"Contexte et Parties Intéressées"** (1-2 pages)

### **Clause 6.2 - Objectifs Qualité annuels**

- **Manque :** Les objectifs ne sont pas formalisés, datés, ni communicables
- **Attendu par ISO :** Document "Objectifs Qualité 20XX" avec:
    - Objectifs mesurables (ex: 100% des rapports relus avant envoi; 0 dépassement délai >72h)
    - Cibles quantifiées (ex: délai moyen 48h; taux satisfaction client >4/5)
    - Responsable assigné
    - Plan d'action pour les atteindre
- **État actuel :** Indicateurs épars dans les fiches processus, mais pas agrégés

### **Clause 9.2 - Audit Interne** ❌ **CRITIQUE**

- **Manque complètement :** Aucune procédure d'audit interne
- **Attendu par ISO :**
    - Programme d'audits annuel (tous les processus audités au moins 1×/an)
    - Procédure : checklist, indépendance de l'auditeur, rapport d'audit, suivi des écarts
    - Exemple de calendrier: Auditer PROC-030 Q1, PROC-020 Q2, etc.
- **Impact :** Sans audits, impossible de certifier ISO 9001

### **Clause 9.3 - Revue de Direction** ❌ **CRITIQUE**

- **Manque complètement :** Aucune procédure formalisée
- **Attendu par ISO :**
    - Réunion planifiée (ex: 1×/trimestre) avec Direction + responsables processus
    - Ordre du jour : bilan objectifs, risques/opportunités, amélioration continue, retours clients, audits
    - PV documenté + décisions enregistrées
- **État actuel :** Probablement fait informellement, mais non tracé

### **Clause 10.2 - Non-conformités et actions correctives** ⚠️

- **Manque :** Pas de procédure formalisée
- **Attendu par ISO :**
    - Formulaire "Rapport de non-conformité" (Qui? Quoi? Où? Pourquoi?)
    - Actions correctives documentées (plan d'action, responsable, délai)
    - Vérification de l'efficacité
    - Exemple: Si un rapport est envoyé sans relecture (écart PROC-030) → déclarer non-conformité → analyser → corriger → vérifier
- **État actuel :** Traité au cas par cas dans PROC-010 (Niveau 1/2/3) mais sans trace formelle

### **Clause 10.3 - Amélioration continue** ⚠️

- **Existe :** Mentionné dans STRAT-001 (PM-02) et PROC-030 ("entretiens clients trimestriels")
- **Manque :** Processus explicite pour capturer + prioriser + mettre en œuvre les améliorations
- **Attendu :** "Procédure d'amélioration continue" avec:
    - Où/comment capturer idées (suggestion boîte, réunions, audits, clients)
    - Qui évalue et priorise
    - Qui pilote la mise en œuvre
    - Traçabilité des améliorations implémentées

### **Clause 8.4 - Maîtrise des prestataires externes** ⚠️

- **Partiellement couverte :** Consultants externes via PROC-010 ✓
- **Manque :** Processus pour les AUTRES fournisseurs (logiciels, hébergement cloud, data centers, tests psychométriques sous licence)
- **Attendu :** Procédure "Achats et maîtrise des prestataires" avec:
    - Évaluation initiale des fournisseurs (compétence, conformité RGPD/IA Act)
    - Critères de sélection
    - Clauses contracuelles (confidententialité, partage de données)

### **Clause 8.6 & 8.7 - Maîtrise des sorties**

- **Clause 8.6 (Libération des services) :** Couvert implicitement par supervision PROC-030 mais sans procédure explicite
- **Clause 8.7 (Sorties non-conformes) :** Pas de processus si une évaluation est découverte défectueuse POST-envoi
- **Exemple manquant :** Que faire si le Gérant détecte une erreur d'analyse 10 jours après l'envoi au client ?

### **Clause 7.4 - Communication** ⚠️

- **Manque :** Aucun document sur la communication (interne + externe)
- **Attendu :**
    - Qui doit connaître la politique qualité ? (Tous les collaborateurs)
    - Comment est-elle diffusée ? (Formation, wiki, mail)
    - Comment les changements au SMQ sont-ils communiqués ?

---

## 📋 STRUCTURE DOCUMENTAIRE : AMÉLIORATIONS

**Manquent des documents clés :**

|Document manquant|Nécessité|Contenu|
|:--|:-:|:--|
|**Manuel Qualité**|HAUTE|Synthèse SMQ : politique, contexte, processus, responsabilités|
|**Domaine du SMQ**|HAUTE|Définition explicite : "Le SMQ s'applique à [activités]. Exclusions : [éventuellement]"|
|**Procédure Audits Internes**|CRITIQUE|Programme, checklist, responsable, traçabilité|
|**Procédure Revue de Direction**|CRITIQUE|Fréquence, ordre du jour, responsables, enregistrement|
|**Procédure Non-conformités**|HAUTE|Déclaration, investigation, actions correctives, suivi|
|**Procédure Amélioration Continue**|HAUTE|Capture d'idées, priorisation, implémentation, suivi|
|**Procédure Achats**|HAUTE|Évaluation fournisseurs, critères, conformité|
|**Procédure Communication**|MOYENNE|Diffusion politique, formation, changelog|
|**Objectifs Qualité annuels**|HAUTE|Tableau mesurable avec cibles et responsables|
|**Contexte et Parties Intéressées**|MOYENNE|Analyse SWOT, parties prenantes, leurs exigences|

---

## 🎯 PLAN D'ACTION RECOMMANDÉ (par priorité)

**IMMÉDIAT (avant certification) :**

1. Créer **PROC-005 Audits Internes** + programmer les audits Q1 2025
2. Créer **PROC-006 Revue de Direction** + planifier RD Q4 2024/Q1 2025
3. Créer **PROC-007 Gestion des non-conformités** + formulaire ENR-001
4. Documenter **Objectifs Qualité 2025** (tableau clair : cible, mesure, responsable)

**COURT TERME (1-2 mois) :** 5. Créer **Procédure Achats/Prestataires externes** (au-delà des consultants) 6. Enrichir **PROC-001** avec section "Communication du SMQ" 7. Ajouter **document "Domaine du SMQ"** + **"Parties Intéressées"** 8. Créer **PROC-008 Amélioration Continue**

**MOYEN TERME (avant certification) :** 9. Créer un **Manuel Qualité** (synthèse 10-15 pages, référençant tous les processus) 10. Mettre en place **tableaux de bord** mesurables (KPIs par processus) 11. Former **interne 2 auditeurs** pour audits internes

---

## 📊 RÉSUMÉ CONFORMITÉ ISO 9001

|Domaine|Couverture|Verdict|
|:--|:-:|:--|
|**Politique & Leadership**|95%|✓ Bon|
|**Processus réalisation**|90%|✓ Bon|
|**Ressources & Compétences**|85%|✓ Bon|
|**Évaluation des performances**|30%|❌ **CRITIQUE**|
|**Amélioration**|40%|❌ **CRITIQUE**|
|**Gestion des risques**|75%|⚠️ À consolider|

**Verdict global :** Fondations solides, mais **3 processus critiques manquent** (Audits, Revue de direction, Non-conformités). Vous êtes à ~70% de conformité ISO 9001.

Avez-vous besoin que je vous propose les **modèles de ces documents manquants** (Procédure Audits, Revue de Direction, etc.) ?