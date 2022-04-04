# js-karma-jasmine-coverage-examples

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.2.2 for showing difference between naive and proper Jest coverage configuration.

## Running unit tests

Run `npm run test-coverage-naive` to view "naive" configuration results. Note that coverage is 100% as our only `.spec` file tests everything it references. However there are files in the application that neither have associated `.spec` files nor are they referenced by any existing ones, which causes them not to be taken into account when calculating coverage. See: `karma.naive.conf.js` file.

Run `npm run test-coverage` to view "proper" configuration results. Here all files of interest are taken into the account. See: `karma.conf.js` file. You may want to extend this configuration however you need.
