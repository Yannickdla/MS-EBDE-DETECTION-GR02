# Data Report


## General summary of the data

Le jeu de données de base est composé des informations fournies par l'API de X (ancien twitter). Il contient les informations sur descriptives d'un tweet : les informations sur l'utilisateur, les informations sur le tweet, les mentions, les hashtags.
Les informations sont sur la période de temps allant du 14 Juin 2018 à 04:14:00 jusqu'au 17 juin 2018 à 19:01:00. Il est composé de 118 variables. Il comprend 4569999 observations de tweets dans la plage temporelle.
Afin de réaliser de la manière la plus optimale notre analyse exploratoire, nous avons effectué tout d’abord la préparation de nos données, transformation de nos fichiers json en un dataframe avec uniquement les données qui nous seront nécessaires pour la suite. Ensuite nous avons travaillé individuellement puis avons revu ensemble les résultats obtenus afin de les analyser plus précisemment.

## Data quality summary
Notre jeu de données après préparation contient 47 colonnes et 4569999 lignes. Nous constatons plusieurs valeurs manquantes notamment pour les colonnes tweet_coordinates,tweet_country_code, etc. Au total nous avons 7648231 valeurs manquantes.




## Target variable

Nous partons sur de l'apprentissage non supervisé donc nous n'avons pas de variable cible. Notre but est d'utiliser des algorithmes de détection d'anomalies pour retirer des tweets qui seront jugés anormals et ensuite avec le nouveau jeu de données on va effectuer un graphe de cooccurence pour détecter des communautés.

## Signal


## Analyse exploratoire
Dans le cadre de l'analyse exploratoire nous avons 


