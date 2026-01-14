# 📊 Analyse Statistique Avancée des Accidents de la Route aux États-Unis

## 📌 Description du projet
Ce projet vise à analyser un dataset massif d’accidents de la route aux États-Unis en appliquant des **statistiques avancées** et des **visualisations de données**, dans un objectif de **bien social** (prévention routière, sensibilisation et aide à la décision).

L’analyse cherche à identifier les facteurs **temporels**, **météorologiques** et **infrastructurels** influençant la **gravité des accidents**, et à produire des **insights actionnables** présentés de manière compréhensible pour un **public non technique**.

---

## 🎯 Objectifs
- Explorer et comprendre un dataset volumineux (7,7M lignes)
- Réaliser un **EDA complet et justifié**
- Nettoyer les données de manière **logique et conditionnelle**
- Appliquer des **statistiques avancées** :
  - Tests statistiques
  - ANOVA
  - Corrélations
  - Régressions
  - Séries temporelles
  - Analyses multivariées (ACP / MANOVA)
- Produire **au moins 30 interprétations**
- Créer un **rapport écrit** et des **slides Canva**
- Travailler en **collaboration réelle via GitHub**

---

## 🗂️ Structure du projet

```bash
US-Accidents-Advanced-Analysis/
│
├── data/
├   ├── dataset-description.txt  # Description des colonnes
│   └── US_Accidents.zip         # Dataset principal compressé 
│
├── notebooks/
│   ├── EDA.ipynb                # Analyse exploratoire des données
│   └── Statistiques.ipynb       # Tests statistiques & modélisation
│
├── docs/
│   ├── dataset_description.md
│   └── liste_mecanisme_statistique.md
│
├── reporting/
│   ├── rapport.md
│   └── slides_canva.pdf
│
├── requirements.txt
└── README.md
```
---

## 📊 Dataset

**Nom** : US Accidents  
**Période** : Février 2016 → Mars 2023  
- Couverture : 49 State  des États-Unis
- Période : Février 2016 à Mars 2023
- Taille : ~7.7 millions d'accidents (version complète), version échantillonnée : 500,000 lignes
- Nombre de colonnes : 46
- Objectif : Analyse statistique avancée et exploration des facteurs contribuant aux accidents


## 🧪 Méthodologie

Le projet suit une démarche Data Analyst standard :

### 1. EDA (Exploratory Data Analysis)
- Analyse de structure
- Valeurs manquantes
- Distributions
- Analyse temporelle, météo et infrastructure

### 2. Nettoyage raisonné
- Imputation conditionnelle
- Suppression ciblée
- Justification métier

### 3. Statistiques avancées
- Tests statistiques (t-test, chi², ANOVA)
- Corrélations
- Régressions
- Séries temporelles
- ACP / MANOVA

### 4. Reporting & Visualisation
- Graphiques interprétables
- Insights actionnables
- Slides Canva pour public non technique

## 🛠️ Technologies utilisées

- **Python** : pandas, numpy, scipy, statsmodels, matplotlib, seaborn, plotly
- **Git / GitHub**
- **Confluence**
- **Canva**

## ▶️ Installation et exécution

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/zinebettahery/US-Accidents
cd US-Accidents
```
### 2️⃣ Installer les dépendances
```bash
pip install -r requirements.txt
```
3️⃣ Télécharger et préparer le dataset
```bash
- Télécharger le fichier US_Accidents.zip
- Décompresser l’archive
- Placer le fichier US_Accidents.csv dans le dossier data/
```
4️⃣ Exécuter les notebooks
```bash
Ouvrir Jupyter Notebook puis exécuter dans l’ordre :
1. notebooks/EDA.ipynb
2. notebooks/Statistiques.ipynb
```


