
# Description du dataset US Accidents

---
Open on https://stackedit.io/app#
---

## Présentation générale
- Couverture : 49 State  des États-Unis
- Période : Février 2016 à Mars 2023
- Taille : ~7.7 millions d'accidents (version complète), version échantillonnée : 500,000 lignes
- Nombre de colonnes : 46
- Objectif : Analyse statistique avancée et exploration des facteurs contribuant aux accidents

## Source des données
- Collectées en temps réel via multiples APIs (DOT, caméras, capteurs)
- Données météorologiques intégrées via stations météo locales
- Usage : recherche académique, analyse statistique
- Licence : CC BY-NC-SA 4.0

## Description des colonnes

| Nom de la colonne            | Description | Explication |
|-------------------------------|-------------|------------|
| ID                            | Identifiant unique de l’accident |  |
| Source                        | Source brute des données d’accident | Provenance du signalement (capteur, police, API…) |
| Severity                      | Gravité de l’accident (1-4) | 1 = impact faible, 4 = impact très fort sur le trafic |
| Start_Time                    | Heure de début de l’accident (timezone locale) | Moment où l’accident a commencé |
| End_Time                      | Heure de fin de l’incident | Moment où l’accident a été résolu et la circulation est redevenue normale |
| Start_Lat                     | Latitude du point de départ | Coordonnée GPS pour localisation initiale |
| Start_Lng                     | Longitude du point de départ | Coordonnée GPS pour localisation initiale |
| End_Lat                       | Latitude du point de fin | Coordonnée GPS pour localisation finale si déplacement sur route |
| End_Lng                       | Longitude du point de fin | Coordonnée GPS pour localisation finale |
| Distance(mi)                  | Longueur de route affectée (miles) | Distance sur laquelle la route a été impactée |
| Description                   | Description textuelle fournie par l’utilisateur | Brève description de l’accident |
| Street                        | Nom de la rue | Où l’accident s’est produit |
| City                          | Ville | Nom de la ville où l’accident a eu lieu |
| County                        | Comté | Division administrative de l’état (ex : Los Angeles County) |
| State                         | État | État des USA (ex : CA, NY) |
| Zipcode                       | Code postal | Code postal pour localisation plus précise |
| Country                       | Pays | Toujours "US" dans ce dataset |
| Timezone                      | Fuseau horaire | Ex : Eastern, Central, Mountain, Pacific |
| Airport_Code                  | Code de la station météo la plus proche | Pour lier les données météorologiques locales |
| Weather_Timestamp             | Timestamp de l’observation météo | Heure précise de l’observation |
| Temperature(F)                | Température en Fahrenheit | Température ambiante au moment de l’accident |
| Wind_Chill(F)                 | Température ressentie | Ressentie par effet vent/froid |
| Humidity(%)                   | Humidité relative | Pourcentage d’humidité dans l’air |
| Pressure(in)                  | Pression atmosphérique | Mesurée en pouces de mercure |
| Visibility(mi)                | Visibilité en miles | Distance visible sur la route |
| Wind_Direction                | Direction du vent | Orientation du vent au moment de l’accident |
| Wind_Speed(mph)               | Vitesse du vent | Mesurée en miles par heure |
| Precipitation(in)             | Précipitations | Quantité de pluie/neige tombée en pouces |
| Weather_Condition             | Conditions météorologiques | Ex : Rain, Snow, Fog, Thunderstorm |
| Amenity                       | Présence d’une amenité à proximité | Ex : restaurant, station essence, parking |
| Bump                          | Présence d’un ralentisseur | Dos d’âne ou dispositifs similaires |
| Crossing                      | Présence d’un passage piéton | Permet de savoir si un passage piéton est proche |
| Give_Way                       | Présence d’un panneau "cédez le passage" | Indique la signalisation pour les conducteurs |
| Junction                      | Présence d’une jonction | Intersection avec d’autres routes |
| No_Exit                       | Présence d’une impasse | Route sans issue (cul-de-sac) |
| Railway                       | Présence d’une voie ferrée | Si l’accident est proche d’un passage ferroviaire |
| Roundabout                     | Présence d’un rond-point | Structure circulaire pour gérer le trafic |
| Station                        | Présence d’une station | Ex : station de bus, train à proximité |
| Stop                           | Présence d’un panneau stop | Signalisation pour arrêter le véhicule |
| Traffic_Calming                | Présence de dispositifs de ralentissement | Ex : chicanes, dos d’âne, rétrécissements |
| Traffic_Signal                 | Présence d’un feu de signalisation | Pour réguler le trafic aux intersections |
| Turning_Loop                   | Présence d’un loop de virage | Boucle ou rond-point de virage pour véhicules |
| Sunrise_Sunset                 | Jour ou nuit selon lever/coucher du soleil | Permet d’analyser l’effet de la luminosité |
| Civil_Twilight                 | Période de twilight civil | Temps entre lever/coucher du soleil et crépuscule civil |
| Nautical_Twilight              | Période de twilight nautique | Intervalle utilisé en navigation marine |
| Astronomical_Twilight          | Période de twilight astronomique | Intervalle utilisé pour observations astronomiques |

## Remarques
- Certaines valeurs peuvent être manquantes pour certains jours
- La version échantillonnée (~500,000 lignes) est recommandée pour un usage pédagogique
- Les données sont distribuées uniquement pour la recherche académique ou analyse statistique

