# Concepts généraux d'Angular

## Introduction aux concepts d'Angular

* Angular est une plateforme et framework pour la création des applications Single-Page (Single Page Application) en utilisant HTML et TypeScript.
* Angular est écrit en TypeScript.
* L'architecture d'une application Angular se base sur 3 éléments fondamentaux :<br>
1. Modules
2. Components
3. Services et Injection de Dépendances

---

## Modules

* Les modules sont connus par _@NgModule()_
* Les _@NgModule_ sont les blocs de construction de base qui permettent la compilation des _Components_
* Une application Angular est définie par un ensemble de _@NgModule_
* Une application Angular a au moins un _root module_ qui assure le démarrage de l'app
* _@NgModules_ peuvent importer des fonctionnalités des autres _@NgModules_ comme ils peuvent exporter leurs fonctionnalités pour être utilisées par les autres _@NgModules_
* Cette organization assure la réutilisabilité du code et le _lazy loading_ càd n'utiliser un module qu'au besoin

---

## Components

* Les components sont connus par _@Component()_
* Les components définissent les _views_, qui sont un ensemble d'éléments d'écran qu'Angular peut choisir et modifier selon la logique et les données du programme
* Toute application Angular a au moins un component, _root component_, qui relie une hiérarchie de components avec le DOM de la page
* Chaque component définie une classe qui contient les données et la logique de l'application, et est associé avec une _template HTML_ qui définie le _view_ à être affiché

---

## Services et Injection de dépendances

* Les sevices sont connus par _@Injectable()_
* Les services sont utilisés par les components, ce qui permet d'offrir des fonctionnalités spécifiques qui ne sont pas directement liées aux _views_
* Les services peuvent être injectés dans les _components_ comme des _dependancies_, pour avoir un code modulaire et réutilisable
* Les services contiennent les données et la logique qui ne sont pas associés à un _view_ spécifique, et qui sont dédiés à être partagés entre les _components_
 
---

Plus :<br>
<i>https://angular.io/guide/architecture <br>
<i>https://angular.io/guide/architecture-moodules <br>
<i>https://angular.io/guide/architecture-components <br>
<i>https://angular.io/guide/architecture-services