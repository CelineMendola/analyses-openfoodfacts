# analyses-openfoodfacts

Ce projet a pour but de proposer une idée d'application à partir des analyses de données du site [openfoodfacts](https://world.openfoodfacts.org/). 

## Description

Les données sont disponibles sur ce [lien](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/parcours-data-scientist/P2/fr.openfoodfacts.org.products.csv.zip).   

Dans le notebook PSante_01_notebooknettoyage.ipynb, on nettoie les données et on effectue une première sélection des variables. Le dataset de sortie est dataset_opff_cleaned.pkl.    
Dans le notebook PSante_02_notebookexploration.ipynb, nous réalisons des analyses de données univariées et bivariées, notamment nous réalisons des tests afin de mesurer 
l'interdépendance des variables: par exemple, "la taille des portions des biscuits dépend-elle de leur catégorie ?" ou bien "la présence du label gluten-free et 
l'écoscore sont-ils indépendants? "  
Noous réalisons également une Analyse en composantes principales. Le fichier fucnctions.py contient l'ensemble des fonctions qui lui sont relatives. 

## Idée d'application 
Notre application aurait pour but d'aider les personnes allergiques/ intolérantes au gluten.  
L'utilisateur entre dans l'application un produit qui contient en général du gluten.  
L'application retourne un ensemble de produits équivalents sans gluten, que l'utilisateur pourrait trier par énergie, teneur en sel, nutriscore...  
Sur la page de chaque produit, on verrions en plus de la description de celui-ci une comparaison des valeurs nutritionnelles moyennes avec l'équivalent du produit avec gluten.  
Des exemples de radarplot sont dans les fichiers PSante_03_cookies.html, PSante_03_pain_de_mie.html et PSante_03_pates.html


