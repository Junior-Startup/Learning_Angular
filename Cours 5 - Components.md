# Components

Les components sont les composantes de base d'une application Angular : une application est une arborescence de plusieurs components.

Imaginez la page web suivante :

![bootstrap](/assets/images/3.png)

> Tout d'abord, notre  **AppComponent**  est notre component principal : tous les autres components de notre application seront emboîtés ou "nested" dans celui-ci.

> Pour cette structure, on peut imaginer un component pour la barre de menu, un autre pour la partie contenu et un dernier pour le menu à droite.

<br>

## Découvrez la structure du code

Pour commencer à comprendre la structure d'une application Angular, ouvrez  **index.html**  dans votre éditeur :

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>MonProjetAngular</title>
    <base href="/">
    
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="icon" type="image/x-icon" href="favicon.ico">
</head>
<body>
    <app-root></app-root>
</body>
</html>
```

Comme vous pouvez le constater, au lieu d'y voir tout le contenu que nous voyons dans le navigateur, il n'y a que cette balise vide ```<app-root>``` : il s'agit d'une balise Angular. Pour en savoir plus, ouvrez le dossier  app  : 

![appcomponent files](/assets/images/4.png)



Ce dossier contient le module principal de l'application et les trois fichiers du component principal  **AppComponent**  : son template en HTML, sa feuille de styles en CSS, et son fichier TypeScript, qui contiendra sa logique. 

Regardez maintenant dans le fichier  **app.component.ts**  :

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'app';
}
```
Ici, à l'intérieur du décorateur  **@Component()**  , vous trouvez un objet qui contient les éléments suivants :

- **selector**  : il s'agit du nom qu'on utilisera comme balise HTML pour afficher ce component, comme vous l'avez vu avec  ```<app-root>```  . Ce nom doit être unique et ne doit pas être un nom réservé HTML de type  ```<div>```  ,  ```<body>```  etc. On utilisera donc très souvent un préfixe comme app par exemple ;

- **templateUrl**  : le chemin vers le code HTML à injecter ;

- **styleUrls**  : un array contenant un ou plusieurs chemins vers les feuilles de styles qui concernent ce component ;

Quand Angular rencontre la balise  <app-root>  dans le document HTML, il sait qu'il doit en remplacer le contenu par celui du template  **app.component.html** , en appliquant les styles  **app.component.css** , le tout géré par la logique du fichier  **app.component.ts** .

<br>

# Créer notre premier component

Précédemment on a travaillé sur le component principal qui s’appelle **Appcomponent**. Généralement, on n’ajoute pas des components dans la page **index.html** mais on les attaches au composant principal “AppComponent”.

Supposons que je veuille créer un composant **MonPremierComponent**.

> J’ouvre un terminal, je me place à la racine du projet, et je tape la commande :
```
ng generate component mon-premier 
```

Ou la syntaxe raccourcie équivalente :
```
ng g c mon-premier 
```
> Dans le répertoire src/app du projet, le CLI va créer un répertoire **mon-premier** qui contient 4 fichiers correspondant au composant :

```
/mon-premier 
  mon-premier.component.ts       # Classe du composant
  mon-premier.component.html     # Template du composant
  mon-premier.component.css      # Styles CSS du composant
  mon-premier.component.spec.ts  # Tests unitaires du composant
  ```

> Par ailleurs, le CLI ajoute la classe du composant créé dans les declarations du module principal :

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppComponent } from './app.component';
import { MonPremierComponent } from './mon-premier/mon-premier.component';

@NgModule({
  declarations: [
    AppComponent,
    MonPremierComponent
  ],
  imports: [
    BrowserModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

> Le CLI a ajouté  **MonPremierComponent**  à l'array  declarations  de votre module.  Il a également ajouté le statement import en haut du fichier.  Ce sont des étapes nécessaires pour que vous puissiez utiliser votre component au sein de votre application Angular.

Regardez maintenant le fichier  **mon-premier.component.ts**  :

```ts
import { Component, OnInit } from '@angular/core';

@Component({
  selector: 'app-mon-premier',
  templateUrl: './mon-premier.component.html',
  styleUrls: ['./mon-premier.component.css']
})
export class MonPremierComponent implements OnInit {

  constructor() { }

  ngOnInit() {
  }
  
}
```
Vous constaterez que le CLI a créé un sélecteur :  **app-mon-premier** . Nous pouvons donc utiliser ce sélecteur dans notre code pour y insérer ce component.

> Félicitations, vous avez créé votre premier component Angular !

