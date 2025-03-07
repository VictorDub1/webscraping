#Titre : Webscraping pour le chargement automatique de pdf dans une revue openedition

#Présentation :

Ce programme est dédié au webscraping. Ici l’objectif était de parcourir automatiquement toutes les rubriques d’une revue scientifiques en Openedition pour télécharger les pdfs (dans le cas présent, environ 10 000 fichiers). Le site cible se présentait de la manière suivante : page d’entrée avec une liste d’édition ; page de l’édition n avec une liste d’articles ; page de l’article présentant un bouton « Télécharger ». 
L’utilité de ce programme réside notamment dans sa stabilité. Des temps d’attentes sont mis en places à chaque étape pour éviter une rupture du programme lié au temps de chargement des différentes pages et documents. En cas de crash, le programme se relance tout seul et reprend au point où il s’est arrêté. La mise en place du programme est adaptée à la cible. Cependant, il peut être facilement adapté pour un site ou pour un usage différent. L’ensemble du code est commenté pour en faciliter la compréhension.

#Bibliothèques :

La bibliothèque principale est selenium, une bibliothèque couramment utilisée pour le webscraping. L’utilisation de cette bibliothèque nécessite l’emploi de chromedriver et Chromium. Pour ma part, j’ai utilisé chromedriver version 1.2.12. compatible avec Chromium Version 114.0.5735.0.
