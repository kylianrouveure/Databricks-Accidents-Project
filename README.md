# Databricks-Accidents-Project
Exam Formation GitHub / Azure

## Présentation du projet

Le projet était de predire la gravité des accidents. Pour cela, nous avons utilisé la suite Microsoft Azure et Databricks.

## Sources des données

Les jeux de données sont (data.gouv.fr) :
1. carac.csv
2. lieux.csv
3. veh.csv
4. vict.csv

Iris - Get Started, KNN Classifier : https://github.dev/asardell/IUT_SD3/blob/main/Iris - get started.dbc
Tuto clustering, Ilyes Talbi : https://larevueia.fr/xgboost-vs-random-forest-predire-la-gravite-dun-accident-de-la-route/

## Les éléments des notebooks
1. Modelisation.dbc
    A. Importation des CSV
    B. Fusion des CSV
    C. Nettoyage des données (PreProcessing)
    D. Construction des échantillons
    E. Test des classifieurs
    F. Export des résultats

2. Test API.dbc
Nous testons l'API


## Les modèles utilisés et le modèle retenu

On a choisi 3 modéles :
1. KNN - Accuracy: 0.6667, F1-Score: 0.3333
2. Decision Tree - Accuracy: 0.6667, F1-Score: 0.4000
3. Random Forest - Accuracy: 0.6667, F1-Score: 0.4000

Avec les performances, nous avons gardé la méthode KNN

## Le lien de l'endpoint du modèle

https://adb-3510722246019924.4.azuredatabricks.net/serving-endpoints/api-accidents/invocations