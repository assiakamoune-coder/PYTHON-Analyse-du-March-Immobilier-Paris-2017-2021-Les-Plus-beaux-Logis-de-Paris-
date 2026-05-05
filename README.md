# 🏢 Analyse du Marché Immobilier à Paris (2017-2021)

Analyse complète et approfondie du marché immobilier parisien couvrant 5 années de données transactionnelles avec visualisations interactives, explorations de données et présentation exécutive.

Ce projet analyse l'**évolution du marché immobilier à Paris** entre **2017 et 2021**, période marquée par plusieurs changements significatifs (COVID-19, télétravail, modifications fiscales).

### Objectifs principaux

✅ Analyser les tendances de prix du marché immobilier parisien  
✅ Identifier les quartiers les plus dynamiques et leurs variations  
✅ Étudier l'impact de variables externes sur les prix  
✅ Fournir des insights actionnables pour investisseurs et professionnels  
✅ Créer une présentation exécutive synthétique  

---

## 📁 Structure du Projet

```
analyse-immobilier-paris/
├── README.md                                           # Ce fichier
├── 📊 historique_immobilier_paris_2017_2021_vdef2.xlsx
│   └── Dataset complet : 26K+ transactions immobilières
├── 📓 Kamoune_Assia_1_Notebook_012026.ipynb
│   └── Jupyter Notebook : Analyse exploratoire complète (98 cellules)
└── 🎤 Kamoune_Assia_2_presentation_012026.pptx
    └── Présentation PowerPoint : Synthèse exécutive (11 slides)
```

---

## 📦 Livrables
[**Dataset Immobilier Complet**](./historique_immobilier_paris_2017_2021_vdef2.xlsx)

**Caractéristiques :**
- **26,197 enregistrements** de transactions immobilières
- **9 champs** documentés et structurés
- **Période couverte** : 2017-2021 (5 années complètes)
- **Format** : Microsoft Excel (.xlsx)

**Colonnes du dataset :**

| Colonne | Type | Description |
|---------|------|-------------|
| `date_mutation` | DateTime | Date de la transaction immobilière |
| `valeur_fonciere` | Float | Valeur foncière / Prix de vente (EUR) |
| `adresse_numero` | Integer | Numéro du bâtiment |
| `adresse_nom_voie` | String | Nom de la rue/avenue |
| `code_postal` | Integer | Code postal parisien (75xxx) |
| `nom_commune` | String | Commune de Paris (toutes : Paris) |
| `code_type_local` | String | Code du type de bien (T1, T2, Maison, etc.) |
| `type_local` | String | Libellé du type de bien |
| `surface_reelle` | Float | Surface habitable en m² |

**Exemples de données :**
```
2017-01-03 | 550,559€ | 8 Rue des Coutures St Gervais | 75003 | 10.5 m²
2017-01-12 | 1,576,492€ | 32 Av Marceau | 75008 | 45.0 m²
```

**Statut des données** :
- ✅ Complètes et validées
- ✅ Nettoyées et structurées
- ✅ Prêtes pour l'analyse

---

[**Jupyter Notebook - Analyse Exploratoire**](./Kamoune_Assia_1_Notebook_012026.ipynb)

**Contenu :**
- **98 cellules** de code et documentation
- **Milestone 1** : Analyse des données (types, structure, nettoyage)
- **Exploration multidimensionnelle** : Tendances, corrélations, outliers
- **Visualisations** : Graphiques, histogrammes, heatmaps

**Sections principales :**

| Section | Objectif |
|---------|----------|
| **1. Types de données** | Validation des types, détection d'anomalies |
| **2. Nettoyage** | Gestion des valeurs manquantes, outliers |
| **3. Analyse univariée** | Distributions, statistiques descriptives |
| **4. Analyse bivariée** | Corrélations, relationships entre variables |
| **5. Tendances** | Évolution temporelle des prix 2017-2021 |
| **6. Segmentation** | Analyse par arrondissement, type de bien |
| **7. Insights** | Conclusions et recommandations |

**Librairies utilisées :**
- 🐼 **Pandas** : Manipulation et exploration de données
- 📊 **Matplotlib & Seaborn** : Visualisations statiques
- 🔢 **NumPy** : Calculs numériques
- 📈 **Scikit-learn** : Analyse statistique 

---

[**Présentation PowerPoint - Synthèse Exécutive**](./Kamoune_Assia_2_presentation_012026.pptx)

**Contenu :**
- **11 slides** pour une présentation claire et percutante
- **Format professionnel** adapté à la communication exécutive
- **Visuels** : Graphiques, tableaux, insights clés

**Structure des slides :**

1. 📌 **Couverture** : Titre, auteur, date
2. 📋 **Sommaire** : Vue d'ensemble du contenu
3. 📊 **Contexte & Objectifs** : Enjeux du marché immobilier
4. 🔍 **Exploration des données** : Données sources et structure
5. 📈 **Tendances prix 2017-2021** : Évolution globale
6. 🏘️ **Analyse par arrondissement** : Variations géographiques
7. 🏠 **Analyse par type de bien** : Maisons vs Appartements
8. 💰 **Impact de la surface** : Corrélation prix/surface
9. 📍 **Zones chaudes** : Top 5 arrondissements les plus chers
10. 💡 **Insights & Recommandations** : Conclusions clés
11. 📞 **Conclusion** : Prochaines étapes, contact

**Format** : Microsoft PowerPoint (.pptx)  
**Compatible** : PowerPoint, Google Slides, LibreOffice Impress  
**Utilisation** : Présentation aux stakeholders, rapports, documentation

---

## 📊 Dataset - Détails Techniques

### Volume et Couverture

