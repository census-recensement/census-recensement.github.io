## Guide de l’utilisateur et dictionnaire des données

### Introduction

L'inventaire des données du Recensement du Canada est un projet du Partenariat de découverte des données du Recensement du Canada (PDDRC). Il s'agit d'un inventaire bilingue complet des données du recensement remontant jusqu'à 1665, constituant la base du projet de portail de découverte des données du recensement du Canada du PDDRC. L'inventaire comprend des données du recensement (tableaux de données agrégées et fichiers de microdonnées), des documents spatiaux (données spatiales numériques, cartes de référence, cartes thématiques), des rapports analytiques et des monographies, des documents d'archives (rapports du recensement - lorsque l'accès aux documents numérisés est possible) et toute la documentation disponible (tels que les documents de référence généraux et spécifiques, les rapports techniques, les documents de référence géographiques et les produits d'attributs).

L'inventaire du recensement du PDDRC consiste en un ensemble personnalisé de champs de métadonnées qui sont décrits dans ce document. Chaque item a été inventorié séparément en anglais et en français. Certains champs sont alimentés par des listes d'autorité contenant des informations textuelles supplémentaires telles que les définitions et les plages de dates pour lesquelles la terminologie était utilisée. Les listes d'autorité suivantes ont été créées par le projet du PDDRC :

Liste de tous les recensements dans l'énoncé

- Types de contenu

- Sujets

- Couverture géographique

- Unités géographiques

- Auteurs / éditeurs

- Publications
 

Les listes d'autorité, ainsi que de la documentation supplémentaire sur les objectifs et l'énoncé du projet du PDDRC, sont disponibles dans le dépôt Borealis (lien). Des informations générales sont également disponibles sur le site web du projet.

## Utilisation de l’inventaire

Il existe deux méthodes pour effectuer une recherche dans l'inventaire des données du recensement du Canada :

1.	Par le biais de la démonstration de faisabilité du portail de découverte. Ce portail a été créé par l'équipe du projet du PDDRC dans le cadre d'une une subvention de développement de partenariat du CRSH (2021-2025). Il s'agit uniquement d'une démonstration de ce qu'un portail de découverte du recensement du Canada pourrait offrir. Il ne s'agit pas d'un système prêt pour la production. Des problèmes techniques et des temps d'arrêt peuvent survenir. Cependant, nous sommes heureux d'y donner accès afin de faciliter la recherche de documents historiques du recensement.

2.	L'inventaire a été déposé dans le dépôt Borealis du PDDRC (lien) en format .csv. Notez que les fiches d'inventaire pour les deux langues ont été compilées dans un seul fichier de données, de sorte que chaque item du recensement apparaît deux fois (une fois pour chaque langue).

a.	Des conseils pour effectuer des recherches dans la feuille de calcul de l'inventaire. Une façon simple de naviguer dans l'inventaire est d'ouvrir la feuille de calcul dans Excel et d'activer les filtres. Vous pouvez ensuite trier les documents de la base de données à l'aide des filtres. Par exemple, si vous ne souhaitez consulter que les métadonnées en français, filtrez le champ « rowLand » pour la valeur « fr ». Vous pouvez ensuite filtrer par année, sujet, unité géographique et d'autres colonnes.

b.	Notez que nous ne recommandons pas l'utilisation de la fonctionnalité « Explorateur de données » de Borealis pour explorer cet ensemble de données, car elle ne prend pas en compte certaines caractéristiques, telles que la présence de plusieurs valeurs dans une seule cellule.

## Descriptions des champs

### Identifiant unique

#### Nom du champ : 

ItemID

#### Valeurs : 

Identifiant unique pour chaque ligne de la base de données.
Valeurs : Champ numérique

---

### ID

#### Nom du champ :

id

#### Valeurs :

Un identifiant attribué à chaque item lors de l'inventaire. Comme chaque item du recensement apparaît deux fois dans l'inventaire (une ligne en anglais et une en français), chaque identifiant apparaît deux fois dans la base de données afin de relier les documents anglais et français décrivant le même item.

#### Valeurs :

Identifiants alphanumériques uniques

---

### Langue

#### Nom du champ : 

rowLang

#### Valeurs : 

La langue du document dans l’inventaire.

#### Valeurs : 

- en

- fr

---

### Titre

#### Nom du champ : 

itemTitle

#### Définition: 

Le titre de l’item du recensement

#### Notes : 

- Si aucun titre ne figurait sur l’item du recensement, le catalogueur en a créé un et l'a placé entre crochets.

- Si le document n'a été publié que dans une seule langue officielle, un titre dans l'autre langue officielle n'a pas été créé. Dans l'ensemble des résultats pour l'autre langue officielle, le titre apparaîtra tel qu'il a été publié avec une note entre crochets « [English only] » ou « [Français seulement] ».

#### Valeurs : 

champ de texte

---

### Type de contenu

#### Nom du champ : 

itemType

#### Définition : 

Le type de contenu dans l’item du recensement.

#### Valeurs : 

- Tableaux de données agrégées. Tableaux statistiques qui résument les données du recensement.

