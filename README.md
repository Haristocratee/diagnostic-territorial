# Diagnostic socio-économique des communes françaises  
### Aide à la priorisation des investissements publics

##  Objectif du projet
Ce projet vise à **aider les décideurs publics, les cabinets de conseil et les collectivités** à identifier et prioriser les communes françaises nécessitant des investissements publics, à partir d’indicateurs démographiques et socio-économiques.

L’objectif principal n’est pas la performance algorithmique, mais la **production d’insights clairs, interprétables et actionnables**.

---

##  Problématique métier
> Comment identifier les communes qui cumulent une forte pression démographique et une situation socio-économique fragile afin d’orienter efficacement les politiques publiques et les investissements territoriaux ?

---

##  Données utilisées
Les données proviennent exclusivement de **sources ouvertes officielles** :

- **INSEE – Population par commune** (via data.gouv.fr)  
- **INSEE – Revenus fiscaux localisés** (via data.gouv.fr)

### Principaux indicateurs retenus
- Population communale  
- Revenu médian du niveau de vie disponible  
- Indicateurs de dispersion des revenus  

Les contraintes liées au **secret statistique** (valeurs manquantes pour certaines communes) ont été identifiées et intégrées dans l’analyse.

---

##  Stack technique
- **Python** : pandas, numpy, matplotlib, scikit-learn  
- **Google Colab**  
- **Tableau** : visualisation et dashboard décisionnel  
- **Git & GitHub** : versioning et documentation

---

## 🗂️ Structure du projet

```texttext
projet-1-diagnostic-territorial/
├── data/
│   ├── raw/                 # Données brutes issues des sources officielles
│   └── clean/               # Données nettoyées et prêtes à l’analyse
│
├── notebooks/
│   ├── 01_exploration.ipynb # Exploration initiale et compréhension des données
│   ├── 02_nettoyage.ipynb    # Nettoyage, sélection des variables et préparation
│   ├── 03_analyse.ipynb      # Analyse métier et création d’indicateurs
│   └── 04_clustering.ipynb   # Segmentation des communes (clustering)
│
├── dashboard/
│   └── tableau_dashboard.twbx # Dashboard Tableau interactif
│
└── README.md                # Documentation du projet
```

## Méthodologie

### 1️⃣ Exploration des données
- Analyse de la structure des datasets
- Identification des variables pertinentes
- Évaluation de la qualité et des valeurs manquantes

### 2️⃣ Nettoyage et préparation
- Harmonisation des codes géographiques (INSEE)
- Sélection des indicateurs clés
- Création de tables propres et réutilisables

### 3️⃣ Analyse métier
- Jointure des données population / revenus
- Construction d’indicateurs décisionnels
- Identification des communes à enjeux socio-économiques

### 4️⃣ Segmentation des communes
- Standardisation des variables
- Détermination du nombre optimal de clusters via la **méthode du coude**
- Segmentation en **4 typologies socio-économiques interprétables**

---

##  Résultats clés
- Mise en évidence de profils territoriaux distincts
- Identification de communes combinant **forte population et faibles revenus médians**
- Production d’une typologie exploitable pour l’aide à la décision publique

---

##  Dashboard décisionnel
Un **dashboard Tableau interactif** a été conçu afin de :
- visualiser les typologies territoriales
- comparer les profils de communes
- filtrer dynamiquement par population, revenu et cluster

Les clusters ont été renommés en **désignations métier** pour faciliter la lecture par des décideurs non techniques.

---

##  Apports métier
- Traduction de données publiques complexes en **outils décisionnels**
- Segmentation interprétable et orientée usage
- Approche réaliste intégrant les contraintes des données publiques

---

##  Axes d’amélioration
- Intégration de données sur les équipements publics
- Analyse temporelle de l’évolution socio-économique
- Croisement avec des données d’emploi ou de mobilité

---

## 👤 Auteur
**Harry TEGUE**  
Étudiant en reconversion en **Data Science / Data Analytics / Machine Learning**  
📍 Paris, France  
🎯 Recherche d’une **alternance de 18 mois en data science**

---
