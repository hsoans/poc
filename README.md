# ARKeth Angular 6 + Angular CLI + Angular Material + Docker + Unit Testing+ Angular Library

> ### Base project. Contains CRUD, patterns, generated library, etc.

## ARketh Getting started

**Warning**

> Verify that you are running at least node 8.9.x and npm 5.x.x by running node -v and npm -v in a terminal/console window. Older versions produce errors, but newer versions are fine.

1. Go to project folder and install dependencies.
 ```bash
 npm install
 ```

2. Launch development server:
 ```bash
 npm start
 ```

**Note**

> You don't need to build the library because it's published in npm and added as dependency of the project.

## Usage

Tasks                    | Description
-------------------------|---------------------------------------------------------------------------------------
npm i                    | Install dependencies
npm start                | Start the app in development mode
npm run test             | Run unit tests with karma and jasmine
npm run e2e              | Run end to end tests with protractor
npm run build            | Build the app for production
npm run build:library    | Build the library
npm run lint             | Run the linter (tslint)
npm run ci               | Execute linter and tests
npm run extract          | Generate all json files with the translations in assets folder
npm run deploy           | Build the app and deploy dist folder to Github pages (angular-cli-ghpages) (fork to do this and remove CNAME file)
npm run bundle-report    | Build and run webpack-bundle-analyzer over stats json, really cool :)
npm run release          | Create a new release using standard-version
npm run docker           | Build the docker image and run the container
npm run update           | Update the project dependencies with ng update

## Features

* CRUD: create, update and remove heroes
* Search bar, to look for heroes
* Custom loading page
* Angular Pipes
* Interceptors and Events (Progress bar active, if a request is pending)
* Modal and toasts (snakbar)!
* Responsive layout (flex layout module)
* SASS (most common used functions and mixins) and BEM styles
* Internationalization with ng-translate and ngx-translate-extract. Also use cache busting for translation files with [webpack translate loader](https://github.com/ngx-translate/http-loader#angular-cliwebpack-translateloader-example)
* Lazy loading modules
* Service Workers
* Dynamic Imports
* More logical structure directory (from [here](https://itnext.io/choosing-a-highly-scalable-folder-structure-in-angular-d987de65ec7))
* Basic example library
* Scroll restoration and anchor examples
* Modernizr (browser features detection)
* Safari polyfill for date inputs (date-input-polyfill)
* Google Tag Manager
* Github pages deploy ready
* Unit tests with Jasmine and Karma including code coverage
* End-to-end tests with Protractor
* ES6 Promises and Observables
* Following the [best practices](https://angular.io/guide/styleguide)!

## Docker

You can build the image and run the container with Docker. The configuration is in the nginx folder if you want to change it.

`docker build -t angularexampleapp .`

`docker run -d -p 4200:80 angularexampleapp`

## Travis CI

We use Travis CI to run this tasks in order:
* Linter
* Tests
* Build for production
* Deploy in Github pages

## Contributing

- Please see the CONTRIBUTING file for guidelines.
- Create **pull requests, submit bugs, suggest new features** or documentation updates :wrench:

## Server

This repo is using [a minimal app](https://github.com/Ismaestro/nodejs-example-app) in NodeJS deployed on Heroku and using PostGreSQL, to create, modify and delete heroes.

## License