- Rapports analytiques. Rapports qui analysent les données du recensement. Bien que ces rapports puissent contenir d'autres types de contenu (tableaux de données, etc.), ils ne sont généralement pas inventoriés séparément.

- Produits de référence du recensement. Produits de documentation et d'information. 

- Fiches de recensement. Documents originaux du recensement archivés. Ils sont inclus dans l'inventaire du PDDRC s'ils sont disponibles sous forme de base de données consultable ou téléchargeable. 

- Produits spatiaux numériques. Fichiers de limites géospatiales et autres données géospatiales.

- Produits de référence géographique. Cela comprend la documentation et les produits d'information liés aux données spatiales et cartes, ainsi que des produits d'information sur les attributs (tels que les fichiers de correspondance, GeoSuite, etc.).  

- Microdonnées. Données individuelles anonymisées. Cela comprend des fichiers de microdonnées à grande diffusion (FMGD) produits par Statistique Canada ainsi que les fichiers de microdonnées produits par la communauté des chercheurs.

- Monographies. Analyse d'un livre sur les thèmes du recensement.

- Documentation au niveau du produit. Documentation créée spécifiquement pour guider l'utilisation d'un item particulier.

- Cartes de référence. Cartes montrant les limites géographiques du recensement.

- Rapports techniques. Rapports décrivant la méthodologie et d'autres détails techniques relatifs à la collecte de données et à la production de produits du recensement.

- Cartes thématiques. Cartes montrant les thèmes du recensement.

---

### Supplémentaire

#### Nom du champ : 

itemSupplementary

#### Définition:

Indicateur signalant que l’item n'a pas été publié par une autorité officielle chargée des données du recensement dans le cadre d'une diffusion de données du recensement. Il peut s'agir de données supplémentaires, de formats convertis ou d'une documentation complémentaire créée pour faciliter l'utilisation du matériel officiel.

#### Notes : 

Les produits de données créés ultérieurement à partir de dossiers ou de publications du recensement, tels que des fichiers de microdonnées (créés à partir des archives du recensement) et des fichiers de limites spatiales (créés à partir des cartes de référence) ne sont pas considérés comme supplémentaires. Il s'agit de matériel essentiel. 

#### Valeurs :
 

binaire O/N, où O indique que l’item est supplémentaire.

---

### Année du recensement (de la publication)

#### Nom du champ: 

itemYearPub

#### Valeurs : 

Le recensement avec lequel l’item a été publié, suivi par l'année où le recensement a été effectué.

#### Notes : 

Une seule année peut être enregistrée dans ce champ. Si l’item n'a pas été publié « avec » un recensement, alors il s'agit d'un supplément ou d'une publication a posteriori et ce champ est laissé vide.
 

#### Valeurs : 

Veuillez consulter la liste des années du recensement (lien) pour une liste complète des recensements inclus dans l'inventaire.

---

### Année(s) de recensement couverte(s) par l’item

#### Nom du champ : 

itemYearsCovered

#### Valeurs : 

Tous les recensements couverts par l'item, classés par année de recensement.

#### Notes : 

Plusieurs années de recensement peuvent être enregistrées dans ce champ. Par exemple, si un tableau de données contient des données comparatives pour trois recensements, chacun d'entre eux sera marqué ici.

#### Valeurs : 

Veuillez consulter la liste des années du recensement (lien) pour une liste complète des recensements inclus dans l'inventaire.

---

### Titre parallèle

#### Nom du champ : 

itemTitleParallel

#### Valeurs : 

Le titre dans l'autre langue officielle.

#### Valeurs : 

champ de texte

---

### Auteur/créateur de l'item

#### Nom du champ : 

itemAuthor

#### Valeurs : 

La personne ou l'entité responsable de la création de l'item du recensement.
 

Valeurs : Veuillez consulter la liste des auteurs/créateurs (lien) pour une liste complète inclus dans l'inventaire.

---

### Sujets

#### Nom du champ : 

itemSubject

#### Valeurs : 

Le sujet de l’item du recensement.

#### Notes : 

Les sujets sont sélectionnés à partir d'une liste d'autorités créée et maintenue par l'équipe du projet du PDDRC.

#### Valeurs : 

Veuillez consulter la liste d’autorité associée aux sujets (lien).

---

### Date de parution

#### Nom du champ : 

itemDateRelease

#### Valeurs : 

L'année de parution ou de diffusion de l'item.

#### Notes :
 

Elle se distingue de l'« année du recensement » qui est l'année au cours de laquelle le recensement a été effectué. Si l'année de publication n'est pas connue, ce champ est laissé vide.

#### Valeurs : 

champ de texte.

---

### Couverture géographique

#### Nom du champ : 

itemGeoCoverage

#### Valeurs : 

La zone géographique globale couverte par l'item.

#### Notes : 

Ce champ utilise la terminologie utilisée pour décrire les régions au moment du recensement. Lorsque la terminologie utilisée dans le recensement est incompatible avec les noms officiels de l'époque, les deux termes sont marqués. La liste d’autorité de couverture géographique contient des informations sur la fourchette d'années qui s'applique à chaque territoire colonial et à la province/territoire actuelle.

