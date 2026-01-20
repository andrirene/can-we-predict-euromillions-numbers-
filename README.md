# Les numéros de l’Euromillions sont-ils prédictibles ?

Ce projet vise à analyser si les numéros tirés à l’Euromillions présentent
des structures statistiques pouvant être modélisées et, dans une certaine mesure,
anticipées.

À partir des données historiques des tirages de l’Euromillions (2004–2023),
nous nous intéressons à la **somme des numéros tirés**, qui présente une rareté
des valeurs faibles. Cette caractéristique justifie l’utilisation d’un
**modèle Tobit**, adapté aux variables dépendantes tronquées ou censurées.

## Question de recherche
Existe-t-il des régularités statistiques dans les tirages de l’Euromillions
permettant d’expliquer la somme des numéros tirés ?

## Données
La base de données contient 1 685 tirages de l’Euromillions et plusieurs variables
construites à partir des propriétés mathématiques des numéros :
- Écart-type des numéros tirés
- Présence de nombres consécutifs
- Présence de nombres de la suite de Fibonacci
- Nombre de nombres premiers
- Nombre de multiples de 7
- Intervalle entre le minimum et le maximum des numéros

## Méthodologie
- Estimation par moindres carrés ordinaires (MCO)
- Mise en évidence d’une troncature à gauche pour les faibles sommes
- Estimation d’un modèle Tobit avec un seuil de troncature fixé à 70
- Analyse et interprétation des effets marginaux et des probabilités associées

## Résultats principaux
- L’écart-type, la présence de nombres consécutifs et le nombre de multiples de 7
  influencent positivement la somme des numéros tirés.
- La présence de nombres de Fibonacci, le nombre de nombres premiers et
  l’amplitude de l’intervalle influencent négativement cette somme.
- Le modèle Tobit fournit des estimations plus pertinentes que le MCO
  en présence de données tronquées.

## Contenu du dépôt
- `/report/` : rapport académique complet (PDF)
- `/data/` : description des données et des variables construites
- `/scripts/` : scripts d’estimation (SAS)

## Auteures
ANDE Irene  


Master 1 – Ingénierie de données et Evaluation Econométrique   
Université d’Angers (2024–2025)
