# Projet IA — Données multimodales  
**Classification d’images & Séries temporelles**

---

## 2. Contexte, données et méthodologie

Vous travaillez en tant qu’**ingénieur IA** au sein d’une entreprise spécialisée dans l’analyse et l’exploitation de **données multimodales** (images, textes et séries temporelles).  
L’objectif est d’**optimiser la prise de décision** et d’**améliorer les performances des services** proposés par l’entreprise.

Votre mission consiste à **concevoir, implémenter et documenter** des pipelines de modèles d’apprentissage automatique adaptés aux différents types de données traités.

---

## Méthodologie — Classification d’images

Le projet de **classification d’images** suit une démarche structurée, depuis l’analyse des données jusqu’à l’interprétation et l’explicabilité des prédictions.

### Étapes du projet

1. **Contexte et objectif du projet**  
   Définition du problème de classification et des objectifs à atteindre.

2. **Présentation des données**  
   Description du jeu de données, des classes et des formats d’images.

3. **Analyse exploratoire des données (EDA)**  
   Visualisation des images, analyse de la répartition des classes et détection d’éventuels déséquilibres.

4. **Organisation et chargement des données**  
   Structuration des dossiers et chargement des images à l’aide des outils adaptés.

5. **Prétraitement des données**  
   Redimensionnement, normalisation et préparation des images pour l’entraînement.

6. **Data Augmentation**  
   Application de transformations afin d’améliorer la robustesse et la capacité de généralisation du modèle.

7. **Construction d’un modèle CNN baseline (3 classes)**  
   Implémentation d’un premier réseau de neurones convolutionnel simple.

8. **Compilation du modèle**  
   Choix de la fonction de perte, de l’optimiseur et des métriques d’évaluation.

9. **Entraînement du modèle**  
   Apprentissage du modèle sur les données d’entraînement.

10. **Évaluation des performances**  
    Analyse des métriques (accuracy, loss) sur les jeux de validation et de test.

11. **Analyse détaillée des résultats**  
    Étude des erreurs de classification et des limites du modèle.

12. **Extension à 4 classes**  
    Adaptation du modèle pour gérer une classe supplémentaire.

13. **Expérimentations avancées**  
    Ajustement des hyperparamètres et tests de nouvelles architectures.

14. **Modèles pré-entraînés (Transfer Learning)**  
    Utilisation de réseaux existants (VGG, ResNet, etc.) afin d’améliorer les performances.

15. **Interprétabilité des prédictions (Machine Learning II)**  
    Analyse des prédictions du modèle à l’aide de méthodes d’explicabilité telles que **LIME** ou **Grad-CAM**.

---

## Méthodologie — Séries temporelles (TP Météo)

### Contexte et données

Les données météorologiques sont fournies par l’**API Open-Meteo**, basée sur des ensembles de données de réanalyse issus de différentes sources (stations météorologiques, radars, satellites, etc.).  
Grâce à des modèles mathématiques, cette API permet d’obtenir des informations météorologiques historiques détaillées, y compris pour des zones dépourvues de stations locales.

Dans ce projet, une **série temporelle de température à 2 mètres du sol** est extraite pour une ville donnée, à partir de ses **coordonnées géographiques (latitude, longitude)**.

### Objectif

Développer un **modèle de prédiction** capable d’estimer la température d’une ville donnée avec un **pas de temps de 3 heures**  
(00h, 03h, 06h, …, 21h).

---

### Étapes du projet

- **Étape 1 — Imports et configuration de l’environnement** 
- **Étape 2 — Acquisition des données météo via l’API Open-Meteo** 
- **Étape 3 — Transformation de la série temporelle (agrégation au pas de 3h)** 
- **Étape 4 — Analyse exploratoire des données (EDA)** 
- **Étape 5 — Tests de stationnarité (ADF, KPSS)** 
- **Étape 6 — Découpage train / validation / test** 
- **Étape 7 — Analyse des autocorrélations (ACF)** 
- **Étape 8 — Modélisation statistique ARIMA**
- **Étape 9 — Grid search ARIMA** 
- **Étape 10 — Modélisation statistique SARIMA**
- **Étape 11 — Grid search SARIMA**
- **Étape 12 — Modélisation SARIMAX avec variable exogène (humidité)** 
- **Étape 13 — Évaluation finale ARIMA / SARIMA / SARIMAX**  
- **Étape 14 — Méthodes de Machine Learning (Ridge, Random Forest)**
- **Étape 15 — Analyse des résidus et comparaison finale des modèles**

---

