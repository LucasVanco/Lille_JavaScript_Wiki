# Les Classes

Les classes JavaScript ont été introduites avec **ECMAScript 2015 (ES6)**. Elle fournit uniquement une syntaxe plus simple pour créer des objets et manipuler l'héritage.

## Définir une classe

En réalité, les classes sont juste des [fonctions](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/functions/Les_fonctions.md) spéciales. Ainsi, les classes sont définies de la même façon que les fonctions : par déclaration, ou par expression.

### Déclarations de classe

Pour utiliser une déclaration de classe simple, on utilisera le mot-clé class, suivi par le nom de la classe que l'on déclare.

![class declaration](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/declaration.png)

### Expressions de classe

Il est possible d'utiliser des expressions de classes pour définir des classes.

![class expression](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/expression.png)

## Corps d'une classe

Le corps d'une classe est la partie contenue entre les accolades `{...}`. C'est dans cette partie que l'on définit les propriétés d'une classe comme ses méthodes et son constructeur.

### Constructeur

La méthode `constructor` est une méthode spéciale qui permet de créer et d'initialiser les objets créés avec une classe.

> Il ne peut y avoir qu'une seule méthode avec le nom `constructor` pour une classe donnée.

![constructor](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/constructor.png)

### Méthodes

La définition d'une méthode se fait directement dans le corps de la classe. Pour définir une méthode il suffit de préciser son nom et ses arguments entre les parenthèses.

![methode declaration](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/methode.png)

#### Le mot-clé `this`

Le mot-clé this est défini automatiquement par JavaScript à l'intérieur d'une méthode et représente l'objet sur lequel la méthode a été appelée.

#### Le mot-clé `static`

Le mot-clé `static` permet de définir une méthode statique pour une classe. Les méthodes statiques sont appelées par rapport à la classe entière et non par rapport à une instance donnée.

> Les méthodes `static` ne peuvent pas être appelées « depuis » une instance de l'objet.

![methode static](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/static.png)

#### Le mot-clé `get`

La syntaxe `get` permet de lier une propriété d'un objet à une fonction qui sera appelée lorsqu'on accédera à la propriété.

![get syntaxe](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/get.png)

#### Le mot-clé `set`

La syntaxe `set` permet de lier une propriété d'un objet à une fonction qui sera appelée à chaque tentative de modification de cette propriété.

![set syntaxe](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/set.png)

## L'héritage de classe

Avec l'introduction des classes en ES6, l'héritage de classe est donc possible. Pour hériter d'une classe on utilisera le mot-clé `extends`.

![extends](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/extends.png)

> Dans le cas où le constructeur de la classe fille est identique à celui de la classe parente, et uniquement dans ce cas, alors il n'est pas nécessaire de le spécifier dans la classe fille.

![same construct](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/same_constructor.png)

### Le mot-clé `super`

Le mot-clé super est utilisé afin d'appeler ou d'accéder à des fonctions définies sur l'objet parent.

> Il est possible d'utiliser super pour invoquer des méthodes statiques.

![super](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/super.png)

### Surcharge de méthode

Lorsque qu'une classe fille redéfinit une méthode de sa classe parente, on dit qu'elle **surcharge** la méthode.

![override](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/class/override.png)

