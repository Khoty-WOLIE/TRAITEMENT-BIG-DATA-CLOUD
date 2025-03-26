# BIG-DATA-APPLICATION-FRUITS-PYSPARK-AWS-PROJET-FRUITS!

## Aperçu de l'entreprise

![Aperçu du site web](images/DS_projet9.PNG)

## 🍓 Contexte professionnel

En tant que **Data Scientist** chez **Fruits!**, une startup AgriTech spécialisée dans la reconnaissance de fruits par robotique intelligente, j’ai été missionné pour reprendre, améliorer et déployer une **chaîne de traitement Big Data** permettant de préparer les données d’images de fruits pour de futures prédictions via un modèle TensorFlow.

L’objectif est de traiter des **données massives** issues de l’application mobile de reconnaissance de fruits, à l’aide de **PySpark** sur un environnement **AWS EMR**, tout en assurant **la scalabilité**, **la conformité RGPD** et **l’optimisation des coûts**.

---

## 🎯 Objectifs

- Concevoir une architecture **Big Data scalable** avec **AWS EMR**.
- Compléter un pipeline **PySpark** avec réduction de dimension (**PCA**).
- Intégrer les **poids TensorFlow** pour permettre de l’inférence distribuée.
- Garantir la **conformité RGPD** en traitant les données en Europe.
- Préparer une **démonstration technique** de la chaîne de traitement dans le cloud.

---

## 🧩 Étapes du projet

### 🔹 Étape 1 : Développement local de la chaîne de traitement
- Environnement **PySpark** configuré en local.
- Nettoyage des données images (formatage, filtrage, vectorisation).
- Réduction de dimension par **PCA** pour faciliter le traitement massif.
- 📄 **Livrable** : Notebook local PySpark avec pipeline PCA complet.

### 🔹 Étape 2 : Migration vers AWS EMR (Traitement distribué)
- Création d’un **cluster EMR** avec configuration optimisée.
- Utilisation d’**AWS S3** pour le stockage des données et des sorties.
- Intégration des **poids du modèle TensorFlow** via **broadcast PySpark** pour l’inférence.
- 📄 **Livrable** : Pipeline distribué opérationnel sur AWS EMR.

### 🔹 Étape 3 : Présentation et soutenance
- Vérification des notebooks et scripts (commentaires, reproductibilité).
- Préparation d’une **présentation technique** (PDF) expliquant :
  - L’architecture cloud et les services AWS utilisés
  - La chaîne de traitement PySpark
  - Les choix technologiques, coûts et respect du RGPD
- 📄 **Livrable** : Présentation PDF pour la démonstration finale.

---

## 🛠️ Technologies utilisées

- **PySpark** : Traitement parallèle des données, PCA
- **TensorFlow** : Utilisation des poids pour inférence distribuée
- **AWS EMR** : Exécution Big Data à grande échelle
- **AWS S3** : Stockage des données/images et résultats
- **AWS IAM** : Gestion des droits d’accès
- **PCA** : Réduction de dimension sur données d’images

---

## 📂 Livrables

- ✅ Pipeline PySpark local (avec PCA)
- ✅ Pipeline PySpark cloud sur EMR avec diffusion TensorFlow
- ✅ Architecture cloud documentée (cluster EMR, IAM, S3)
- ✅ Présentation de soutenance (format PDF)

---

## 🔐 RGPD et Scalabilité

- Traitement des données exclusivement sur **instances EU AWS** pour conformité RGPD.
- Sécurisation des accès aux buckets S3 via **politiques IAM**.
- Chaîne pensée pour **scalabilité progressive** après mise en production de l’app mobile.

---

## ✅ Résultats

- Pipeline PySpark fonctionnel localement et dans le cloud
- Architecture cloud déployée et reproductible
- Données prêtes pour un usage à grande échelle avec modèle d’inférence intégré
- Soutenance prête à démontrer le potentiel Big Data du système

---

## 🔍 Aperçu

> Ce projet m’a permis de combiner des compétences en **traitement Big Data**, **scalabilité cloud**, **machine learning distribué** et **gestion des contraintes légales (RGPD)** dans un contexte concret d’innovation AgriTech.

---

*Projet réalisé dans un cadre professionnel simulé avec les responsabilités typiques d’un Data Engineer / Data Scientist dans une startup technologique tournée vers l’IA et le traitement massif de données.*
