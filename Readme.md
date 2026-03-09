# 🍷 Optimisation de la gestion des données d'une boutique (BottleNeck)

## 📝 Contexte du projet
En tant qu'étudiant en Data & IA j'ai éffectué pour **BottleNeck**, un marchand de vin prestigieux, une mission consistait à centraliser et analyser les données de l'entreprise. L'entreprise utilisait deux systèmes distincts : un outil ERP pour la gestion des stocks et un CMS (WordPress) pour la boutique en ligne, sans lien direct entre les deux.

L'objectif de ce projet est de nettoyer ces données hétérogènes, de les fusionner, de calculer le chiffre d'affaires web et d'effectuer une analyse exploratoire pour détecter d'éventuelles erreurs de prix.

## 🛠️ Outils et Technologies
* **Langage :** Python
* **Manipulation de données :** Pandas, NumPy
* **Visualisation :** Matplotlib, Seaborn
* **Environnement :** Jupyter Notebook

## 🎯 Missions réalisées
1. **Audit et Nettoyage des données (Data Cleaning) :**
   - Traitement de 3 jeux de données : `erp.xlsx`, `web.xlsx`, `liaison.xlsx`.
   - Gestion des valeurs manquantes, suppression des doublons et standardisation des noms de colonnes.
   - Filtrage des données web pour ne conserver que les produits de vente.
2. **Rapprochement des bases de données :**
   - Jointures multiples (Merge) entre l'ERP et le fichier Web grâce au fichier de liaison.
   - Identification d'anomalies de référencement (produits en stock physique mais absents du site internet).
3. **Analyse du Chiffre d'Affaires :**
   - Calcul du chiffre d'affaires par produit et du Chiffre d'Affaires Total réalisé en ligne.
4. **Analyse univariée et Détection d'Outliers :**
   - Visualisation de la distribution des prix (Histogrammes, Boxplots).
   - Utilisation de la méthode mathématique de l'Écart Interquartile (IQR) pour isoler les valeurs aberrantes.
   - Interprétation métier des résultats.

## 📊 Résultats Clés
* 💰 **Chiffre d'Affaires total calculé :** 70 568,60 €
* ⚠️ **Anomalies de référencement :** 91 produits présents dans l'ERP ne sont pas mis en vente sur le site Web (manque à gagner potentiel).
* 📈 **Analyse des Outliers :** Détection de **37 produits** avec un prix considéré comme statistiquement atypique (> 83 €). Après analyse métier, il a été recommandé de conserver ces valeurs car elles représentent de réels produits (Champagnes, Cognacs, Grands Crus) appartenant au segment "Luxe" de la boutique.

## 🚀 Comment exécuter le projet ?
1. Clonez ce dépôt GitHub.
2. Assurez-vous d'avoir installé les bibliothèques requises : `pip install pandas matplotlib seaborn openpyxl`.
3. Ouvrez le fichier `Analyse.ipynb` via Jupyter Notebook ou Google Colab.
4. Exécutez les cellules séquentiellement. *(Note : Les fichiers Excel sources doivent se trouver dans le même répertoire que le notebook).*

---
*Réalisé par **Fogue Arsene Magloire** dans le cadre de ma recherche d'alternance en Data Analysis.*
