# Angular 2 Notes

### Essential parts of Angular 2

##### Angular 2 Modules

- In ng2 we separate our code into modules separate features, assemble the application from module then we expose by exporting it.
- changed from ng1 because ES6 has it own implementation
- Import using the import keyword, it is using destructuring

##### Angular 2 Components, one of the most important players of ng2
- Component contains application logic that controls a region of the user interface that we call a view.
- It provides, reuse and consistency.
- Nest components inside other components, kind like extjs.
- Need start component main.ts  which contains a bootstrap of the main components
- Entry point for the app

##### Angular 2 templates

- Directive
- Interpolation {{}}
- Nested components <vehicle> </vehicle>
- basic html
- component -> template by connecting it
- Either inline or by url.
- Create component tree
- Nesting components

##### Angular 2 metadata
- Declare all directives as child components.
- selector used ex: app   <app></app>
- styleUrls - can have multiple
- templateUrl - only one
- directives - other components
- providers - services used
- @Component decorator
- Input and Output a great way for child components to communicate with parent components

#### Parent to Child Communication
- ViewChild to grad child component and call its methods.
- Used in a filter scenario to call clear and clear the results

#### Interpolation
- One way in
- {{vehicle.name}}

#### Property Binding
- One way in
- take property and [] send values to components
- ex: character name
- interpolation is a short way to property Binding
- [target]="expression"
- always one way unidirectional

#### Event Binding
- How we comunicate from the template to the Component
- (event)="clickHandler"
- ex: (click)="save()">Save</button>
- ex: (changed)="vehicleChanged()"
```
(click)="select('asdf')"
```

#### Two way Binding
- [()] banana in a box syntax
- [(ngModel)]="expression"
- [(ngModel)]="character.name

#### Built-in Directives
- Transform the DOM
- Camel case
- [ngStyle]="setStyle()"
- [ngClass]
- *ngFor, *ngIf, *ngSwith
- ex: *ngIf="currentVehicle"
- ex: *ngFor="#story of stories"> {{story.name}}

####

#### End of Course objective
- Do basic component comunication and app
- 4-30