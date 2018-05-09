# Les opérations sur les variables

Il est possible d'effectuer diverses opérations sur une ou plusieurs [variables](./Les_Variables.md).

## Opérations mathématiques

Comme en mathématique, il est possible d'effectuer des additions, soustraction, division et multiplication sur les [variables](./Les_Variables.md).

### Opérations basique

Il possible de manipuler les variables via les différents opérateurs mathématiques pour en modifier leurs valeurs.

![Basic Operations](../../ressources/basics/operations/basics.png)

Il est possible d'effectuer des opérations sur les variables entres-elles.

![Variable Operations](../../ressources/basics/operations/basics_2.png)

Comme en mathématique il est possible d'utiliser les parenthèses pour modifier l'ordre de priorité des opérations.

![Parentheses](../../ressources/basics/operations/parentheses.png)

### Modulo

Le `modulo` est une opération mathématique qui permet d'obtenir le reste de la division euclidienne.

![Modulo](../../ressources/basics/operations/modulo.png)

### Incrémentation

On appelle `incrémentation` le fait d'ajouter une valeur fixe à une variable.
> Il existe plusieurs manières d'incrémenter une variable.
> 
> L'opérateur `++` ajoute 1 à la variable tandis que l'opérateur `+=` permet d'ajouter une valeur choisie

![Incrementation](../../ressources/basics/operations/incrementation.png)

###

> À l'inverse, on appelle `décrémentation` l'action de soustraire une valeur fixe à une variable.
> 
> On utilisera pour cela l'opérateur logique `myVar--` ou `myVar -= 1`.

## Conversions de types

Bien qu'en JavaScript on indique pas le type d'une variable lors de sa déclaration, il reste toutefois possible de modifier celui-ci au cours d'un programme.

### Conversions implicite

Certaines conversions sont dites implicites : elles sont faites **automatiquement** par l'ordinateur.

![Implicite conversion](../../ressources/basics/operations/implicit.png)

**Résultat :**

![Implicite conversion result](../../ressources/basics/operations/implicit_result.png)

### Conversions explicite

Bien que le JavaScript soit extrêmement tolérant avec les conversions de types, il arrive parfois qu'une conversion de soit pas possible.

>En cas d'échec de conversion d'un nombre, la valeur du résultat est `NaN` (Not A Number).

![NaN](../../ressources/basics//operations/nan.png)

Dans ce cas il va falloir **expliciter** la conversion. C'est à dire qu'il faudra dire au programme comment on souhaite convertir une donnée.

**Conversion vers une chaîne de caractères :**

Pour convertir explicitement une valeur en [une chaîne de caractères](./Les_chaines_de_characteres.md), il faut utiliser l'instruction `String(expression)` :

![NaN](../../ressources/basics//operations/string_convert.png)

**Conversion vers un nombre :**

Pour convertir explicitement une valeur en un nombre, il faut utiliser l'instruction `Number(expression)` :

![NaN](../../ressources/basics//operations/number_convert.png)
