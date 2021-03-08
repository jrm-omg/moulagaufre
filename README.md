## Moulagaufre

Moulagaufre est le nom de cet exo qui vous fera mettre les mains dans la Programmation Orientée Objet (POO) que nos amis anglo-saxons nomment OOP (Object-oriented programming).

## Programmation orientée quoi ?

Tout d'abord un petit rappel, la programmation orientée objet est une approche, une façon de faire, où l'on créé et manipule des "objets". Un objet peut contenir des données et du code :
- Des données sous la forme de variables (appelées propriétés).
- Et du code sous la forme de fonctions (appelées méthodes).

Il existe de multiples langages POO, mais les plus populaires sont basées sur des classes. C'est à dire que les objets sont des instances de classes.

Par exemple, si vous avez déjà manipulé des bases de données en PHP, il se pourrait bien que vous ayez déjà *instancié* un objet. Regardez l'exemple suivant où l'on instancie un objet `$bdd`, à partir de la classe `PDO`.

```php
$bdd = new PDO("mysql:host=localhost;dbname=test", $user, $pass);
```

Oui, si vous avez déjà fait ça, c'est que vous vous êtes déjà amusé avec de la programmation orientée objet. C'est fou non ? Et maintenant on va se créer notre propre classe [spoiler] qui va s'appeler `Moulagaufre` et qui va nous permettre d'instancier des objets qu'on appellera `gaufre`. À table :

## Exo

1. Dans un nouveau fichier et dans un language de programmation orienté server, créer une nouvelle classe appelée `Moulagaufre`.
2. À l'intérieur de cette classe, déclarer les nouvelles propriétés suivantes :
  - `id`
  - `poids`
  - `nappage`
  - `nappageTableau`, cette propriété est constituée des entrées suivantes :
    - sucre glace
    - caramel beurre salé
    - pâte à tartiner
    - confiture
    - miel
    - sirop d'érable
    - pâté de tête
    - gélée d'angélique
    - sucre roux
    - chantilly
    - sauce samouraï
3. Instancier un nouvel objet appelé `gaufre`, à partir de notre classe `Moulagaufre` et trouver le moyen d'afficher le contenu de cet objet, *juste pour débugger*.
4. Dans notre classe `Moulagaufre`, créer une méthode appelée `setRandomId` dont le rôle est de donner une valeur aléatoire à la propriété `id`
5. Instancier un nouvel objet appelé `gaufre2` puis appelez la nouvelle méthode `setRandomId`.
6. Afficher le contenu de notre objet `gaufre2` qui doit contenir une propriété `id` définie aléatoirement.
7. Dans notre classe, créer une méthode appelée `getId` dont le rôle est de **retourner** la valeur de la propriété `id`
8. Instancier un nouvel objet appelé `gaufre3` puis appelez la nouvelle méthode `setRandomId` puis afficher ce que retourne la méthode `getId`.
9. Dans notre classe, créer une méthode appelée `setRandomPoids` dont le rôle est de donner une valeur aléatoire comprise entre 80 et 95 (grammes) à la propriété `poids`. Créer également une méthode appelée `getPoids` dont le rôle est de **retourner** la valeur de la propriété `poids`. Instancier un nouvel objet `gaufre4`, appeler la méthode `setRandomPoids` puis afficher ce que retourne la méthode `getPoids`.
10. Dans notre classe, créer une méthode appelée `setRandomNappage` dont le rôle est de prendre une entrée aléatoire parmi celles contenues dans la propriété `nappageTableau` et de la définir à `nappage`. Créer également une méthode appelée `getNappage` dont le rôle est de **retourner** la valeur de la propriété `nappage`. Instancier un nouvel objet `gaufre5`, appeler la méthode `setRandomNappage` puis afficher ce que retourne la méthode `getNappage`.

## Pour aller plus loin

1. Premier supplément chantilly : générer 10 gaufres à l'aide d'une boucle et afficher chaque gaufre dans le format suivant :
```
Gaufre n°1
- id : xxx
- poids : xxx g
- nappage : xxx

Gaufre n°2
- id : xxx
- poids : xxx g
- nappage : xxx
```
2. Deuxième supplément chantilly : dans notre classe, créer un constructeur qui appelle de suite nos méthodes `setRandomId`, `setRandomPoids` et `setRandomNappage`. Afficher les propriétés d'un nouvel objet instancié à partir de cette classe.