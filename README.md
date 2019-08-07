# 'SARA 2.0 Light' - Installationguide

### Releaseinformomation

+ Author: Projectgroup HTW 'Project Consulting'
+ Releasedate: 07/2019

### Purpose of the document

This document describes which software is necessary for the further development  of the software 'SARA 2.0 Light'.

### Tooldescription

SARA stands for "Structure Ability Rating Application" and can be used to for determining the maturity level in terms of readiness for industry 4.0.

### Necessary software

The software listed in tabular form must first be installed and executed by the user for execution.

|Softwarename|Downloadlink|Purpose|
|------------|:-----------|:-------------------------|
|Angular|https://angular.io/ |Visualize the frontend via localhost.|
|Visual Studio Code|https://code.visualstudio.com/download |Needed as IDE for developers. This IDE is a suggestion.|
|GraphQL (Playground)|http://saradev.azurewebsites.net/ |Needed for creating queries and mutations in GraphQL. A frontend is provided and can be used directly without installing any software.|

### Setup Angular and start coding

1. Download and install the latest NodeJS Version: https://nodejs.org/en/download/ <br>
   Version can be checked in terminal running command `node -v`
2. Open console and install Angular (optional but recommended) <br>
   `npm install Z-g @angular/cli`
3. Open project folder in code editor <br>
    - In VS Code: File > Open Folder > Sara <br>
    - In terminal: Navigate to /Sara, then run `code`.
4. Before the first start or when pulling a new version run the following in the terminal 
   > `npm install` <br>
   > `npm install` will pull all node_modules configured in the app. This only needs to be run when changes to the modules are made or the project is imported again.
   > Tip: When moving the project from a to b or when zipping etc., select all folders but leave out the "dist" and "node_modules" folder. The node_modules folder will be         recreated when *npm install* is executed. This will shorten the file size for transferring dramatically.
5. Start the application in console
   > *ng serve* (if angular was installed) or
   
   > *npm start* (if angular was not installed or *ng serve* did not work)
6. Start coding! Project will run in browser on: localhost:/4200

Refernce Link: https://angular.io/guide/setup-local

### Tips
1. When saving Angular will automatically recompile! 
   > Only changed files will recompile, so unchaged files are ignored which can cause unexpected behavior when testing in the browser
   > To avoid that, go to (in VS Code) File > Preferences > Keyboard Shortcuts and change the keybinding "strg s" to save all (from save), so all files will be changed and all    changes are recompiled.
2. VS Code is highly customizable! List of useful extensions:
   > 
3. Install packages with
   > npm install -s packageName (Search for packages: https://www.npmjs.com/)
4. Generate new components
   > ng generate component componentName or 
   > ng g c componentName
5. Generate new services
   > ng generate service serviceName or
   > ng g s serviceName
6. Example: Generate component inside the header-component-folder
   > Option a: navigate to folder (from /sara) "cd header", then run generate commandline
   > Option b: "ng g c header/componentName





### Useful Codesnippets

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

##### GraphQL

1. Query: #NAME#
```graphql
query FooQuery {
  field(call:$value) @directive(awesome:true, number:42, strings:"yes") {
    subfield as alias
  }
}
```
2. Query: #NAME#
```graphql
query FooQuery {
  field(call:$value) @directive(awesome:true, number:42, strings:"yes") {
    subfield as alias
  }
}
```

1. Mutation: #NAME#
```graphql
query FooQuery {
  field(call:$value) @directive(awesome:true, number:42, strings:"yes") {
    subfield as alias
  }
}
```
2. Mutation: #NAME#
```graphql
query FooQuery {
  field(call:$value) @directive(awesome:true, number:42, strings:"yes") {
    subfield as alias
  }
}
```