#### Valeurs : 

Veuillez consulter la liste des autorités associées à la couverture géographique (lien).

---

### Unités géographiques

#### Nom du champ : 

itemGeoUnits

#### Valeurs : 

Les unités géographiques spécifiques par lesquelles les données sont classées.

#### Notes : 

Ce champ utilise la terminologie indiquée sur l’item, même si cette terminologie diffère de l'usage contemporain. La liste d'autorité des unités géographiques fournit des informations sur la fourchette d'années applicable à chaque nom d'unité géographique.

#### Valeurs :
 

Veuillez consulter la liste des autorités associées aux unités géographiques (lien).

---

### Langue

#### Nom du champ : 

itemLanguage

#### Définition: 

La ou les langues de l’item

#### Valeurs : 

- Anglais
- Français

---

### Trouvé dans (document papier original seulement)

#### Nom du champ : 

itemFoundInPrint

#### Valeurs : 

Le volume dans lequel se trouve l'item.

#### Notes : 

Ce champ n'est rempli que pour les documents imprimés à la main et n'est rempli que pour les documents qui font partie d'un volume plus important. 

#### Valeurs : 

Veuillez consulter la liste des publications (lien).

---

### Trouvé dans (fichier numérique)

#### Nom du champ : 

itemFoundInFile

#### Valeurs : 

Le nom de fichier et/ou le numéro d’un fichier particulier dans lequel se trouve cet élément.

#### Notes : 

Ce champ n'est utilisé que dans les cas où plusieurs tableaux distincts (avec leurs propres numéros de tableau) ont été publiés dans un seul fichier informatique. 

#### Valeurs : 

champ de texte 

---

### Numéros de page (document papier original seulement)

#### Nom du champ : 

itemPageNums

#### Valeurs : 

Les numéros de page où l'élément peut être trouvé.

#### Valeurs :
 

champ de texte 

---

### Série de tableaux (document numérique original seulement)

#### Nom du champ : 

itemSeries

#### Valeurs : 

Le nom de la série à laquelle l'item est associé.

#### Notes : 

Ce champ est utilisé pour les noms de séries que Statistique Canada utilise pour organiser les tableaux de données numériques depuis les années 1960; lorsque les tableaux numériques ont été publiés pour la première fois.
Valeurs : (mettre à jour cette page lorsque l'inventaire est terminé)

- Tableaux sommaires de base
- Tableaux de données
- Série dimensions
- Série « Perspective géographique 
- Faits saillants en tableaux
- Série : Le Pays
- Série de profils
- Tableaux thématiques
- Cassettes sommaires pour les utilisateurs

---

### Identifiant du produit

#### Nom du champ : 

itemProdId

#### Valeurs : 

Le numéro d'identification officiel du produit de Statistique Canada / Gouvernement du Canada (le cas échéant).

#### Valeurs : 

Champ de texte.

---

### Format

#### Nom du champ: 

itemFormat

#### Valeurs : 

Le(s) format(s) physique(s) ou numérique(s) dans lequel(s) l’item est disponible.

#### Notes : 

Des sélections multiples sont autorisées.

#### Valeurs : (mettre à jour cette page lorsque l'inventaire sera terminé)

- ASCII text

- CSV

- DOC

- DTA

- IVT

- JPG

- JP2

- MDB

- Microform

- PDF

- Print

- Print XML

- SAV

- TAB

- TXT

- Site web

- XLS

- XML

---

### Système de coordonnées

#### Nom du champ : 

itemCoordSys

#### Valeurs : 

Informations sur le système de coordonnées (s'applique aux cartes et aux données spatiales)

#### Notes : 

Ces informations peuvent ne pas être connues et ne pas être complétées pour toutes les cartes et données spatiales.

#### Valeurs :
 

champ de texte

---

### Accès aux données

#### Nom du champ : 

itemAccess

#### Valeurs : 

URL permettant d'accéder à l'item.

#### Valeurs : 

champ de texte

---

### Documentation et matériel connexes

#### Nom du champ : 

itemRelated

#### Valeurs : 

Liens vers d'autres items connexes de l'inventaire.
Valeurs : Les titres des items inclus dans la base de données d'inventaire.

---

### Numérisation / Qualité des données

#### Nom du champ : 

itemQuality

#### Valeurs : 

Indication de la qualité des données pour les items numérisés et les imprimés originaux.

#### Notes : 

Parmi les quatre valeurs possibles, deux sont sélectionnées dans chaque cas : complet/incomplet et haute/basse qualité.
 

#### Valeurs : 

- Complet
- Incomplet
- Haute qualité
- Basse qualité

---

### Notes d’accès aux données

#### Nom du champ : 

itemAccessNotes

#### Valeurs : 

Notes relatives à l'accès et à l'utilisation de l'item.

#### Valeurs : 

champ de texte

---

### Notes complémentaires

#### Nom du champ : 

itemAdditionalNotes

#### Valeurs : 

Toute autre note pertinente concernant l’item.

#### Valeurs :
 

champ de texte