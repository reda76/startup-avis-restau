La startup “Avis Restau”, qui met en relation des clients et des restaurants, souhaite améliorer sa plateforme avec une nouvelle fonctionnalité de collaboration. 

![Restau](images/restau.png)

Les utilisateurs pourront par exemple poster des avis et des photos sur leur restaurant préféré. Ce sera aussi l’occasion, pour l’entreprise, de mieux comprendre les avis postés par les utilisateurs.

Voici les différentes étapes que nous allons réaliser :

- analyser les commentaires négatifs pour détecter les différents sujets d’insatisfaction :
- sélection de quelques milliers de commentaires négatifs,
- prétraitement des données textuelles,
- utilisation de techniques de réduction de dimension,
- visualisation des données de grandes dimensions afin de détecter des mots-clés et sujets d’insatisfaction ;


Analyser les photos pour déterminer les catégories des photos : 
- sélection de 100 à 200 photos par catégorie,
- prétraitement des images. Nous allons tester deux approches, une par extraction de descripteurs (SIFT, ORB ou SURF) et une par Transfer Learning d’un réseau de neurones de type CNN,
- utilisation de techniques de réduction de dimension,
- visualisation des données de grandes dimensions en mettant en évidence les catégories des images,
- vérification que les images sont correctement regroupées selon les catégories en réalisant un clustering, puis une comparaison des clusters avec les catégories des images, via un graphique et une mesure. Nous allons analyser également quelles sont les catégories les mieux regroupées,
Cette vérification nous permettra de conclure sur la faisabilité de réaliser ultérieurement une classification supervisée, nous avons bien compris qu’il n’était pas nécessaire à ce stade de réaliser cette classification supervisée ;

- collecter un échantillon de données (environ 200 restaurants et leurs revues) via l’API Yelp :
- récupérer uniquement les champs nécessaires,
- stocker les résultats dans un fichier exploitable (par exemple CSV).