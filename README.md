# npmdoc-change-case

#### basic api documentation for  [change-case (v3.0.1)](https://github.com/blakeembrey/change-case#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-change-case.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-change-case) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-change-case.svg)](https://travis-ci.org/npmdoc/node-npmdoc-change-case)

#### Convert a string between camelCase, PascalCase, Title Case, snake_case and more.

[![NPM](https://nodei.co/npm/change-case.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/change-case)

- [https://npmdoc.github.io/node-npmdoc-change-case/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-change-case/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-change-case/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-change-case/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-change-case/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-change-case/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Blake Embrey",
        "url": "http://blakeembrey.me"
    },
    "bugs": {
        "url": "https://github.com/blakeembrey/change-case/issues"
    },
    "dependencies": {
        "camel-case": "^3.0.0",
        "constant-case": "^2.0.0",
        "dot-case": "^2.1.0",
        "header-case": "^1.0.0",
        "is-lower-case": "^1.1.0",
        "is-upper-case": "^1.1.0",
        "lower-case": "^1.1.1",
        "lower-case-first": "^1.0.0",
        "no-case": "^2.2.0",
        "param-case": "^2.1.0",
        "pascal-case": "^2.0.0",
        "path-case": "^2.1.0",
        "sentence-case": "^2.1.0",
        "snake-case": "^2.1.0",
        "swap-case": "^1.1.0",
        "title-case": "^2.1.0",
        "upper-case": "^1.1.1",
        "upper-case-first": "^1.1.0"
    },
    "description": "Convert a string between camelCase, PascalCase, Title Case, snake_case and more.",
    "devDependencies": {
        "istanbul": "^0.4.3",
        "mocha": "^3.0.0",
        "standard": "^8.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "ee5f5ad0415ad1ad9e8072cf49cd4cfa7660a554",
        "tarball": "https://registry.npmjs.org/change-case/-/change-case-3.0.1.tgz"
    },
    "files": [
        "change-case.js",
        "change-case.d.ts",
        "LICENSE"
    ],
    "gitHead": "428974c49af64a9065b446a4798978521d7ddadd",
    "homepage": "https://github.com/blakeembrey/change-case#readme",
    "keywords": [
        "camel",
        "pascal",
        "title",
        "case",
        "lower",
        "upper",
        "param",
        "dot",
        "path",
        "constant",
        "cases",
        "check"
    ],
    "license": "MIT",
    "main": "change-case.js",
    "maintainers": [
        {
            "name": "blakeembrey"
        }
    ],
    "name": "change-case",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/blakeembrey/change-case.git"
    },
    "scripts": {
        "lint": "standard",
        "test": "npm run lint && npm run test-cov",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- -R spec --bail",
        "test-std": "mocha -- -R spec --bail"
    },
    "typings": "change-case.d.ts",
    "version": "3.0.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
