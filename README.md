# Dr Death – Analyse des meurtres de Harold Shipman avec Power BI

## Contexte du projet

Harold Shipman, médecin généraliste britannique respecté en apparence, a assassiné au moins 215 de ses patients entre 1975 et 1998 en leur administrant des surdoses mortelles d'opiacés. Ce cas, glaçant et sans précédent, a profondément ébranlé la confiance dans le corps médical.

Ce projet vise à analyser les données relatives aux victimes de Shipman, pour tenter de répondre à la question :

> **Quels types de personnes Harold Shipman a-t-il assassinées, et quand sont-elles mortes ?**

Nous utiliserons l’outil **Microsoft Power BI** pour construire un **dashboard interactif** permettant de visualiser les tendances et les schémas dans les crimes de Shipman.

---

## Veille sur Power BI

### Qu’est-ce que Power BI ?

Power BI est une solution de **business intelligence** développée par Microsoft. Elle permet de **collecter, transformer, analyser et visualiser** des données de manière interactive à travers des tableaux de bord (dashboards) dynamiques.

### Fonctionnalités principales

- Connexion à de nombreuses sources de données : fichiers plats (CSV, Excel), bases de données (SQL Server, MySQL, PostgreSQL), APIs, services cloud (Azure, Google Sheets, etc.).
- Visualisations variées : histogrammes, camemberts, cartes géographiques, courbes, jauges...
- Possibilité de créer des **mesures personnalisées** via DAX (Data Analysis Expressions).
- Partage de rapports via **Power BI Service**.

### Avantages

- Interface intuitive et no-code pour les non-développeurs.
- Grande richesse de visualisations.
- Intégration native avec l’écosystème Microsoft.
- Idéal pour le prototypage rapide de dashboards.

### Inconvénients

- Limitations dans la version gratuite (stockage, rafraîchissement auto...).
- Courbe d’apprentissage de DAX pour les analyses complexes.

---

## Données utilisées

Deux fichiers CSV ont été fournis :

- `shipman-confirmed-victims.csv` : informations détaillées sur les victimes (nom, âge, sexe, date de décès, lieu...).
- `shipman-times-comparison.csv` : comparaison des heures de décès entre les patients de Shipman et ceux d'autres médecins généralistes.

---

## Analyse des données

Après importation dans Power BI :

### 1. Nettoyage (via Power Query)

- Vérification du typage des colonnes : dates reconnues, âges convertis en numérique, textes nettoyés.
- Suppression des lignes incomplètes ou doublons éventuels.

### 2. Visualisations créées

#### Distribution des âges des victimes
> Graphique en histogramme montrant que la majorité des victimes avaient plus de 70 ans.

#### Répartition hommes/femmes
> Diagramme circulaire indiquant une majorité de femmes parmi les victimes.

#### Décès par année
> Courbe temporelle permettant de visualiser une augmentation des décès au fil des années.

#### Heures de décès : Shipman vs autres médecins
> Graphique en barres comparatives montrant un pic anormal de décès dans la journée chez Shipman.

### Captures d’écran

---

## Conclusion

L’analyse met en lumière un **profil très ciblé de victimes** : principalement des **femmes âgées**, vivant dans la région de Hyde. La majorité des décès surviennent en **journée**, à des horaires atypiques pour un décès naturel, ce qui alimente les soupçons sur l’intervention active de Shipman.

Grâce à Power BI, nous avons pu **transformer des données brutes en informations compréhensibles** et visuelles, permettant de mieux appréhender les schémas criminels derrière ce cas hors norme.

---

## 📁 Structure du dépôt

