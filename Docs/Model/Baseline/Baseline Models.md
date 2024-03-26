# Baseline Model Report

## Analytic Approach

* Le but de ce modèle est de pouvoir déterminer des anomalies dans un jeu de données
* En entrée nous avons le jeu de données préparé avec les différents encodages
* Ce modèle est un modèle detection d'anomalies


## Model Description

* Models and Parameters

  * On est dabord parti sur un modèle d'ensemble : le isolation forest 
  * L'algorithme apprend avec un ensemble d'arbre de décision
  * les hyper-paramètres sont :
    * 'n_estimators': le nombre d'estimateurs,
    * 'max_samples': Le nombre d'échantillons à tirer de X pour entraîner chaque estimateur de base,
    * 'contamination': la proportion d'anomalies dans le jeu de données.
  * Learner hyper-parameters
  * Les meilleurs hyperparamètres sont calculés par une optimisation bayesienne et on a pu trouver:
    * 'n_estimators': 102.7957817274436
    * 'max_samples': 0.12902288328519948
    * 'contamination': 0.012378174798332604


## Conclusion and Discussions for Next Steps

* Ce modèle a servi de base pour notre projet de détection d'anomalies
* On va s'en servir pour retirer les valeurs anormales et faire de la détection de communauté.
