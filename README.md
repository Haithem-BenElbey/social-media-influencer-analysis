📊 Analyse et Optimisation des Influenceurs sur Instagram, TikTok et YouTube

Ce projet vise à analyser et optimiser la performance des influenceurs sur Instagram, TikTok et YouTube. Il combine un travail complet de collecte, nettoyage, exploration et modélisation des données, ainsi qu’une analyse stratégique avancée destinée à optimiser les campagnes marketing basées sur des partenariats d’influence.

🚀 Objectifs du Projet

Comprendre les caractéristiques et performances des influenceurs sur les trois plateformes.

Évaluer l’engagement réel et la pertinence des créateurs.

Identifier les meilleurs influenceurs selon les catégories, pays, et types de contenu.

Optimiser les budgets de sponsoring grâce à des métriques fiables.

Détecter les profils sous-évalués offrant le meilleur retour sur investissement.

🗂️ 1. Collecte, Fusion et Préparation des Données
✔️ Collecte & Fusion

Téléchargement des datasets Instagram, TikTok et YouTube depuis Kaggle.

Fusion de multiples fichiers CSV en DataFrames combinés pour chaque plateforme (df_combined, dt_combined, dy_combined).

Uniformisation des noms de colonnes pour faciliter les traitements.

✔️ Nettoyage des Données

Suppression des doublons basés sur les noms d’influenceurs.

Conversion des colonnes numériques au format réel (ex : "1.2M", "500K" → valeurs numériques).

Gestion des valeurs manquantes :

Imputation via RandomForestRegressor pour les indicateurs d'engagement.

Remplissage des catégories/pays via valeurs factices cohérentes.

Suppression des colonnes inutiles (S.no, Rank, row-cell).

🔍 2. Analyse Exploratoire (EDA)

Distribution des followers par plateforme.

Analyse des corrélations : followers, engagement, authentic engagement, commentaires.

Étude des catégories et sous-catégories d’influenceurs.

Visualisations : histograms, scatter plots, box plots, heatmaps, sunburst interactif (Plotly).

📈 3. Calcul des Indicateurs et Scoring Avancé

Engagement_Rate : (Avg. Likes + Avg. Comments) / Followers

Authentic_Engagement_Rate

Comments_Rate

Influence_Score : score composite pour évaluer l’impact global.

Estimation du Story_Price basé sur followers + engagement.

🎯 4. Analyse Stratégique & Optimisation Marketing
✔️ Identification des Influenceurs Clés

Influenceurs les plus performants globalement et localement (plateforme, pays, catégorie).

✔️ Optimisation du Budget Sponsoring

Calcul du Coût par 1000 engagements authentiques.

Analyse du rapport qualité / prix de chaque influenceur.

✔️ Stratégie Plateforme & Contenu

Détermination des plateformes les plus efficaces selon la catégorie de contenu.

Analyse de la performance par pays.

✔️ Détection des Opportunités

Identification des influenceurs sous-évalués via segmentation par quantiles.

🧠 5. Techniques et Méthodes Utilisées
🔧 Pré-processing & Imputation

pandas pour la manipulation des datasets.

SimpleImputer et RandomForestRegressor pour remplir les valeurs manquantes.

LabelEncoder pour encoder les variables catégorielles.

⚙️ Feature Engineering

Création de métriques clés :

Influence_Score

Cost_per_Influence_Point : Story_Price / Influence_Score

Cost_per_1000_Authentic_Engagements

📊 Analyses

Agrégation : groupby, mean, idxmax.

Corrélations et régressions linéaires (via seaborn.lmplot).

Segmentation par quantiles.

📉 Visualisation

matplotlib, seaborn, plotly.

🛠️ Technologies

Python

Pandas, Matplotlib, Seaborn, Plotly

Scikit-learn

Google Colab
