# Angular Commands Memento

> ### Installing Angular CLI :
```
npm install -g @angular/cli
```
> ### Create new project (this will create the project workspace too):
```
ng new my-project-name
```
> ### Run the application :

>> * First navigate to the application folder
```
cd my-project-name
```
>> * run the command : 
* * *
Default port is 4200
```
ng serve
```
***
We can specify the port to listen on using --port 
```
ng serve --port < port-number >
```
***
To automatically open the url in the default browser we use --open or -o

```
ng serve --open
```

### Generate new component :
```
ng generate component < component-name >
```
```
ng g c < component-name >
```

### Generate new service :
```
ng generate service < service-name >
```
```
ng g s < service-name >
```

### Generate new pipe :

```
ng generate pipe < pipe-name >
```

```
ng g p < pipe-name >
```