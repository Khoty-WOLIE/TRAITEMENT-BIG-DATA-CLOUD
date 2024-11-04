# OPC_DATA_SCIENTIST_PROJET9
Réalisez un traitement dans un environnement Big Data sur le Cloud


# Traitement Big Data dans le Cloud pour Fruits!

## Contexte

Je suis Data Scientist chez **"Fruits!"**, une start-up innovante dans le secteur de l'AgriTech, qui développe des solutions pour préserver la biodiversité des fruits à travers des robots cueilleurs intelligents. L’objectif est de construire une application mobile permettant de reconnaître les fruits à partir de photos, tout en posant les bases d’une infrastructure Big Data pour le traitement à grande échelle des images de fruits.

Mon rôle est de reprendre et d'améliorer un prototype de chaîne de traitement de données Big Data, initialement mis en place par un alternant, en utilisant **PySpark** dans un environnement **AWS EMR**. L'accent est mis sur la **scalabilité** et la conformité au **RGPD**.

## Objectifs

- **Mettre en place une architecture Big Data** en utilisant **AWS EMR** pour le traitement de données massives.
- **Compléter et optimiser un pipeline de traitement PySpark** basé sur des images de fruits et leurs labels associés.
- **Respecter les contraintes du RGPD** en paramétrant l'architecture pour utiliser des serveurs en Europe.
- **Minimiser les coûts du cloud**, en ne maintenant l'instance EMR que pour les tests et démos.
- **Préparer une démonstration** de la chaîne de traitement, incluant la réduction de dimension et la diffusion des poids du modèle TensorFlow pour les prédictions.

## Étapes du Projet

### Étape 1 : Préparation de la chaîne de traitement en local

1. **Objectif** : Développer une chaîne de traitement PySpark en local pour traiter les données et réduire leur dimension avec **PCA (Principal Component Analysis)**.
2. **Tâches** :
   - Configurer un environnement **PySpark** local.
   - **Nettoyer et préparer les données** d'images de fruits, incluant la conversion au bon format pour le traitement Big Data.
   - **Appliquer la réduction de dimension PCA** sur les données pour diminuer leur volume tout en conservant les caractéristiques importantes.
3. **Livrable** : Un **notebook PySpark** contenant un pipeline fonctionnel de traitement et de réduction de dimensions, prêt à être migré dans le cloud.

### Étape 2 : Migration de la chaîne de traitement dans le Cloud

1. **Objectif** : Migrer la chaîne de traitement dans le cloud en utilisant **AWS EMR** pour distribuer les calculs à l’échelle.
2. **Tâches** :
   - **Créer un cluster EMR** sur AWS, avec des instances adaptées aux calculs distribués.
   - **Configurer les services AWS nécessaires** : **S3** pour stocker les données, **IAM** pour gérer les accès, et **EC2** pour les instances de calcul.
   - Connecter le notebook local au cluster EMR pour **exécuter la chaîne de traitement sur le cloud**.
   - **Broadcast des poids TensorFlow** sur les clusters PySpark pour permettre l'inférence du modèle sur des données distribuées.
3. **Livrable** : Un **notebook PySpark** exécuté dans le cloud sur EMR, incluant les étapes de traitement et de réduction de dimension, avec les poids du modèle TensorFlow distribués.

### Étape 3 : Vérification et préparation de la soutenance

1. **Objectif** : Préparer une présentation claire et concise du projet, expliquant l’architecture cloud et la chaîne de traitement PySpark.
2. **Tâches** :
   - **Vérifier le notebook** pour s'assurer que tous les scripts sont bien commentés et facilement compréhensibles pour la démonstration.
   - **Organiser les données et résultats** pour les rendre accessibles depuis le cloud (via **S3**) pour la présentation.
   - **Créer une présentation** expliquant la mise en place de l’architecture, les choix techniques, et les résultats obtenus.
   - **Pratiquer la démonstration technique** pour garantir une explication fluide et préparer les réponses aux questions techniques.
3. **Livrable** : Une **présentation PDF** expliquant l'architecture Big Data, les choix technologiques et le fonctionnement du pipeline PySpark.

## Technologies Utilisées

- **PySpark** : Pour le traitement des données massives et la réduction de dimension.
- **TensorFlow** : Pour l’inférence du modèle à partir des poids déjà entraînés.
- **AWS EMR (Elastic MapReduce)** : Pour l'exécution distribuée des tâches PySpark.
- **AWS S3** : Pour le stockage des données d’images.
- **AWS IAM** : Pour la gestion des accès et des autorisations dans le cloud.
- **PCA (Principal Component Analysis)** : Pour la réduction de dimension des données.

## Résumé Technique

### PySpark
- Configuration d’un environnement PySpark local pour tester la chaîne de traitement.
- Nettoyage des données et application de PCA pour réduire la dimension des images de fruits.
  
### Cloud AWS
- Mise en place d’un cluster EMR pour distribuer les calculs.
- Utilisation d'AWS S3 pour stocker les données et les résultats de traitement.
- Diffusion des poids TensorFlow via **broadcast** pour l'inférence sur les clusters.

### RGPD
- Utilisation d’instances AWS situées en Europe pour garantir la conformité avec le RGPD.
- Paramétrage des services AWS pour limiter l’accès et sécuriser les données via IAM.

## Points de Vigilance

- **Coûts** : Minimiser les coûts en utilisant le cluster EMR uniquement pour les tests et démos.
- **Conformité RGPD** : Vérifier que tous les traitements de données se font sur des serveurs européens.
- **Scalabilité** : Adapter la chaîne de traitement pour qu'elle supporte un volume croissant de données après le déploiement de l’application mobile.

## Ressources Utiles

- **AWS Documentation** : [EMR Documentation](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-what-is-emr.html)
- **PySpark Documentation** : [PySpark Guide](https://spark.apache.org/docs/latest/api/python/)
- **TensorFlow Keras API for Model Inference** : [TensorFlow Inference Guide](https://www.tensorflow.org/guide/keras/model_inference)
- **PCA (Principal Component Analysis)** : [PCA with PySpark](https://spark.apache.org/docs/latest/ml-features.html#pca)
