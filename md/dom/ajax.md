# Ajax

JQuery offre la possibilité d'effectuer des requêtes HTTP très facilement par le biais de la fonction `.ajax()`.

## Instancier une requête HTTP

Instancier une requête HTTP devient extrêmement simple.Cela est rendu possible par la fonction `$.ajax()`. 

![instanciation.png](/ressources/dom/ajax/instanciation.png)

> Pas besoin d'utiliser le mot-clé `new` pour instancier l'objet.

## Les paramètres

La fonction `$.ajax()` accepte en paramètre un [objet](/md/basics/Les_objets.md) qui permet de définir les différents paramètres de notre requête comme la cible, le type de la requête ainsi que le type de données qu'on attend en retour.

### La cible

Pour spécifier la cible de notre requête HTTP, il faut utiliser le paramètre `url`.

![url.png](/ressources/dom/ajax/url.png)

### Type de la requête

Pour indiquer le type de requête que l'on souhaite envoyer, il faut utiliser le paramètre `type`.

![get.png](/ressources/dom/ajax/get.png)

> Pour les requêtes de type `GET`.

![post.png](/ressources/dom/ajax/post.png)

> Pour les requêtes de type `POST`.

### Données à envoyer

Pour envoyer des données via notre requête il faut utiliser le paramètre `data`.

![data.png](/ressources/dom/ajax/data.png)

### Le type de données à recevoir

Pour spécifier le type de données que l'on s'attend à recevoir, il faut utiliser le paramètre `dataType`.

![datatype.png](/ressources/dom/ajax/datatype.png)

## Traiter les retours de la fonction

Maintenant que notre requête est prête et paramétrée comme on le souhaite, il faut implémenter la gestion du retour pour interpréter ce que renvoie le serveur à la suite de l'envoi.

### Le paramètre `success`

Il existe un paramètre nommé `success`.
Ce paramètre attend une fonction et celle-ci ne sera exécutée **QUE** si l'appel AJAX a abouti.

![success.png](/ressources/dom/ajax/success.png)

> L'argument `data` correspond aux données renvoyées par le serveur.

> L'argument `statut` est une chaîne de caractère automatiquement générée par jQuery pour donner le statut de la requête.

### Le paramètre `error`

À l'inverse du paramètre `success`, il existe également un paramètre nommé `error` qui ne sera exécuté **QUE** si l'appel AJAX a échoué.

![error.png](/ressources/dom/ajax/error.png)

> L'argument `xhr` est l'objet [XHR](http://api.jquery.com/jQuery.ajax/#jqXHR) renvoyé par JQuery.

> L'argument `statut` est une chaîne de caractère automatiquement générée par jQuery pour donner le statut de la requête.

> L'argument `error` est une chaîne de caractère correspondant à l'erreur rencontrée.

### Le paramètre `complete`

Le paramètre `complete` quant à lui est exécuté une fois la requête terminée (après `success` ou `error`).

![error.png](/ressources/dom/ajax/error.png)

> L'argument `xhr` est l'objet [XHR](http://api.jquery.com/jQuery.ajax/#jqXHR) renvoyé par JQuery.

> L'argument `statut` est une chaîne de caractère automatiquement générée par jQuery pour donner le statut de la requête.

## Les formulaires

Un raccourci très sympathique peut être exploité lorsque vous gérez un appel AJAX de type POST impliquant l'utilisation d'un formulaire. Il s'agit de la **sérialisation**.

Prenons le formulaire suivant : 

![form.png](/ressources/dom/ajax/form.png)

On peut sérialiser les données renseignées avec la méthode `.serialize()`.

![serialize.png](/ressources/dom/ajax/serialize.png)

Grâce à la sérialisation, on obtient une chaîne de caractères de la forme : `'valeur1=' + valeur1 + '&valeur2=' + valeur2 + '&valeur3=' + valeur3`
