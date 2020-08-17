# Présentation

Angular est tout un Framework JavaScript Open Source. Angular est apparu, la première fois en 2009. Il est créé par Misko Hevery et Adam Abrons.

Maintenant il est totalement avalé et supporté par Google. Donc on parle d’un produit Google.<br>
> La meilleure partie à ce sujet est le support à long terme de Google (LTS). Cela met en lumière le plan de Google de le respecter et de développer davantage l'écosystème angulaire.

Il y a toute une rupture entre AngularJS et Angular2.0 et les versions qui suivent. En fait, google a annoncé que l’idée est de créer tout un framework basé sur Javascript et non pas une simple bibliothèque ( Comme JQuery) qui permet d'exploiter la puissance de JavaScript et qui assure une expérience utilisateur très riche et fluide à la fois.

# Différence entre Angular et AngularJS

> Angular et AngularJs sont deux frameworks différents qui ont +- le même nom, et ça peut créer un conflit.

> La première Version (AngularJS ) est assez proche du patron de conception MVC, mais coté JavaScript. Donc nous sommes appelés à créer des contrôleurs et des vues JavaScript.

> Par contre dans Angular 2, il fallait créer des composants.

> Ces composants sont totalements indépendants et peuvent être utilisés plusieurs fois dans l’application et même dans d’autres applications.

> Angular 2 est orienté mobile aussi. Donc vous pouvez créer des applications avec Angular 2 et l’utiliser sur votre Iphone ou Samsung Mobile.

> Généralement Angular 2 utiliser TypeScript et AngularJs utilise JavaScript.<br>Le TypeScript est une couche supérieur au Javascript développé par Microsoft qui se compile en JavaScript simple. Etant un language typé, il permet de créer des classes, des variables, des signatures de fonction et l'utilisation de modules. Il est important de noter que l'utilisation du TypeScript est facultative, on peut tout à fait utiliser du JavaScript dans un fichier TypeScript.

> Angular 2 est plus performant que AngularJS.

> Angular 2 est plus testable que AngularJS.

> Angular 2 a tué beaucoup des notions des AngularJS comme: Contrôleurs, $Scope, ng-repeat, les directives (qui sont remplacées par les composants).

> Le changement le plus important pour moi c’est l’utilisation des composants qui servent pour créer des applications modernes. Les composants peuvent êtres aussi utilisables plusieurs fois dans la même application. Aussi on peut utiliser le même composant dans plusieurs applications séparées.

> Dans Angular 2 et les versions suivantes, tout est basé sur la notion de components. Donc tout est basé sur l’encapsulation et la communication inter-components.

> Dans Angular 2 et surtout à partir de la version 4 d’angular on utilise des nouvelles notions d’ECMAScript ES6 tels que les classes, les modules, Lambda Expression, les ternaires, les décorateurs ...

<br> 

# Pourquoi Angular ?

Contrairement à d'autres alternatives intéressantes telles que React, Angular n'est pas une "library" mais bien un framework avec une approche "batteries included".
Angular fournit donc nativement tout le nécessaire pour produire une application entière avec une configuration standard :
- Configuration de build et d'optimisation complète.
- Module d'animations.
- Module de "routing".
- Module de formulaires.
- Debug.
- Tests unitaires et e2e.
- ...<br>

Il n'est donc pas nécessaire d'hésiter et de débattre le choix des modules de routing, de formulaires etc...
Avec Angular, la majorité des applications ont la même structure de projet et la même "stack" d'outils.
**Les applications Angular sont donc homogènes** et vous tomberez donc plus rarement sur des "cas particuliers".<br>

Dans la plupart des cas, vous éviterez les problèmes de compatibilité de dépendances en laissant l'équipe Angular s'en charger pour vous.

<br>

# Avantages 

>Un framework complet avec une architecture élégante.

>Une documentation très étoffée qui permet aux développeurs de trouver toutes les informations nécessaires rapidement.

>Une grande communauté, qui permet toujours de pouvoir poser des questions en cas de blocage.

>Des améliorations constantes et régulières (compilation inférieure à 3 secondes pour Angular 5).

>L’association bidirectionnelle de données, qui répercute les effets de chaque modification mineure des données, supprime le besoin de synchronisation supplémentaire des données de la vue et du modèle, et minimise les risques d’erreurs.

>Modèle MVVM (Model – View- View Model), qui permet aux développeurs de travailler séparément sur la même section d’application en utilisant le même ensemble de données.

>Un moteur de DI ( injection de dépendances ).

>Les avantages du TypeScript : vérification statique et opérationnelle de la saisie, fonctions de saisie très performantes.  

<br> 

# Architecture d'Angular

Angular est aujourd'hui basé sur une architecture de composants complètement indépendants les uns des autres. Une fois le composant principal chargé, il analyse ensuite la vue html correspondant à celui-ci et détecte si il comporte des composants imbriqués. Si c'est le cas, Angular va trouver toutes les correspondances et exécuter le code lié a celles-ci. On peut imbriquer autant de composants que l'on souhaite.

Un composant dans Angular sert à générer une partie de code html et fournir des fonctionnalités à celle-ci. C'est pour cela qu'un composant est constitué d'une classe dans laquelle on pourra définir la logique d'application pour ce composant avec des propriétés, des méthodes...etc.

<br> 

![Architecture d'Angular](/assets/images/1.png)

