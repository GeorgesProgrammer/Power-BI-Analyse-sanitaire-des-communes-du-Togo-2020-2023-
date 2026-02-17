# 🏥 Analyse sanitaire des communes du Togo (2020–2023)

## 📌 Contexte
Le système de santé publique au Togo fait face à des défis majeurs liés aux disparités territoriales, aux maladies endémiques, à la pression démographique et à l’accès inégal aux infrastructures sanitaires.

Ce projet Power BI s’inscrit dans une démarche d’analyse décisionnelle visant à exploiter des données sanitaires mensuelles afin d’aider les autorités publiques, les collectivités locales et les partenaires de santé à identifier les zones prioritaires et orienter les politiques de santé.

---

## 🎯 Objectifs du projet
- Analyser les performances sanitaires des communes et préfectures
- Identifier les zones en situation d’urgence sanitaire
- Évaluer la disponibilité des ressources humaines et matérielles
- Suivre l’évolution des maladies endémiques et épidémiques
- Analyser les indicateurs clés de santé publique
- Soutenir la prise de décision basée sur les données

---

## 📊 Périmètre des données
- **117 communes**
- **39 préfectures**
- **Période : 2020 – 2023**
- **Granularité : mensuelle**
- **Types de structures sanitaires :**
  - CMS (Centre Médico-Social)
  - USP (Unité de Soins Périphériques)

---

## 🗂️ Modèle de données
Le modèle repose sur **4 tables relationnelles** :

### Tables de dimensions
- **dim_prefectures** : liste des préfectures
- **dim_communes** : communes rattachées à leur préfecture
- **dim_structures** : types de structures sanitaires (CMS, USP)

### Table de faits
- **fait_sante_mensuelle**  
  Contient les indicateurs sanitaires mensuels par commune et par structure :
  - Population
  - Accès à l’eau potable (%)
  - Ressources humaines (médecins, infirmiers)
  - Capacité d’accueil (lits, centres)
  - Taux de vaccination
  - Mortalité maternelle et infantile
  - Cas de paludisme, choléra et COVID
  - Volume d’urgences
  - Satisfaction moyenne
  - Indicateur de zone d’urgence

---

## ⚙️ Hypothèses de modélisation
- Population communale considérée comme stable sur la période
- Chaque commune dispose de deux structures sanitaires (CMS & USP)
- Une commune est classée en **zone d’urgence** si au moins un critère est vérifié :
  - Accès à l’eau potable < 60 %
  - Cas de paludisme > 500
  - Mortalité infantile > 10

---

## 📈 Axes d’analyse

### 🌍 Analyse territoriale
- Comparaison des communes et préfectures
- Cartographie des urgences sanitaires
- Identification des zones vulnérables
- Analyse des disparités régionales

### 🏥 Analyse opérationnelle
- Ressources humaines de santé
- Capacité d’accueil des structures
- Comparaison CMS vs USP
- Accès à l’eau potable

### 🦠 Analyse épidémiologique
- Tendances mensuelles du paludisme
- Évolution du choléra et du COVID
- Analyse de la saisonnalité

### ❤️ Analyse de santé publique
- Mortalité maternelle et infantile
- Taux de vaccination
- Satisfaction des usagers

### 🚨 Analyse des urgences
- Volume d’urgences par commune
- Corrélations avec les infrastructures
- Identification des zones critiques

---

## 📊 Indicateurs clés (KPI)
- Taux d’accès à l’eau potable
- Ratio médecins / population
- Ratio infirmiers / population
- Nombre de centres de santé
- Taux de vaccination
- Cas de maladies (paludisme, choléra, COVID)
- Mortalité maternelle
- Mortalité infantile
- Taux de satisfaction
- Nombre de communes en zone d’urgence

---

## 🛠️ Outils & technologies
- Power BI
- DAX
- Power Query
- Excel

---

## 📦 Livrables
- 📊 Rapport Power BI interactif (5–7 pages)
- 📄 Note d’analyse stratégique
- 📈 Tableaux de bord décisionnels

---

## 🎯 Conclusion
Ce projet démontre comment la Business Intelligence peut soutenir efficacement la santé publique en transformant des données complexes en indicateurs clairs, permettant d’anticiper les urgences sanitaires et d’optimiser l’allocation des ressources.
