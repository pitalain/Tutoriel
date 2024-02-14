
# Tutoriel: Qu'est-ce que le format datetime : pourquoi et comment l'utiliser ?

## Introduction 
Comme tout langage en programmation, Python intègre le module datetime, indispensable dans de nombreux projets et structures organisationnelles pour la gestion précise des dates d'échéance et d'enregistrement. Contrairement à certains types de données intégrés, tels que les nombres, Python ne propose pas de structure native pour les dates, d'où l'importance du module datetime pour manipuler efficacement ces informations. Ce module fournit une classe de base abstraite qui offre une gamme de types de données pour les heures et les dates, permettant ainsi une flexibilité et une précision accrues dans la programmation. Dans des contextes de projets complexes, où la gestion du temps est cruciale, le module datetime devient un outil incontournable, facilitant la manipulation et le traitement des informations temporelles. Grâce à cette fonctionnalité, les développeurs peuvent structurer leurs applications de manière plus robuste et efficace, améliorant ainsi la qualité et la fiabilité de leurs logiciels. En somme, l'intégration du module datetime dans Python renforce sa polyvalence et sa pertinence dans une variété de contextes de développement logiciel.

## Fonctionnement du module datetime
Il Permet de créer des objets qui vont représenter le temps avec les heures, les minutes, les secondes et les microsecondes. Il nous donne quatre classes principales pour travailler avec les heures et les dates qui sont : 
- Classe date : pour reprsenter des dates (année, mois, jour) 
- Classe time : représente des heures (heure, minutes, secondes, microsecondes) 
- Classe datetime : représente des dates et des heures combinées
- Classe timedelta : représente une différence entre deux dates ou heures.

  Avant toute manipulation, vous devez importer le module avant de le manipuler
```python
# Section d'importation des modules
import datetime
```

Première manipulation

Dans cet exemple, nous pouvoir voir comment obtenir la date et l'heure exacte à l'instant ou nous exécutons le code.
```python
asd = datetime.datetime.today()
print(asd)
```




