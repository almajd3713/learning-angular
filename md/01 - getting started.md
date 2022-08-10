
Ight so this will be a long one
This is the file structure of a --minimal angular project
```html
playground
-- .vscode
-- src
---- app <!-- components storage -->
------ app.component.ts <!-- import your html/css/scripts here -->
------ app.module.ts <!-- have no idea -->
---- assets 
---- environments <!-- contains files to config environment type -->
---- main.ts <!-- runs the App component, like `index.js` in react -->
---- polyfills.ts 
---- styles.scss <!-- global styles -->
-- .browserlistrc <!-- adjusts css/js for browsers listed -->
```

`ng g c NAME` creates a new componetn and imports it to your `app.module.ts`
```ts
@Component({
  selector: 'Server', // change this to the tag you wanna use
  templateUrl: "server.component.html", // the html file
  styles: [ // css files
  ]
})
```

adding components is in multiple ways:
```ts
@Component({
  selector: "Server"
})
```
<Server></Server>

<!-- or -->
```ts
@Component({
  selector: "[Server]"
})
```
<div Server></div>

<!-- or -->
```ts
@Component({
  selector: ".Server"
})
```
<div class="Server"></div>