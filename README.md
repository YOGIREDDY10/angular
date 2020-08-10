# angular

# Angular CLI
+ NOTE: this documentation is for Angular CLI 6. For Angular CLI Version 7 and later go here and 1.x go here instead.

# Overview
+ The Angular CLI is a tool to initialize, develop, scaffold and maintain Angular applications

# Getting Started
+ To install the Angular CLI:

+ npm install -g @angular/cli
+ If you get an error installing the CLI, this is an issue with your local npm setup on your machine, not a problem in Angular CLI. 
+ Please have a look at the fixing npm permissions page, common errors page, npm issue tracker, or open a new issue if the problem you are experiencing isn't known. 
+ To install a different version, see below.

### Generating and serving an Angular project via a development server Create and run a new project:

 + ng new my-project
 + cd my-project
 + ng serve
+ Navigate to http://localhost:4200/. The app will automatically reload if you change any of the source files.

## Bundling
+ All builds make use of bundling, and using the --prod flag in ng build --prod or ng serve --prod will also make use of uglifying and tree-shaking functionality.

# Running unit tests
+ ng test
+ Tests will execute after a build is executed via Karma, and it will automatically watch your files for changes. 
+ You can run tests a single time via --watch=false or --single-run.

## Running end-to-end tests
+ ng e2e
+ Before running the tests make sure you are serving the app via ng serve. End-to-end tests are run via Protractor.

# Additional Commands
+ ng new
+ ng serve
+ ng generate
+ ng lint
+ ng test
+ ng e2e
+ ng build
+ ng get/ng set
+ ng doc
+ ng xi18n
+ ng update
## Angular CLI Workspace Schema
+ Angular CLI workspace file (angular.json) schema
## Additional Information
+ There are several stories which will walk you through setting up additional aspects of Angular applications.

## Installing a specific version
+ The CLI is installed both globally (the command above with the -g argument to npm install) and also within the project. 
+ To install a different version of the CLI, you can just update the version locally within your project. 
+ The globally installed package will always delegate to the local one.

### There are several different versions available at any time:

+ Install a previous version, maybe because of a bug in the latest version. 
+ For example to get 6.0.2: npm install @angular/cli@6.0.2
+ Install the pre-release of a newer minor/major version, to try new features. 
+ For example to get 7.0.0-beta.3: npm install @angular/cli@next. Note that the @next version is only useful during beta periods.
+ Install a snapshot build from the latest passing run of our CI (angular-cli/master). 
+ This is useful if an issue was just fixed or a new feature just landed on master, but is not yet released: npm install @angular/cli@github:angular/cli-builds (or maybe better, find the particular SHA that you want to try: npm install @angular/cli@github:angular/cli-builds#0123456789abcdef)
