# Modernizr SVG Transforms
Modernizr test to determine if the browser supports transforms within inline SVGs. Most modern browsers support css transforms as well as inline SVGs, however some either don't support transforms on SVGs entirely (I'm looking at you IE9-11) or give false-positives (Firefox).

Example problem:
Our mobile nav 'hamburger' icon uses svg transforms to change from the traditional 3 lines to a X, however when this was applied for the desktop nav, the animations weren't behaving correctly.

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 
There are 3 main files within the package.

- __index.js__: Imports the index-babel file for requiring within node / browserify.
- __index-babel.js__ - ES6 version of the test.
- __index-compiled.js__ - Babel compiled version for standalone use

### Prerequisites

####Modernizr
This package uses the Modernizr.addTest method which was intruduced in version 3 of modernizr.

```
npm install modernizr --save
```

####NodeJS / NPM
If you're installing the npm package you will obviously need to have Node & npm installed.

### Installing

If using within node / browserify, run the following from your projects' root folder to install and save as a dependency in your package.json

```
npm install modernizr-svg-transforms --save
```

If using directly in the browser, simply clone the repo (or download), and include index-compiled.js after Modernizr.

## Running the tests

This package uses eslint for code linting tests.

``` 
npm run test
```

## Contributing

Please read [CONTRIBUTING.md](https://github.com/wildpixeldesign/modernizr-svg-transforms/blob/master/CONTRIBUTING.md) for details on the process for submitting pull requests.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/wildpixeldesign/modernizr-svg-transforms/tags).

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
