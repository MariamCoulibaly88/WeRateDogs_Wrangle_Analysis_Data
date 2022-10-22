# DATA Wrangling & Analysis: WeRateDogsTWITTER
## by Mariam COULIBALY

## Project Description:

Les données du monde réel sont rarement claires. L’ensemble de données utiliser dans le cadre de ce projet est l’archive de tweets de l’utilisateur de Twitter **@dog_rates**(https://twitter.com/dog_rates), également connu sous le nom de **WeRateDogs. WeRateDogs** est un compte Twitter qui évalue les chiens des gens avec un commentaire humoristique sur le chien.


## Dataset

Ce projet utilisera des données provenant de trois sources différentes:

**- Les archives Twitter de WeRateDogs :** le fichier **twitter_archive_enhanced.csv** a été fourni par Udacity, disponible en téléchargement. Cette archive contient des données sur plus de 5000 tweets, qui ont été filtré avec des notes à 2356 tweets.

**- Les prédictions de l’image tweet :** ce fichier **image_predictions.tsv** est présent dans chaque tweet selon un réseau neuronal. Il est hébergé sur les serveurs d’Udacity et doit être téléchargé par programme en utilisant la bibliothèque Requests et l’URL suivante: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

**- Twitter API :** en utilisant les ID de tweet dans l’archive Twitter de WeRateDogs, interrogeons l’API Twitter pour obtenir les données JSON de chaque tweet à l’aide de la bibliothèque Tweepy de Python et stockez l’ensemble des données JSON de chaque tweet dans un fichier appelé **tweet_json.txt**. Les données JSON de chaque tweet doivent être écrites sur leur propre ligne. Ensuite, lisez ce fichier .txt ligne par ligne dans un tableau de données pandas avec l’ID du tweet, le nombre de retweets et le nombre de favoris.

## Requirements:
* Jupyter Notebook
* pandas
* NumPy
* requests
* tweepy
* json
* Matplotlib
* Seaborn

## Files:

**1. wrangle_act.ipynb:** Notebook sur le traitement et l'analyse de données.

**2. wrangle_report.pdf:** décrit brièvement nos efforts de traitement de données

**3. act_report.pdf:** communique toutes les observations et affiche les visualisations produites à partir de nos données.

## Summary of Findings

Voici quelques-unes des conclusions de l'analyse des données :

- On peut conclure que les 10 noms de chien les plus populaires sont : **Penny, Charlie, Tucker, Oliver, Cooper**. Suivi de **Lucy** et vient ensuite **Lola, Bo, Sadie et Winston**.
- Il existe une corrélation linéaire positive entre le nombre de retweets et le nombre de favoris.
- On peut voir que le stade de chien le plus courant est **pupper** qui compte **210**, ensuite **doggo** qui compte **78**, **puppo** pour **23** et **flooter** pour **7**.
- On peut conclure que **puppo** est le stade de chien le plus likes, suivi de **doggo**, **flooter** et **pupper**.

