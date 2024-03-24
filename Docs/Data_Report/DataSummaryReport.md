# Data Report


## Présentation générale du jeu de données

Le jeu de données de base est composé des informations fournies par l'API de X (ancien twitter). Il contient les informations sur descriptives d'un tweet : les informations sur l'utilisateur, les informations sur le tweet, les mentions, les hashtags.
Les informations sont sur la période de temps allant du 14 Juin 2018 à 04:14:00 jusqu'au 17 juin 2018 à 19:01:00. Il est composé de 118 variables. Il comprend 4569999 observations de tweets dans la plage temporelle.
Afin de réaliser de la manière la plus optimale notre analyse exploratoire, nous avons effectué tout d’abord la préparation de nos données, transformation de nos fichiers json en un dataframe avec uniquement les données qui nous seront nécessaires pour la suite. Ensuite nous avons travaillé individuellement puis avons revu ensemble les résultats obtenus afin de les analyser plus précisemment.

## Description du dataframe
<p>Le dataframe obtenu après préparation des données contient 47 colonnes et 4569999 lignes. Nous constatons plusieurs valeurs manquantes notamment pour les colonnes tweet_coordinates,tweet_country_code, etc. Au total nous avons 7648231 valeurs manquantes.</p>

## Variable cible

<p>Nous partons sur de l'apprentissage non supervisé donc nous n'avons pas de variable cible. Notre but est d'utiliser des algorithmes de détection d'anomalies pour retirer des tweets qui seront jugés anormals et ensuite avec le nouveau jeu de données on va effectuer un graphe de cooccurence pour détecter des communautés.</p>

## Signal
<p>Nous avons effectué une visualisation de notre signal : son évolution dans le temps. On remarque des pics à certains moments. Par exemple le 14 juillet entre 12h et 15h on observe jusqu'à 2500 tweets réalisés. Par contre, entre 04h et 11h, on constate que la fréquence des tweets est très faible. L'objectif pour la suite du projet sera de détecter les anomalies, nous saurons alors si ces pics visualisés sont effectivement des anomalies.</p>

## Analyse exploratoire
Dans le cadre de l'analyse exploratoire nous avons travaillé particulièrement sur les hashtags, les utilisateurs et les langues. Les différents graphes réalisés lors de cette analyse exploratoire sont dans le dossier "Plots".
- <b>Fréquence des hashtags</b>
<p>On peut remarquer une surreprésentation du hashtag WorldCup. Toutefois nous avons été sensibilisés sur le fait que certains mots dont WorldCup seraient beaucoup plus représentés car les données ont été extraites en utilisant ces mots clés. Il serait donc intéressant de plus se pencher sur les autres hashtags dans la suite du projet</p>

- <b>Utilisateurs les plus actifs en terme de nombre de tweets</b>
<p>Sur le graphe "top 50_users.png", nous avons les 50 utilisateurs les plus actifs en terme de nombre de tweets. Nous remarquons que le bot fcbtweetbot est bien au-dessus des autres avec plus de 7000 tweets sur une période de trois jours. Nous avons aussi les deux suivants qui sont à près de 3000 tweets chacun. Sur une période de trois jours, il est légitime de se demander s’il ne s’agit pas de deux bots également.
Nous avons aussi représenté le nombre moyen de hashtags par tweets des 50 utilisateurs les plus actifs. On peut remarquer qu’au maximum le nombre moyen de hashtags pour un tweet est de 8. De manière générale le nombre moyen de hashtags par tweet est 3.</p>

- <b>Nuage des mots présents dans les tweets</b> 
<p>On peut remarquer que les mots les plus présents dans notre jeu de données sont : WorldCup, ESP, Russia2018, PORESP, RUSKSA, etc.</p>

- <b>Langue des tweets</b>
<p>Nous avons réalisé le graphe de fréquence des langues des tweets. L'anglais est la langue la plus représentée dans nos tweets avec 2949138 tweets. Ensuite vient l'espagnol avec 271882 tweets, le portuguais avec 245540 tweets. La langue française est la 7e langue la plus utilisée dans les tweets avec au total 117359 tweets.</p>



