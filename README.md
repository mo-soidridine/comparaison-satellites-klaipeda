# comparaison-satellites-klaipeda
Analyse comparative des performances de Landsat OLI/TIRS, Sentinel-2 MSI et Kanopus-V à Klaipėda, en Lituanie.

Ce projet porte sur l'analyse comparative des performances de trois différents satellites pour l'étude du territoire de Klaipėda, en Lituanie : Landsat OLI/TIRS, Sentinel-2 MSI et Kanopus-V.

L'objectif est d'évaluer les apports de la télédétection pour identifier les structures urbaines, caractériser l'occupation du sol et analyser les dynamiques territoriales d'une ville portuaire située sur la côte baltique, comparer les caractéristiques spatiales et spectrales des trois satellites, identifier les objets et les structures urbaines, caractériser l'occupation du sol à partir des images satellites, comparer différentes méthodes de classification, et étudier les évolutions de l'occupation du sol et explorer des projections de changements territoriaux.

Données mobilisées

- Landsat 8/9 OLI/TIRS
- Sentinel-2 MSI
- Kanopus-V
- OpenStreetMap
- CORINE Land Cover
- Données géographiques lituaniennes

Méthodologie

1. Analyse des caractéristiques satellitaires

Comparaison des résolutions spatiales, des bandes spectrales et des fréquences de revisite afin d'identifier les avantages et les limites de chaque système pour l'analyse urbaine.

2. Calcul d'indices spectraux

Utilisation de la fonction Image Calculator de TerrSet pour calculer plusieurs indices :

- NDVI : végétation
- NDWI : eau
- MNDWI : eau
- NDBI : bâti
- BSI : sols nus

3. Classification des images

- K-means ;
- Decision Forest ;
- Multilayer Perceptron (MLP) ;
- Self-Organizing Maps (SOM).

Les résultats sont étudiés selon leur capacité à distinguer les espaces bâtis, la végétation, les forêts, les sols nus, les routes et les surfaces en eau.

4. Analyse temporelle et modélisation

Étude des changements d'occupation du sol et exploration des trajectoires possibles de l'évolution territoriale à l'aide d'une modélisation de type Markov.

Principaux enseignements

L'étude met en évidence la complémentarité des systèmes satellitaires. La résolution plus fine de Sentinel-2 facilite l'analyse de plusieurs structures urbaines, tandis que Landsat offre notamment des données thermiques utiles à certaines analyses environnementales.

Les résultats de classification varient selon le capteur et la méthode employée. L'étude souligne également les difficultés liées aux pixels mixtes et à l'hétérogénéité du tissu urbain.

La combinaison de données satellitaires et de sources géographiques de référence permet d'approfondir l'analyse des dynamiques urbaines et littorales.

Outil principal

- TerrSet : calcul des indices spectraux, traitement des images et analyses de classification.


Le rapport PDF de l'étude est disponible dans les fichiers de ce dépôt.

*Travail universitaire réalisé en groupe en Master 1 GAED - Géomatique et Modélisation Spatiale, Aix-Marseille Université.*
