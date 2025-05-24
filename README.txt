M1-GAED-GEOMAS 2024-2025 : A.GIBELLO G.NAVENNEC M.TOURNIER 

Le plugin "visualiser_itineraire" a été conçu pour fonctionner avec QGIS 3.40.4 sur Windows 11
Le fonctionnement du plugin "visualiser_itineraire" n'est pas garantie sur d'autres systèmes d'exploitation ou sur des versions de QGIS antérieurs


1 - Gestion des dépendances
Avant d'utiliser le plugin "visualiser_itineraire" il est nécessaire de réaliser les opérations suivantes :

 - ouvrir le terminal OSGeo4W shell

 - éxécuter dans le terminal les lignes de codes suivantes

python -m pip install pygame
python -m pip install pandas
python -m pip install rasterio


2 - Format des données en entrées
Le format des données attendu pour un bon fonctionnement du plugin sont les suivants :

 - Un fichier CSV comportant : 1 champ d'identifiant sans format spécifique, 1 champ de date au format date format "yyyy-MM-dd hh:mm:ss", 2 champs de coordonnées au format float

3 - (optionnel) un fichier raster au format tif

4 - Affichage des itinéraires
Les itinéraires affichés par le plugin "visualiser_itineraire" sont systématiquement transformés dans le système de coordonnées du fond de plan raster.
Si aucun fond de plan n'est choisie, le système de coordonnées des itinéraires est le même que celui du fichier CSV