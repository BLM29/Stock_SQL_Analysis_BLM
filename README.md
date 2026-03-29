# Analyse des stocks et des ruptures en supply chain avec SQL

Projet personnel réalisé dans une démarche d’apprentissage de l’analyse de données appliquée à la supply chain, à l'aide du langage de gestion de base de donnée SQL.

## Contexte

Une entreprise de distribution gère plusieurs entrepôts régionaux et doit maintenir un niveau de stock suffisant afin de répondre à la demande tout en limitant les coûts de stockage.

Dans ce contexte, l’analyse des niveaux de stock permet d’identifier les situations de rupture, les tensions sur certaines références et les besoins de réapprovisionnement.

## Objectif du projet

L’objectif de ce projet est de modéliser un jeu de données logistique simplifié et d’utiliser SQL pour analyser la gestion des stocks.

Les analyses réalisées permettent notamment de :

- mesurer le taux de rupture de stock
- analyser leur couverture
- identifier les produits sous tension
- comparer la performance des entrepôts
- analyser les réapprovisionnements

## Structure de la base de données

La base repose sur quatre tables principales :

- **produits** : informations sur les références du catalogue
- **entrepots** : informations sur les sites logistiques
- **stock** : état du stock par produit et par entrepôt
- **reapprovisionnements** : commandes de réapprovisionnement

## Scripts SQL

Le projet est organisé en plusieurs scripts SQL :

- **01_create_tables.sql** : création des tables de la base
- **02_insert_data.sql** : insertion des produits et entrepôts
- **03_insert_stock.sql** : insertion des données de stock
- **04_insert_reapprovisionnements.sql** : insertion des commandes de réapprovisionnement
- **05_basic_checks.sql** : vérification de la cohérence des données
- **06_stock_kpis.sql** : calcul des indicateurs principaux
- **07_analyses_detaillees.sql** : analyses détaillées des tensions de stock

## KPI analysés

Plusieurs indicateurs clés ont été calculés :

- taux de rupture de stock
- niveau moyen de stock
- couverture moyenne de stock
- taux de disponibilité par entrepôt
- fréquence de réapprovisionnement

## Analyses réalisées

Les analyses permettent notamment d’identifier :

- les produits sous le point de commande
- les ruptures de stock par entrepôt
- les produits ayant la couverture de stock la plus faible
- les produits les plus fréquemment réapprovisionnés
- la valeur totale du stock par entrepôt

## Principaux enseignements

L’analyse met en évidence plusieurs éléments -> 

- certaines références passent sous le point de commande dans plusieurs entrepôts
- des ruptures de stock apparaissent sur certaines lignes de stock
- certains entrepôts présentent un niveau de disponibilité plus faible
- certains produits nécessitent des réapprovisionnements plus fréquents

## Compétences mobilisées

Ce projet met en œuvre plusieurs compétences en analyse de données :

- modélisation de base de données
- écriture de requêtes SQL
- utilisation des agrégations (SUM, AVG, COUNT)
- jointures entre tables
- calcul d’indicateurs logistiques
- analyse de la gestion des stocks
