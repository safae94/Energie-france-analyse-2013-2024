Analyse du Mix Énergétique Régional Français (2013–2024)

Le nucléaire reste-t-il incontournable ? Quelles régions sont déficitaires ?
Analyse complète des données RTE éCO2mix sur 12 ans et 12 régions françaises.


Aperçu du projet
Ce projet analyse 2,7 millions d'observations de production et consommation électrique régionale en France, issues des données officielles RTE (éCO2mix), de janvier 2013 à janvier 2026.
L'objectif est de répondre à deux questions clés :

Quelle est la place du nucléaire dans le mix énergétique français et comment évolue-t-il ?
Quelles régions produisent plus qu'elles ne consomment, et lesquelles sont déficitaires ?


Dashboard Power BI
Page 1 — Mix énergétique et complémentarité des filières
Afficher l'image
Résultats clés :

Le nucléaire représente 65,14 % de la production totale
Les énergies renouvelables atteignent 25,54 % (hydraulique, éolien, solaire)
Le thermique ne représente plus que 7,60 % du mix

Page 2 — Régions déficitaires et risques de tension

Grand Est et Auvergne-Rhône-Alpes sont les plus grands producteurs nets
Île-de-France et Bretagne consomment largement plus qu'elles ne produisent
La consommation nationale atteint 7,93 Md MW sur la période


Technologies utilisées
OutilUsagePython (Pandas, NumPy)Nettoyage et preprocessing des donnéesMatplotlib / SeabornVisualisations exploratoiresPower BIDashboard interactif finalGoogle ColabEnvironnement de développementGitHubVersioning du projet


Étapes de l'analyse
1. Exploration & audit des données

Dataset : 2 752 704 lignes × 32 colonnes
Identification des valeurs manquantes par région et par année
Compréhension des conventions RTE (NaN avant 2021 = 0 explicite après)

2. Nettoyage & feature engineering

Création de 3 DataFrames spécialisés : df_clean, df_tco, df_nucleaire
Stratégie de traitement colonne par colonne (remplacement par 0 vs suppression)
Extraction de la colonne annee pour analyses temporelles

3. Visualisations Python

Mix énergétique moyen (camembert)
Production vs consommation par région (barres groupées)
Distribution des énergies renouvelables
Évolution temporelle par source

4. Dashboard Power BI interactif

Filtres dynamiques : année, région, mois, filière
KPIs en temps réel
2 pages thématiques avec questions business


Principales conclusions

Le nucléaire domine le mix français (65%) mais sa part varie fortement selon les régions
Les régions sans centrale nucléaire (Bretagne, Île-de-France) sont structurellement déficitaires
La production solaire est en forte croissance sur la période 2013-2024
L'hydraulique joue un rôle clé comme énergie d'équilibrage (stockage par pompage)
La saisonnalité est marquée : la consommation pic en hiver, la production solaire en été


Source des données

RTE éCO2mix Régional — données consolidées et définitives
Période : janvier 2013 – janvier 2026
12 régions françaises métropolitaines
Granularité : pas de 30 minutes
Lien : data.rte-france.com


Auteur
Safae — Formation Data Analyst (Liora / DataScientest)
Master Informatique — CNAM
LinkedIn · GitHub
