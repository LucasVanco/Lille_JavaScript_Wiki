# Les opérations sur les variables

Il est possible d'effectuer diverses opérations sur une ou plusieurs [variables](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/wiki/Les-Variables).

## Opérations mathématiques

Comme en mathématique, il est possible d'effectuer des additions, soustraction, division et multiplication sur les [variables](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/wiki/Les-Variables).

### Opérations basique

Il possible de manipuler les variables via les différents opérateurs mathématiques pour en modifier leurs valeurs.

![Basic Operations](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/basics.png)

Il est possible d'effectuer des opérations sur les variables entres-elles.

![Variable Operations](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/basics_2.png)

Comme en mathématique il est possible d'utiliser les parenthèses pour modifier l'ordre de priorité des opérations.

![Parentheses](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/parentheses.png)

### Modulo

Le `modulo` est une opération mathématique qui permet d'obtenir le reste de la division euclidienne.

![Modulo](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/modulo.png)

### Incrémentation

On appelle `incrémentation` le fait d'ajouter une valeur fixe à une variable.
> Il existe plusieurs manières d'incrémenter une variable.
> 
> L'opérateur `++` ajoute 1 à la variable tandis que l'opérateur `+=` permet d'ajouter une valeur choisie

![Incrementation](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/incrementation.png)

###

> À l'inverse, on appelle `décrémentation` l'action de soustraire une valeur fixe à une variable.
> 
> On utilisera pour cela l'opérateur logique `myVar--` ou `myVar -= 1`.

## Conversions de types

Bien qu'en JavaScript on indique pas le type d'une variable lors de sa déclaration, il reste toutefois possible de modifier celui-ci au cours d'un programme.

### Conversions implicite

Certaines conversions sont dites implicites : elles sont faites **automatiquement** par l'ordinateur.

![Implicite conversion](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/implicit.png)

**Résultat :**

![Implicite conversion result](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/operations/implicit_result.png)

### Conversions explicite

Bien que le JavaScript soit extrêmement tolérant avec les conversions de types, il arrive parfois qu'une conversion de soit pas possible.

>En cas d'échec de conversion d'un nombre, la valeur du résultat est `NaN` (Not A Number).

![NaN](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources//operations/nan.png)

Dans ce cas il va falloir **expliciter** la conversion. C'est à dire qu'il faudra dire au programme comment on souhaite convertir une donnée.

**Conversion vers une chaîne de caractères :**

Pour convertir explicitement une valeur en [une chaîne de caractères](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/strings/Les_chaines_de_characteres.md), il faut utiliser l'instruction `String(expression)` :

![NaN](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources//operations/string_convert.png)

**Conversion vers un nombre :**

Pour convertir explicitement une valeur en un nombre, il faut utiliser l'instruction `Number(expression)` :

![NaN](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources//operations/number_convert.png)
