# Projet-de-Machine-Learning-# Détection de Défauts dans la Production Industrielle 🏭

Ce projet utilise le **Machine Learning** pour identifier automatiquement les pièces défectueuses en fonction de divers paramètres de production (coût, temps de maintenance, score de qualité, etc.).

## 📌 Objectif du projet
L'objectif est de réduire les pertes industrielles en prédisant si une pièce est conforme ou défectueuse (`DefectStatus`) avant qu'elle ne quitte la chaîne de production.

## 🛠️ Stack Technique
- **Langage** : Python
- **Bibliothèques** : 
  - `Pandas` & `NumPy` : Manipulation des données.
  - `Scikit-Learn` : Construction des modèles (**Random Forest**, **Decision Tree**).
  - `Imbalanced-learn (SMOTE)` : Pour gérer le déséquilibre des classes (moins de défauts que de pièces saines).
  - `Matplotlib` & `Seaborn` : Visualisation des données.

## 📊 Méthodologie
1. **Analyse exploratoire** : Étude des corrélations entre le taux de défauts et les variables comme le `QualityScore` ou les `MaintenanceHours`.
2. **Pré-traitement** : Gestion des valeurs manquantes avec `SimpleImputer` et normalisation.
3. **Gestion du déséquilibre** : Application de la technique **SMOTE** pour augmenter artificiellement le nombre d'exemples de pièces défectueuses et améliorer l'apprentissage.
4. **Modélisation** : Entraînement et optimisation via `GridSearchCV`.

## 📈 Résultats
Le modèle final (Random Forest) a été évalué sur :
- **Précision** : Capacité à ne pas déclarer une pièce saine comme défectueuse.
- **Rappel (Recall)** : Capacité cruciale à détecter *tous* les défauts réels.

## 🚀 Comment l'utiliser
1. Cloner le dépôt : `git clone https://github.com/mouadafylal77/Projet-de-Machine-Learning-.git`
2.![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

3. Installer les dépendances : `pip install pandas scikit-learn imblearn matplotlib seaborn`
4. Lancer le notebook `projet_detection_defauts_industriels`.

---
Contributeurs : Moad Afylal & Sofyane Fritit.

Projet académique de fin de module Machine Learning– Licence Analyse de Données, FSTT 2026.
