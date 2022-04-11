Example repo for the [Testing - Coverage sub-chapter of the Angular handbook](https://infinum.com/handbook/frontend/angular/angular-guidelines-and-best-practices/testing#coverage).

## Running unit tests

Run `npm run test-coverage-naive` to view "naive" configuration results. Note that coverage is 100% as our only `.spec` file tests everything it references. However there are files in the application that neither have associated `.spec` files nor are they referenced by any existing ones, which causes them not to be taken into account when calculating coverage. See: `karma.naive.conf.js` file.

Run `npm run test-coverage` to view "proper" configuration results. Here all files of interest are taken into the account. See: `karma.conf.js` file. You may want to extend this configuration however you need.
