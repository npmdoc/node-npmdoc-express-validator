# npmdoc-express-validator

#### api documentation for  [express-validator (v3.1.3)](https://github.com/ctavan/express-validator)  [![npm package](https://img.shields.io/npm/v/npmdoc-express-validator.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-express-validator) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-validator.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-validator)

#### Express middleware for the validator module.

[![NPM](https://nodei.co/npm/express-validator.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/express-validator)

- [https://npmdoc.github.io/node-npmdoc-express-validator/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-express-validator/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-validator/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-validator/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-express-validator/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-express-validator/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christoph Tavan"
    },
    "bugs": {
        "url": "https://github.com/ctavan/express-validator/issues"
    },
    "contributors": [
        {
            "name": "Chris O'Hara"
        },
        {
            "name": "@orfaust"
        },
        {
            "name": "@zero21xxx"
        },
        {
            "name": "Roman Kalyakin"
        },
        {
            "name": "Rusty Bailey"
        },
        {
            "name": "Gustavo Henke"
        },
        {
            "name": "Ayman Nedjmeddine"
        }
    ],
    "dependencies": {
        "@types/bluebird": "~3.0.36",
        "@types/express": "~4.0.34",
        "bluebird": "^3.4.0",
        "lodash": "^4.16.0",
        "validator": "~6.2.0"
    },
    "description": "Express middleware for the validator module.",
    "devDependencies": {
        "body-parser": "1.12.3",
        "chai": "2.3.0",
        "cookie-parser": "1.4.1",
        "coveralls": "2.11.14",
        "eslint": "^3.13.1",
        "express": "4.12.3",
        "mocha": "2.2.4",
        "nyc": "8.4.0",
        "supertest": "0.15.0",
        "typescript": "~2.0.10"
    },
    "directories": {},
    "dist": {
        "shasum": "5670a37921340c1e529c7b6fabc3551ee1dbcf6d",
        "tarball": "https://registry.npmjs.org/express-validator/-/express-validator-3.1.3.tgz"
    },
    "engines": {
        "node": ">= 0.10"
    },
    "gitHead": "b983e4f31b7d6ccccf53b1349329c9f93c84f5b0",
    "homepage": "https://github.com/ctavan/express-validator",
    "keywords": [
        "express",
        "validator",
        "validation",
        "validate",
        "sanitize",
        "sanitization",
        "xss"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "ctavan"
        },
        {
            "name": "gustavohenke"
        },
        {
            "name": "rustybailey"
        }
    ],
    "name": "express-validator",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/ctavan/express-validator.git"
    },
    "scripts": {
        "lint": "eslint lib test",
        "report-coverage": "cat coverage/lcov.info | coveralls",
        "test": "nyc mocha && tsc",
        "travis-build": "npm test && npm run lint"
    },
    "types": "./index.d.ts",
    "version": "3.1.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
