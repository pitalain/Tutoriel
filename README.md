
# Tutoriel: Qu'est-ce que le format datetime : pourquoi et comment l'utiliser?

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

Dans cet exemple, nous pouvoir voir comment obtenir la date, l'heure exacte ainsi que le fuseau horaire à l'instant ou nous exécutons le code.
```python
asd = datetime.datetime.today()
print(asd)
```
![00](https://github.com/pitalain/Tutoriel/assets/132237358/f7d4a838-fdd5-49a3-9828-21e521da243c)

Ceci est un autre exemple nous permettant de voir à travers un autre code pour avoir la date et l'heure exacte à l'instant ou nous exécutons le code 
```python
exple = datetime.datetime.now()
print(exple)
```
![01](https://github.com/pitalain/Tutoriel/assets/132237358/653d5a7f-45b8-45be-88c4-23f7b494fdc7)


Comme on peut le voir la seule différence est avec les méthodes now() et today(). En utilisant la même syntaxe, ceci nous permet d'avoir le même résultat.
En plus, la méthode today() récupère la date du jour à partir de l'horloge interne de l'ordinateur tandis que la méthode

Pour la classe datetime, nous pouvons également afficher uniquement la date, l'heure, les minutes et les secondes.
```python
# Affectation de la date, l'heure, les minutes et les secondes
aff = datetime.datetime(2019, 10, 7, 10, 9, 58)
print(aff)
```

Ce code retournera le résultat: 2019-10-07 10:09:58. Mais il est possible d'exécuter le code en affichant uniquement le mois, l'année, la date, l'heure, les minutes ou les secondes
```python
#Affichage des composantes individuels des dates, d'heures, minutes
print(aff.year)      # Année
print(aff.month)     # Mois
print(aff.day)       # Jour
print(aff.hour)      # Heure
print(aff.minute)    # Minute
print(aff.second)    # Seconde
```

Formatage des dates 
Il est possible également de formater les résultats. L'affichage de la date par-défaut s'effectue au format AAAA-MM-JJ, mais vous pouvez formater des heures et des dates comme vous les souhaitez. 
Il existe une multitude de chaînes de format des dates et d'heures mais dans ce tutoriel, nous allons parcourir quelques unes d'entre elles. Vous pouvez consulter ce lien pour avoir la liste complète 
http://www.python-simple.com/python-modules-autres/date-et-temps.php

Quand vous utilisez des chaînes de format, veillez à placer des espaces, des barres obliques et tout autre élément entre les directives à l'endroit ou vous souhaitez que ces signes apparaissent en sortie.

#Affichage de la date en uttilisant le formatage
```python
print(f"{aff:%A, %d %B, %Y}")
```

Quand le code ci-dessus est exécuté, ce résultat est affiché en sortie: Monday, 07 October, 2019

Pour afficher la date au format JJ/MM/AAAA, utilisez %d%m%Y, de la manière suivante: 
```python
#Affichage de la date au format JJ/MM/AAAA
exple = f"{aff:%d/%m/%Y}"
print(exple)
```





Affichage d'une date
Dans ce cas, nous voyons comment affecter une date pour qu'il nous retourne notre choix. Nous spécifions alors les composantes suivantes année, mois, jour. Il est idéal quand nous n'avons pas à gérer des heures. 
```python
#Demandons lui de nous afficher la date du 2024-2-11
t = datetime.date(2024, 2, 1)
print(t)
```
![02](https://github.com/pitalain/Tutoriel/assets/132237358/cf8345f9-7423-4bd8-9a37-ec0ed3d3784b)

![03](https://github.com/pitalain/Tutoriel/assets/132237358/89d76f8d-f468-4713-9bb3-0286ecf1a014)

Nous voyons ici qu'on a utilisé la classe date pour avoir une date spécifique.

Note: Pour le mois et le jour, assurons nous de ne pas marquer le chiffre 0 devant le deuxième chiffre.
- Par exemple, pour dire le mois de juillet: 7 et non 07.
- Pour le jour 7, mettre 7 au lieu de 07

  Manipulation avec la classse time
  Comme c'est le cas pour la date, nous pouvons afficher l'heure entière avec les composantes suivantes (heure, minutes et secondes)

  ```python
  # Affichage d'une heure spécifique avec tous ses détails

  
  h = datetime.time(11, 19, 52)
  print(h)
```



Références bibliographiques

https://www.youtube.com/watch?v=GzhG26cvmNg&t=541s
https://docs.python.org/fr/3.6/library/datetime.html#datetime-objects
https://www.youtube.com/watch?v=r1Iv4d6CO2Q
