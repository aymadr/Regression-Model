# 📊 Analyse de la performance scolaire des élèves

## 🚀 Objectif du projet
Ce projet vise à identifier le profil d’un élève qui réussit le mieux dans ses études à partir d’un dataset contenant des informations académiques et personnelles.  
Nous avons utilisé un modèle de **régression linéaire** pour prédire le score final d’un élève et analyser les facteurs qui influencent cette réussite.

---

## 📂 Source des données
Le dataset utilisé provient de **Kaggle** :
> *Student Performance Dataset*  
> https://www.kaggle.com/datasets/mahmoudelhemaly/students-grading-dataset/data

Les données incluent :
- Heures d’étude par semaine
- Taux de présence
- Niveau de stress
- Heures de sommeil
- Accès Internet
- Activités extrascolaires
- Niveau d’éducation des parents
- Niveau de revenu familial
- Score total et Grade

---

## ⚙️ Technologies utilisées
- **Python** (pandas, numpy)
- **scikit-learn** (régression, pipeline, validation croisée)
- **matplotlib / seaborn** (visualisations)

---

## 🔑 Étapes réalisées
✅ Analyse exploratoire des données  
✅ Nettoyage et traitement des valeurs manquantes  
✅ Visualisations : corrélations, comparaisons par département, stress, sommeil, présence  
✅ Construction d’un pipeline avec :
- Prétraitement des données (OneHotEncoder pour les variables catégorielles)
- Modèle de régression linéaire  
✅ Validation croisée (5-fold) pour évaluer la robustesse du modèle  
✅ Prédiction d’un score pour un profil d’élève simulé

---

## 📈 Résultats
- **RMSE moyen (validation croisée)** : 7.32  
- **R² moyen (validation croisée)** : -0.00078  

👉 Ces résultats montrent que :
- Le **RMSE** indique une erreur moyenne d’environ 7 points, ce qui peut sembler acceptable en soi.
- Cependant, le **R² négatif** signifie que le modèle **ne parvient pas à expliquer la variance des scores** : il est moins performant que de simplement prédire la moyenne des scores pour tous les élèves.

💡 **Conclusion :**  
Les facteurs sélectionnés (taux de présence, stress, sommeil, activités, etc.) ne permettent pas, dans ce contexte et avec ce modèle, de **prédire efficacement la réussite d’un élève**.  
Cela peut être dû à :
- une faible corrélation entre ces variables et le score final,
- ou un besoin de modèles plus complexes / autres variables pour capturer la réussite.


---

## 💡 À propos
Ce projet a été réalisé dans le cadre d’un exercice de data science pour mettre en pratique :
- la manipulation de données
- la création de modèles prédictifs
- l’évaluation des performances
