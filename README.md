## 🛠 1. Transformation des Données Temporelles
Pour affiner l'analyse et répondre aux objectifs statistiques, nous avons enrichi le dataset initial en décomposant les variables temporelles (`Start_Time`). Cette étape permet d'identifier des cycles précis :

**Analyse Cyclique :**  
- Extraction de l'année, du mois, du jour de la semaine et de l'heure.

**Segmentation Contextuelle :**  
- `season` : Classification en 4 saisons pour étudier l'impact climatique annuel.  
- `day_period` : Segmentation de la journée (Matin, Après-midi, Soirée, Nuit).  
- `is_weekend` : Variable binaire pour comparer le trafic de semaine vs week-end.

## 📈 2. Création de Métriques d'Impact (Indicateurs Clés)
Au-delà des données brutes, nous avons créé des indicateurs de performance pour évaluer les conséquences sociales des accidents :

- `Duration_Minutes` : Calcul du temps d'intervention et de résolution (Différence entre `End_Time` et `Start_Time`). Nous avons filtré les données pour ne conserver que les durées cohérentes (entre 1 min et 24h).  
- `Impact_Social` : Transformation de la durée en variable catégorielle (`Faible`, `Modéré`, `Sévère`, `Critique`). Cet indicateur permet de vulgariser l'analyse pour un public non technique en montrant l'ampleur de la paralysie du trafic.

## 🔍 3. Fiabilité et Validation (Qualité des Données)
Une attention particulière a été portée à la synchronisation des données météorologiques :

- **Analyse du Délai Météo :** Nous avons mesuré l'écart entre l'accident et le relevé météo (`Weather_Timestamp`).  
  **Résultat :** L'écart moyen constaté est de -0.50 minute, confirmant une synchronisation quasi parfaite.

- **Stratégie d'Imputation :** Forts de ce constat, les valeurs manquantes de `Weather_Timestamp` ont été complétées par le `Start_Time` de l'accident, permettant de conserver l'intégralité du volume de données sans biaiser les corrélations météo/gravité.
