# Les conditions

Les conditions permettent d'effectuer des tests sur le code et ainsi produire des actions en fonction de ces conditions.

**Une condition** est une expression dont l'évaluation produit une valeur soit vraie, soit fausse : on parle de valeur [booléenne](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/variables/Les_Variables.md#les-diff%C3%A9rents-type-de-donn%C3%A9es).

## L'instruction if

L'instruction `if` permet de tester une expression, elle est la principale instruction utilisée pour les conditions.

![if condition](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/if.png)

La syntaxe d'une instruction `if` est la suivante : 

![if syntaxe](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/if_syntaxe.png)

Lorsque la `condition` est vraie alors le *bloc de code* à l'intérieur des accolades est exécuté.

> Quand la condition est vraie, on dit que cette condition est **vérifiée**.

Une condition n'a que deux résultats possibles : soit vrai (`true`) soit faux (`false`). Si et seulement si la condition est vérifiée alors l'expression de code entre les accolades est exécuté.

## Ajouter une alternative

Pour exprimer une alternative à l'instruction `if`, on utilise l'instruction `if ... else`.

> Le bloc de code dans le `else` s'exécute lorsque la condition `if` est évalué à `false`

![else](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/if_else.png)

Il est également possible de combiner l'instruction `if` et l'instruction `else` pour exprimer un choix logique. On obtient alors l'instruction `else if` pour exprimer une alternative spécifique.

![else if](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/if_elseif.png)

## Imbriquer les conditions

Il est tout à fait possible d'imbriquer les conditions pour écrire des programmes plus complexes.

![multiple if](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/if_imbrique.png)

## Les opérateurs de comparaison

Les différents opérateurs logiques qui permettent de tester deux valeurs sont les suivants : 

Opérateur | Description
--- | ---
== | Égalité. Renvoie true si les opérandes sont égaux
=== | Égalité stricte. Renvoie true si les opérandes sont égaux et de même type
!= | Inégalité. Renvoie true si les opérandes sont différents.
!== | Inégalité stricte. Renvoie true si les opérandes ne sont pas égaux ou s'ils ne sont pas de même type.
| > | Supériorité Stricte. Renvoie true si l'opérande gauche est supérieur (strictement) à l'opérande droit
| >= | Supériorité ou égalité. Renvoie true si l'opérande gauche est supérieur ou égal à l'opérande droit.
| < | Infériorité Stricte. Renvoie true si l'opérande gauche est inférieur (strictement) à l'opérande droit
| <= | Infériorité ou égalité. Renvoie true si l'opérande gauche est inférieur ou égal à l'opérande droit.

**Exemple**

![operator](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/operator.png)

> `'1' == 1` retourne `true` car, bien qu'il soit de type différent (`string` et `number`), l'ordinateur considère qu'ils sont tous deux égaux.

## Les conditions composées

### L'opérateur logique ET `&&`

L'opérateur logique `&&` permet de combiner des conditions et d'exécuter un bloc de code si **toute les conditions sont vraies**.

![and](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/et_condition.png)

La syntaxe est la suivante :

![and syntaxe](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/et_condition_syntaxe.png)

> Les parenthèses autour des sous conditions ne sont pas obligatoire mais **très fortement conseillées**.

### L'opérateur logique OU `||`

L'opérateur logique `||` permet de combiner des conditions et d'exécuter un bloc de code si **au moins une des conditions est vraie**.

![or](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/ou_condition.png)

La syntaxe est la suivante :

![or syntaxe](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/ou_condition_syntaxe.png)

> Les parenthèses autour des sous conditions ne sont pas obligatoire mais **très fortement conseillées**.

### L'opérateur de négation `!`

L'opérateur logique `!` permet d'inverser la valeur d'une condition.

![inverse](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/inverse.png)

Ainsi :

![inverse log](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/conditions/inverse_log.png)