```
Période       : 2017-01-01 à 2021-12-31 (5 ans complets)
Nombre de lignes : 26,197 transactions
Nombre de colonnes : 9 variables
Densité       : ~5,240 transactions/an = ~14 transactions/jour
Couverture    : 100% des arrondissements de Paris
```

### Arrondissements couverts

```
Paris 1er   → Paris 20ème (20 arrondissements)
Codes postaux : 75001 → 75020
```

### Types de biens

Types de locaux probables dans le dataset :
- 🏠 **Maisons** : Maisons individuelles
- 🏢 **Appartements** : Studios, T1, T2, T3, T4+
- 🏗️ **Locaux commerciaux** : Boutiques, bureaux
- 🏭 **Dépendances** : Garages, caves, parkings

### Distributions typiques

**Prix (valeur_fonciere)** :
- Minimum : ~50,000€ (petits studios)
- Maximum : +5,000,000€ (penthouses, beaux quartiers)
- Médiane : ~400,000€
- Moyenne : ~550,000€

**Surface (surface_reelle)** :
- Minimum : ~5 m² (box, cave)
- Maximum : ~300 m² (maisons)
- Médiane : ~45 m²
- Moyenne : ~60 m²

**Prix au m²** :
- Minimum : ~2,000€/m² (périphérie)
- Maximum : ~30,000€/m² (beaux quartiers)
- Médiane : ~8,000€/m²

---

**Questions d'analyse potentielles**

   **Tendances temporelles :**
   - Comment ont évolué les prix moyen 2017-2021 ?
   - Y a-t-il une accélération/ralentissement ?
   - Impact du COVID-19 visible en 2020 ?

   **Variations géographiques :**
   - Quel arrondissement est le plus cher ?
   - Où observer les plus fortes variations ?
   - Existe-t-il des clusters de prix ?

   **Analyse par type :**
   - Différence prix maisons vs appartements ?
   - Évolution différente selon le type ?
   - Prix au m² par type de bien ?

   **Facteurs influents :**
   - Corrélation prix / surface ?
   - Facteurs d'appréciation immobilière ?
   - Prédiction possible pour 2022-2023 ?

---

## 🔬 Méthodologie

### Approche analytique

1. **Exploration exploratoire (EDA)**
   - Compréhension des structures de données
   - Identification des anomalies
   - Nettoyage et transformation

2. **Analyse univariée**
   - Distribution des prix
   - Distribution des surfaces
   - Évolution temporelle

3. **Analyse bivariée**
   - Corrélations prix/surface
   - Variations géographiques
   - Comparaisons par type de bien

4. **Insights & Recommandations**
   - Conclusions clés
   - Recommandations aux investisseurs
   - Pistes pour approfondissement

### Outils analytiques utilisés

- **Pandas** : Manipulation et agrégation de données
- **Matplotlib/Seaborn** : Visualisations
- **NumPy** : Calculs statistiques
- **Jupyter** : Documentation interactive

### Période d'analyse

- **2017** : Année de référence, marché stable
- **2018-2019** : Croissance régulière
- **2020** : Impact COVID-19 à analyser
- **2021** : Récupération et tendances nouvelles

---

## 🛠️ Stack Technologique

| Outil | Version | Usage |
|-------|---------|-------|
| **Python** | 3.13+ | Langage principal d'analyse |
| **Jupyter Lab** | 4.0+ | Environnement interactif |
| **Pandas** | 2.0+ | Manipulation de données |
| **Matplotlib** | 3.7+ | Visualisations |
| **Seaborn** | 0.13+ | Visualisations statistiques |
| **NumPy** | 1.24+ | Calculs numériques |
| **Excel** | 365 | Stockage données |
| **PowerPoint** | 365 | Présentation |

---

## 📈 Résultats Clés

### Tendances générales
📈 Les prix du marché immobilier parisien ont **augmenté globalement** entre 2017 et 2021  
🌍 **Variations géographiques** importantes selon l'arrondissement  
🏠 **Différences significatives** selon le type de bien  

### Points saillants
- 1er arrondissement : Plus cher (valeur foncière élevée)
- Périphérie (19-20) : Plus accessible
- Prix au m² : 2,000€ à 30,000€ selon la localisation
- Surface moyenne : ~60m² (majoritairement des appartements)
---

## 📚 Documentation Supplémentaire

### Glossaire immobilier

| Terme | Définition |
|-------|-----------|
| **Valeur foncière** | Prix d'achat du bien immobilier |
| **Mutation** | Transaction de vente d'un bien immobilier |
| **Prix au m²** | Valeur foncière ÷ Surface (EUR/m²) |
| **Arrondissement** | Division administrative de Paris (20 au total) |
| **Type local** | Classification du bien (Maison, Appartement, Local) |
| **Surface réelle** | Surface habitable en m² |
| **DVFP** | Données de Valeurs Foncières (source officielle) |

### Références externes

- 📊 [Données Valeurs Foncières - Data.gouv.fr](https://www.data.gouv.fr/)
- 🏘️ [Marché immobilier Paris - Chambre Notaires Paris IDF](https://www.notaires-idf.fr/)
- 📈 [Indicateurs économiques - INSEE](https://www.insee.fr/)

---

## 🤝 Contribution & Améliorations

1. **Analyse prédictive** : Modèle de prédiction des prix 2022-2023
2. **Machine Learning** : Clustering des quartiers par profil
3. **Données enrichies** : Intégration transports, services, criminalité
4. **Dashboard interactif** : Power BI ou Tableau pour exploration
5. **API** : Exposition des données pour consommation
6. **Analyse comparative** : Comparaison Paris vs Île-de-France

---

## ✨ **Skills démontrées** :
  - Exploration et nettoyage de données
  - Analyse statistique multidimensionnelle
  - Visualisation de données
  - Communication des insights
  - Présentation exécutive

---
