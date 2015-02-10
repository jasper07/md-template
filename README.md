## Background
This repo is a copy of the md-template app from the OpenUI5 repository, put it here to make it easy to fork
https://github.com/SAP/openui5/tree/master/src/sap.m/test/sap/m/demokit/md-template

I really like this app because
- it has very useful easy to follow Qunit and Opa tests
- it show cases 'grunt-openui5' and Bower features available
- shows how to automate your Qunit and Opa tests and run them silently in PhantomJS
- shows how to integrate your app with the Continuous Integration platform Travis

more
- has a couple of nice reusable "Fiori" pattern examples, filterbar label (Master) and toggle buttons (LineItem)
- a good examples of how to use promises with models and lists

## To get started
ensure you have installed Node.js

```javascript
git clone https://github.com/jasper07/md-template.git
npm install
bower install
```
this will create a local copy of the repository, install all the necessary node packages and also install the OpenUI5 src

## To run the app
```javascript
grunt serve
```
this will setup a server which hosts the app, open up your browser and point it to
http://localhost:8080/index.html?responderOn=true#
this wil run the app using mock data for the OData service

## To run the Unit and Opa tests
http://localhost:8080/test-resources/unit/UnitTestsGrunt.qunit.html
http://localhost:8080/test-resources/opa/OpaTestsGrunt.qunit.html

## To run the Unit and Opa test via PhantomJS
use one of the following commands to run both, or run individual
```javascript
grunt test

grunt unitTest

grunt opaTest
```
## To integrate with Travis-CI
A CI tool makes working in a team easier with automated builds. These builds are triggered automatically when each developer checks in their code to the repository. The build process incorporates testing, if testing the build stops and team members will be notified.

#### how to, very quick only a couple of steps
http://code.tutsplus.com/tutorials/travis-ci-what-why-how--net-34771

the results
https://travis-ci.org/jasper07/md-template



