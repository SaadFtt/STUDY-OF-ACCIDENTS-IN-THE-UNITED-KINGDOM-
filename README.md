# STUDY-OF-ACCIDENTS-IN-THE-UNITED-KINGDOM-
# Étude des Accidents au Royaume-Uni (2023/2024)

## Introduction
Ce projet vise à analyser les accidents corporels de la circulation routière au Royaume-Uni en mettant en place un système d’information décisionnelle. Grâce à des outils de Business Intelligence et à une modélisation de Data Warehouse, nous fournissons des insights sur les tendances et les facteurs de risque liés aux accidents.


## Réalisé par

- Fettah Sad

---

## Étapes du Projet

### 1. Analyse des Besoins
#### Problématique
L'objectif initial est de comprendre les facteurs liés aux accidents de la route, en étudiant les corrélations entre le nombre de véhicules, la vitesse, les conditions de conduite, et les taux de mortalité.

#### Données Initiales
Les données incluent :
- *84 525 accidents corporels*
- *108 076 blessés, dont **39 811 hospitalisés*
- *5 318 tués à 30 jours*

> *Facteurs de Risque* : Vitesse, Alcool, Âge, Fatigue, Téléphones portables, Visibilité, etc.

### 2. Critique de l'Existant
Les données d'accidents existantes ne sont pas structurées de manière optimale pour une prise de décision. Ce projet propose de concevoir un Data Warehouse pour mieux organiser et analyser ces données.

---

### 3. Modélisation du Système
#### 3.1 Niveaux Conceptuel, Logique et Physique
La base de données est modélisée en plusieurs niveaux, offrant une vue d'ensemble des relations entre les différents éléments.

#### 3.2 Modélisation Multidimensionnelle
Nous avons structuré notre modèle en suivant des schémas *en étoile* et *en flocon*, afin d'améliorer la facilité d'analyse.

![Schéma de Modélisation](<img width="531" alt="image" src="https://github.com/user-attachments/assets/7e72d58e-20de-48c1-b3d3-01e62e98b874">
) <!-- Remplacez par une image réelle -->
![modele en flocon de neige](https://github.com/user-attachments/assets/49491c0c-33f0-4660-b6e4-a41ca3c16eea)


#### 3.3 Modélisation du Data Warehouse
Les dimensions clés du Data Warehouse incluent :
- *Dim_Date* : Informations temporelles
- *Dim_Conducteur* : Informations sur le conducteur
- *Dim_Vehicule* : Informations sur le véhicule
- *Dim_Route* : Informations sur la route
- *Dim_Cause* : Causes potentielles de l'accident

### 4. Intégration des Données
Pour l'intégration, nous utilisons *Talend OpenStudio* pour extraire, transformer et charger (ETL) les données vers MySQL.

![Processus ETL avec Talend](https://github.com/user-attachments/assets/308c808a-4311-4e8c-87b8-e50dfd752833)
) <!-- Remplacez par une image réelle -->

#### Étapes de l'ETL
1. *Connexion MySQL* : Connexion aux bases de données projet_input et projet_dw.
2. *Création des Jobs* : Automatisation des tâches ETL pour transférer les données des tables sources vers les tables du Data Warehouse.
3. *Chargement des Dimensions* : Les tables de dimension (route, cause, conducteur, véhicule) sont alimentées par les données brutes.

### 5. Visualisation avec Power BI
Pour faciliter l'interprétation, des tableaux de bord interactifs ont été créés à l'aide de *Power BI*. Ces visualisations permettent de suivre les tendances et d’explorer les données selon différents axes d'analyse.

![Tableau de Bord Power BI:analyse d’accident]((https://github.com/user-attachments/assets/f0906316-150a-4bb1-a6fc-cc5f119e6ae6))
![Tableau de Bord Power BI:analyse des taux](https://github.com/user-attachments/assets/72afa781-9034-4d3f-8acc-f7290cd4d816)

<!-- Remplacez par une image réelle -->

#### Exemples de Visualisations :
- *Analyse des Accidents par Région* : Comprendre les zones les plus touchées.
- *Analyse des Facteurs de Risque* : Visualisation de la vitesse et de l’alcool comme facteurs principaux.
- *Taux de Gravité des Accidents* : Taux de mortalité et blessés graves par rapport au nombre total d'accidents.

---

## Conclusion
Ce projet démontre l'importance d'un Data Warehouse pour centraliser et analyser les données sur les accidents de la route. Grâce aux visualisations de Power BI, les responsables peuvent désormais prendre des décisions basées sur des insights précis et comprendre les tendances des accidents au Royaume-Uni.

## Technologies Utilisées
- *XAMPP Server* : Hébergement local.
- *MySQL* : Système de gestion de bases de données.
- *Talend OpenStudio* : Outil ETL pour l’intégration des données.
- *Power BI* : Service de visualisation de données.

## Auteurs
- *Fettah Sad*

## License
Ce projet est sous licence MIT. Consultez le fichier [LICENSE](LICENSE) pour plus de détails.

Pour toute question, contactez les auteurs de ce projet.
