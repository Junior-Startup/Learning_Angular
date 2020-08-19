# Créez votre premier projet

> Pour créer un nouveau projet Angular, naviguez vers le dossier souhaité depuis une ligne de commande et saisissez la commande suivante :

```
ng new mon-premier-projet
```

> Ensuite, naviguez dans le dossier du projet et lancez le serveur de développement :

```
cd mon-premier-projet
ng serve --open
```

> Si tout se passe bien, vous verrez les informations du serveur qui se lance à l'adresse ***localhost:4200*** et votre navigateur préféré se lancera automatiquement avec le message " ***Welcome to app !!*** " et le logo Angular.

> Félicitations, votre environnement de développement est prêt !

## Bootstrap

> Bootstrap est une bibliothèque css très connue . Pour l'integrer dans notre projet, on a besoin de la télécharger et l’installer sur le projet.

> Il faut faire distinction entre la bibliothèque css Bootstrap et le mot clé **bootstrap** utilisé dans Angular qui signifie Déclencher ou lancer (On va l’utiliser par la suite).

> Première étape: se positionner sur la racine du projet puis exécuter la commande suivante qui permet d’installer bootstrap dernière version :

```
npm install bootstrap
```
> Après l’installation avec succès de bootstrap, dans le dossier du projet. On a besoin d’informer Angular implicitement de l’existence de ce nouveau module. Pour ceci , il faut modifier le fichier de configuration **angular.json**.
Il suffit d’ajouter le path du fichier “**bootstrap.min.css**” au bloc style comme ça:

![bootstrap declaration](/assets/images/5.png)

## Quelques conseils pour le développement

> Je vous conseille d'utiliser Chrome comme navigateur par défaut pour le développement, car les Developer Tools sont très complets, et vous avez également la possibilité d'installer ***Augury***, un plugin Chrome spécifique pour le développement Angular.
