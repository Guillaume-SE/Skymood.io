![Static Badge](https://img.shields.io/badge/html-FD501A?style=for-the-badge&logo=html5&logoColor=white)
![Static Badge](https://img.shields.io/badge/css-306AF1?style=for-the-badge&logo=css3&logoColor=white)
![Static Badge](https://img.shields.io/badge/javascript-EFD81B?style=for-the-badge&logo=javascript&logoColor=black)
![Static Badge](https://img.shields.io/badge/sass-C56293?style=for-the-badge&logo=sass&logoColor=white)

## Qu'est-ce que Skymood ?

Un site permettant de connaître la météo du moment et avoir les prévisions des 24 prochaines heures le tout par tranches de 3 heures et ce pour la totalité des villes du monde.

## De quoi est composé le projet ?

De 2 apis:

[Geoapify](https://www.geoapify.com/) qui va permettre de retourner des coordonnées géographiques permettant d'avoir un positionnement plus précis et respecter les bonnes pratiques demandé par l'api de prévisions météorologiques.

[Openweathermap](https://openweathermap.org/) qui elle va fournir des données météorologiques très complètes et précises.
Il suffit juste de faire quelques convertions simples comme pour la vitesse du vent, les latitudes et longitudes ainsi que pour les fuseaux horaires.

Pour le reste c'est du vanilla !
Il est construit sur une structure type MVC comme ceci:  

**Repository**: Contient mes fetch aux différentes apis.  

**Controller**: Gère les données en faisant les échanges entre repository et view mais également aux fonctions situées dans Other comme pour créer des chemins d'images dynamiquement.  

**View**: Ici c'est la création des affichages, dynamiquement en fonction des données qui sont envoyés par le controller.  

**Model**: Les données récupérées du fichier JSON retourné par les apis.  

**Other**: Tout ce qui va être fonction annexes.  

**Utils**: Stockage de données créés à la main comme les ISO des pays et fonction générique pas forcément propre au projet en cours.  

Il y a également un stockage fait dans le session storage pour qu'il y soit stocké le nom de la ville recherché par l'utilisateur pour que s'il cherche à nouveau la même ville, aucune appel à l'api ne soit effectué.

Bonne visite !
