# Les chaînes de caractères

On appelle **chaîne de caractères** un ensemble de caractères formant une ou plusieurs phrases.

Une [variable](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/wiki/Les-Variables) peut contenir une chaîne de caractères.

![String Assignation](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/assignation.png)

> On assigne toujours une chaîne de caractères avec des guillemets simples : '

## Manipuler les chaînes de caractères

Il est possible de manipuler les chaînes de caractères pour effectuer des opérations sur celle-ci et ainsi les transformer en fonction du besoin.

### Concaténation de chaîne

> On appelle concaténation l'action de mettre bout à bout deux chaînes de caractères.

Pour concaténer deux chaînes de caractères on utilisera l'opérateur logique ```+```.

![String Concatenation](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/concatenation.png)

**Résultat :**

![String Concatenation's Result](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/concatenation_result.png)

> Pensez aux espaces afin de rendre votre concaténation plus lisible.

### Convertir une chaîne de caractères en minuscules ou en majuscules

Une chaîne de caractères peut être convertie en minuscule ou en majuscule en utilisant [la méthode](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/objects/Les_objets.md#m%C3%A9thodes) approprié : respectivement `toLowerCase()` ou `toUpperCase()`, qui renvoient tous deux la nouvelle chaîne de caractères modifiée.

![String Case](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/case.png)

## Obtenir la longueur d'une chaîne de caractères

Pour obtenir la longueur d'une chaîne (c'est-à-dire le nombre de caractères qui la composent, qu'on appelle également sa taille), il faut utiliser [la propriété](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/objects/Les_objets.md#propri%C3%A9t%C3%A9s) `length`, on obtient ainsi la longueur sous la forme d'une valeur entière.

![String length](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/length.png)

## Accéder à un caractère d'une chaîne

Une chaîne de caractères peut être considérée comme un ensemble de caractères. Chaque caractère est identifié par un numéro, appelé son **index**.

> L'indice du premier caractère d'une chaîne est 0.

Il existe deux possibilités pour accéder à un caractère d'une chaîne :

* Utiliser la méthode `charAt(index)` en indiquant l'index du caractère auquel on souhaite accéder.

![String charAt](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/charat.png)

* Utiliser la syntaxe `string[index]` en indiquant l'index du caractère auquel on souhaite accéder.

![String tabIndex](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/strings/tabindex.png)

> Une chaîne de caractères de taille `10` aura donc pour un index maximal de `9`