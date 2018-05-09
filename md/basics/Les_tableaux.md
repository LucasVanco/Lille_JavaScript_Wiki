# Les tableaux

**Un tableau** est [un type de donnée](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/variables/Les_Variables.md#les-diff%C3%A9rents-type-de-donn%C3%A9es) qui permet de stocker un ensemble d'éléments.

## Créer un tableau 

Pour créer un tableau, on le déclare en utilisant une paire de crochets `[]`. Les différents éléments du tableau sont séparés par des virgules `,`.

![Tab declaration](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/tabs/tab.png)

En JavaScript il est possible de déclarer un tableau contenant plusieurs types de données (`String`, `Number`, `Boolean`, `Object` ou encore d'autres `Tableaux`).

![Tab multiple types](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/tabs/tab_multiple.png)

> Un tableau possédant plusieurs données, on les nommera toujours avec des noms exprimant le pluriel


## Obtenir la taille d'un tableau

Comme pour [les chaîne de caractères](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/strings/Les_chaines_de_characteres.md), pour obtenir la taille d'un tableau on utilisera [la propriété](https://github.com/TresorDeKelloggS/Lille_JavaScript_Wiki/blob/master/md/objects/Les_objets.md#propri%C3%A9t%C3%A9s) `length` de celui-ci.

![Tab length](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/tabs/tab_length.png)

> `length` renvoie `0` dans le cas d'un tableau vide (sans élément).

## Accéder à un élément d'un tableau

Chaque élément présent dans un tableau est identifié par un numéro, appelé son `index`.

On peut représenter graphiquement un tableau comme un ensemble de cases, chacune stockant une valeur spécifique et associée à un indice.

> Le premier élément du tableau a pour index `0`

L'accès à un élément s'effectue en plaçant cet indice entre crochets : `myTab[index]`.

![Tab length](https://raw.githubusercontent.com/TresorDeKelloggS/Lille_JavaScript_Wiki/master/ressources/tabs/tab_access.png)

> Les tableaux et les chaînes de caractères sont semblables sur certains points, notamment par rapport aux index.