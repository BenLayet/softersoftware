# Maintenabilité
## C'est quoi ?
La **maintenabilité d'un logiciel** c'est la capacité à le faire évoluer.

## Pourquoi c'est important ?
Pour la plupart des logiciels, ajouter des fonctionnalités est de plus en plus coûteux.
Pour une fonctionnalité d'une même complexité métier, ce qui prend quelques heures en début de projet, peut prendre des jours,
voir des mois, une fois que le logiciel comporte de nombreuses fonctionnalités.

> Sans une bonne maintenabilité, le coût d'ajout de fonctionnalité est **exponentiel**.

(TODO: graphe coût de CLEAN ARCHITECTURE)
## Conséquences d'une mauvaise maintenabilité

### Projets qui n'aboutissent pas
Il existe de nombreux cas célèbres d'échecs (TODO à documenter) de projets informatiques qui échouent à cause d'une mauvaise maintenabilité.

### Obsolescence logicielle
Une complexité exponentielle implique qu'à un moment on arrive devant un 'mur de complexité', tel que faire évoluer ne vaut plus le coup.
Il faut repartir à zéro (exemple : netscape)
C'est la première cause d'obsolescence logicielle, avant l'évolution des technologies, et avant l'évolution du métier.

### Surcoûts
Avant d'atteindre le 'mur de complexité', un éditeur logiciel/une équipe de développement peut choisir d'absorber le coût et de recruter
des développeurs et testeurs de façon exponentielle. Mais le risque est important car les revenus sont rarement exponentiels.

### Pénibilité
Travailler sur une base de code de mauvaise qualité implique perte de temps et frustration. Il est plus difficile de 
recruter et de conserver les développeurs compétents, ce qui nuit encore à la qualité du logiciel.

## Les clés d'une bonne maintenabilité
Il existe de nombreux ouvrages et articles qui présentent les principes à respecter pour une bonne maintenabilité.
Étant passionné par le sujet depuis plus de 20 ans, j'ai éprouvé ces principes au long de ma carrière et je souhaite présenter ici ceux qui ont été fondamentaux dans mes différents projets.

### Organisation d'équipe
- les développeurs doivent parler directement avec les utilisateurs
- partager le même vocabulaire
- les développeurs doivent être capable de présenter le métier, en utilisant le vocabulaire métier
### Architecture
- utiliser un framework
- séparation du code métier et des dépendances techniques
- le code métier ne doit pas dépendre des frameworks ou des librairies externes
### Code
- [injection de dépendance](./dependency-injection.fr.md)
### Modélisation 
- utiliser le langage naturel
### Domaine Driven Design
### Clean Architecture
### Tester TDD