# api documentation for  [change-case (v3.0.1)](https://github.com/blakeembrey/change-case#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-change-case.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-change-case) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-change-case.svg)](https://travis-ci.org/npmdoc/node-npmdoc-change-case)
#### Convert a string between camelCase, PascalCase, Title Case, snake_case and more.

[![NPM](https://nodei.co/npm/change-case.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/change-case)

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
    "version": "3.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module change-case](#apidoc.module.change-case)
1.  [function <span class="apidocSignatureSpan">change-case.</span>camel (value, locale, mergeNumbers)](#apidoc.element.change-case.camel)
1.  [function <span class="apidocSignatureSpan">change-case.</span>camelCase (value, locale, mergeNumbers)](#apidoc.element.change-case.camelCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>constant (value, locale)](#apidoc.element.change-case.constant)
1.  [function <span class="apidocSignatureSpan">change-case.</span>constantCase (value, locale)](#apidoc.element.change-case.constantCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>dot (value, locale)](#apidoc.element.change-case.dot)
1.  [function <span class="apidocSignatureSpan">change-case.</span>dotCase (value, locale)](#apidoc.element.change-case.dotCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>header (value, locale)](#apidoc.element.change-case.header)
1.  [function <span class="apidocSignatureSpan">change-case.</span>headerCase (value, locale)](#apidoc.element.change-case.headerCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>isLower (string, locale)](#apidoc.element.change-case.isLower)
1.  [function <span class="apidocSignatureSpan">change-case.</span>isLowerCase (string, locale)](#apidoc.element.change-case.isLowerCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>isUpper (string, locale)](#apidoc.element.change-case.isUpper)
1.  [function <span class="apidocSignatureSpan">change-case.</span>isUpperCase (string, locale)](#apidoc.element.change-case.isUpperCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>lcFirst (str, locale)](#apidoc.element.change-case.lcFirst)
1.  [function <span class="apidocSignatureSpan">change-case.</span>lower (str, locale)](#apidoc.element.change-case.lower)
1.  [function <span class="apidocSignatureSpan">change-case.</span>lowerCase (str, locale)](#apidoc.element.change-case.lowerCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>lowerCaseFirst (str, locale)](#apidoc.element.change-case.lowerCaseFirst)
1.  [function <span class="apidocSignatureSpan">change-case.</span>no (str, locale, replacement)](#apidoc.element.change-case.no)
1.  [function <span class="apidocSignatureSpan">change-case.</span>noCase (str, locale, replacement)](#apidoc.element.change-case.noCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>param (value, locale)](#apidoc.element.change-case.param)
1.  [function <span class="apidocSignatureSpan">change-case.</span>paramCase (value, locale)](#apidoc.element.change-case.paramCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>pascal (value, locale, mergeNumbers)](#apidoc.element.change-case.pascal)
1.  [function <span class="apidocSignatureSpan">change-case.</span>pascalCase (value, locale, mergeNumbers)](#apidoc.element.change-case.pascalCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>path (value, locale)](#apidoc.element.change-case.path)
1.  [function <span class="apidocSignatureSpan">change-case.</span>pathCase (value, locale)](#apidoc.element.change-case.pathCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>sentence (value, locale)](#apidoc.element.change-case.sentence)
1.  [function <span class="apidocSignatureSpan">change-case.</span>sentenceCase (value, locale)](#apidoc.element.change-case.sentenceCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>snake (value, locale)](#apidoc.element.change-case.snake)
1.  [function <span class="apidocSignatureSpan">change-case.</span>snakeCase (value, locale)](#apidoc.element.change-case.snakeCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>swap (str, locale)](#apidoc.element.change-case.swap)
1.  [function <span class="apidocSignatureSpan">change-case.</span>swapCase (str, locale)](#apidoc.element.change-case.swapCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>title (value, locale)](#apidoc.element.change-case.title)
1.  [function <span class="apidocSignatureSpan">change-case.</span>titleCase (value, locale)](#apidoc.element.change-case.titleCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>ucFirst (str, locale)](#apidoc.element.change-case.ucFirst)
1.  [function <span class="apidocSignatureSpan">change-case.</span>upper (str, locale)](#apidoc.element.change-case.upper)
1.  [function <span class="apidocSignatureSpan">change-case.</span>upperCase (str, locale)](#apidoc.element.change-case.upperCase)
1.  [function <span class="apidocSignatureSpan">change-case.</span>upperCaseFirst (str, locale)](#apidoc.element.change-case.upperCaseFirst)



# <a name="apidoc.module.change-case"></a>[module change-case](#apidoc.module.change-case)

#### <a name="apidoc.element.change-case.camel"></a>[function <span class="apidocSignatureSpan">change-case.</span>camel (value, locale, mergeNumbers)](#apidoc.element.change-case.camel)
- description and source-code
```javascript
camel = function (value, locale, mergeNumbers) {
  var result = noCase(value, locale)

  // Replace periods between numeric entities with an underscore.
  if (!mergeNumbers) {
    result = result.replace(/ (?=\d)/g, '_')
  }

  // Replace spaces between words with an upper cased character.
  return result.replace(/ (.)/g, function (m, $1) {
    return upperCase($1, locale)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.camelCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>camelCase (value, locale, mergeNumbers)](#apidoc.element.change-case.camelCase)
- description and source-code
```javascript
camelCase = function (value, locale, mergeNumbers) {
  var result = noCase(value, locale)

  // Replace periods between numeric entities with an underscore.
  if (!mergeNumbers) {
    result = result.replace(/ (?=\d)/g, '_')
  }

  // Replace spaces between words with an upper cased character.
  return result.replace(/ (.)/g, function (m, $1) {
    return upperCase($1, locale)
  })
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/camel-case.svg?style=flat)](https://npmjs.org/package/camel-case)
[![Build status](https://img.shields.io/travis/blakeembrey/camel-case.svg?style=flat)](https://travis-ci.org/blakeembrey/camel-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/camel-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/camel
-case?branch=master)

Return as a string with the separators denoted by having the next letter capitalized.

'''js
changeCase.camelCase('test string')
//=> "testString"
'''

### [constantCase](https://github.com/blakeembrey/constant-case)

[![NPM version](https://img.shields.io/npm/v/constant-case.svg?style=flat)](https://npmjs.org/package/constant-case)
[![NPM downloads](https://img.shields.io/npm/dm/constant-case.svg?style=flat)](https://npmjs.org/package/constant-case)
...
```

#### <a name="apidoc.element.change-case.constant"></a>[function <span class="apidocSignatureSpan">change-case.</span>constant (value, locale)](#apidoc.element.change-case.constant)
- description and source-code
```javascript
constant = function (value, locale) {
  return upperCase(snakeCase(value, locale), locale)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.constantCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>constantCase (value, locale)](#apidoc.element.change-case.constantCase)
- description and source-code
```javascript
constantCase = function (value, locale) {
  return upperCase(snakeCase(value, locale), locale)
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/constant-case.svg?style=flat)](https://npmjs.org/package/constant-case)
[![Build status](https://img.shields.io/travis/blakeembrey/constant-case.svg?style=flat)](https://travis-ci.org/blakeembrey/constant
-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/constant-case.svg?style=flat)](https://coveralls.io/r/blakeembrey
/constant-case?branch=master)

Return as an upper case, underscore separated string.

'''js
changeCase.constantCase('test string')
//=> "TEST_STRING"
'''

### [dotCase](https://github.com/blakeembrey/dot-case)

[![NPM version](https://img.shields.io/npm/v/dot-case.svg?style=flat)](https://npmjs.org/package/dot-case)
[![NPM downloads](https://img.shields.io/npm/dm/dot-case.svg?style=flat)](https://npmjs.org/package/dot-case)
...
```

#### <a name="apidoc.element.change-case.dot"></a>[function <span class="apidocSignatureSpan">change-case.</span>dot (value, locale)](#apidoc.element.change-case.dot)
- description and source-code
```javascript
dot = function (value, locale) {
  return noCase(value, locale, '.')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.dotCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>dotCase (value, locale)](#apidoc.element.change-case.dotCase)
- description and source-code
```javascript
dotCase = function (value, locale) {
  return noCase(value, locale, '.')
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/dot-case.svg?style=flat)](https://npmjs.org/package/dot-case)
[![Build status](https://img.shields.io/travis/blakeembrey/dot-case.svg?style=flat)](https://travis-ci.org/blakeembrey/dot-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/dot-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/dot-
case?branch=master)

Return as a lower case, period separated string.

'''js
changeCase.dotCase('test string')
//=> "test.string"
'''

### [headerCase](https://github.com/blakeembrey/header-case)

[![NPM version](https://img.shields.io/npm/v/header-case.svg?style=flat)](https://npmjs.org/package/header-case)
[![NPM downloads](https://img.shields.io/npm/dm/header-case.svg?style=flat)](https://npmjs.org/package/header-case)
...
```

#### <a name="apidoc.element.change-case.header"></a>[function <span class="apidocSignatureSpan">change-case.</span>header (value, locale)](#apidoc.element.change-case.header)
- description and source-code
```javascript
header = function (value, locale) {
  return noCase(value, locale, '-').replace(/^.|-./g, function (m) {
    return upperCase(m, locale)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.headerCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>headerCase (value, locale)](#apidoc.element.change-case.headerCase)
- description and source-code
```javascript
headerCase = function (value, locale) {
  return noCase(value, locale, '-').replace(/^.|-./g, function (m) {
    return upperCase(m, locale)
  })
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/header-case.svg?style=flat)](https://npmjs.org/package/header-case)
[![Build status](https://img.shields.io/travis/blakeembrey/header-case.svg?style=flat)](https://travis-ci.org/blakeembrey/header
-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/header-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/header
-case?branch=master)

Return as a title cased, dash separated string.

'''js
changeCase.headerCase('test string')
//=> "Test-String"
'''

### [isLowerCase](https://github.com/blakeembrey/is-lower-case)

[![NPM version](https://img.shields.io/npm/v/is-lower-case.svg?style=flat)](https://npmjs.org/package/is-lower-case)
[![NPM downloads](https://img.shields.io/npm/dm/is-lower-case.svg?style=flat)](https://npmjs.org/package/is-lower-case)
...
```

#### <a name="apidoc.element.change-case.isLower"></a>[function <span class="apidocSignatureSpan">change-case.</span>isLower (string, locale)](#apidoc.element.change-case.isLower)
- description and source-code
```javascript
isLower = function (string, locale) {
  return lowerCase(string, locale) === string
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.isLowerCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>isLowerCase (string, locale)](#apidoc.element.change-case.isLowerCase)
- description and source-code
```javascript
isLowerCase = function (string, locale) {
  return lowerCase(string, locale) === string
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/is-lower-case.svg?style=flat)](https://npmjs.org/package/is-lower-case)
[![Build status](https://img.shields.io/travis/blakeembrey/is-lower-case.svg?style=flat)](https://travis-ci.org/blakeembrey/is-lower
-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/is-lower-case.svg?style=flat)](https://coveralls.io/r/blakeembrey
/is-lower-case?branch=master)

Return a boolean indicating whether the string is lower cased.

'''js
changeCase.isLowerCase('test string')
//=> true
'''

### [isUpperCase](https://github.com/blakeembrey/is-upper-case)

[![NPM version](https://img.shields.io/npm/v/is-upper-case.svg?style=flat)](https://npmjs.org/package/is-upper-case)
[![NPM downloads](https://img.shields.io/npm/dm/is-upper-case.svg?style=flat)](https://npmjs.org/package/is-upper-case)
...
```

#### <a name="apidoc.element.change-case.isUpper"></a>[function <span class="apidocSignatureSpan">change-case.</span>isUpper (string, locale)](#apidoc.element.change-case.isUpper)
- description and source-code
```javascript
isUpper = function (string, locale) {
  return upperCase(string, locale) === string
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.isUpperCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>isUpperCase (string, locale)](#apidoc.element.change-case.isUpperCase)
- description and source-code
```javascript
isUpperCase = function (string, locale) {
  return upperCase(string, locale) === string
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/is-upper-case.svg?style=flat)](https://npmjs.org/package/is-upper-case)
[![Build status](https://img.shields.io/travis/blakeembrey/is-upper-case.svg?style=flat)](https://travis-ci.org/blakeembrey/is-upper
-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/is-upper-case.svg?style=flat)](https://coveralls.io/r/blakeembrey
/is-upper-case?branch=master)

Return a boolean indicating whether the string is upper cased.

'''js
changeCase.isUpperCase('test string')
//=> false
'''

### [lowerCase](https://github.com/blakeembrey/lower-case)

[![NPM version](https://img.shields.io/npm/v/lower-case.svg?style=flat)](https://npmjs.org/package/lower-case)
[![NPM downloads](https://img.shields.io/npm/dm/lower-case.svg?style=flat)](https://npmjs.org/package/lower-case)
...
```

#### <a name="apidoc.element.change-case.lcFirst"></a>[function <span class="apidocSignatureSpan">change-case.</span>lcFirst (str, locale)](#apidoc.element.change-case.lcFirst)
- description and source-code
```javascript
lcFirst = function (str, locale) {
  if (str == null) {
    return ''
  }

  str = String(str)

  return lowerCase(str.charAt(0), locale) + str.substr(1)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.lower"></a>[function <span class="apidocSignatureSpan">change-case.</span>lower (str, locale)](#apidoc.element.change-case.lower)
- description and source-code
```javascript
lower = function (str, locale) {
  var lang = LANGUAGES[locale]

  str = str == null ? '' : String(str)

  if (lang) {
    str = str.replace(lang.regexp, function (m) { return lang.map[m] })
  }

  return str.toLowerCase()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.lowerCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>lowerCase (str, locale)](#apidoc.element.change-case.lowerCase)
- description and source-code
```javascript
lowerCase = function (str, locale) {
  var lang = LANGUAGES[locale]

  str = str == null ? '' : String(str)

  if (lang) {
    str = str.replace(lang.regexp, function (m) { return lang.map[m] })
  }

  return str.toLowerCase()
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/lower-case.svg?style=flat)](https://npmjs.org/package/lower-case)
[![Build status](https://img.shields.io/travis/blakeembrey/lower-case.svg?style=flat)](https://travis-ci.org/blakeembrey/lower-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/lower-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/lower
-case?branch=master)

Return the string in lower case.

'''js
changeCase.lowerCase('TEST STRING')
//=> "test string"
'''

### [lowerCaseFirst](https://github.com/blakeembrey/lower-case-first)

[![NPM version](https://img.shields.io/npm/v/lower-case-first.svg?style=flat)](https://npmjs.org/package/lower-case-first)
[![NPM downloads](https://img.shields.io/npm/dm/lower-case-first.svg?style=flat)](https://npmjs.org/package/lower-case-first)
...
```

#### <a name="apidoc.element.change-case.lowerCaseFirst"></a>[function <span class="apidocSignatureSpan">change-case.</span>lowerCaseFirst (str, locale)](#apidoc.element.change-case.lowerCaseFirst)
- description and source-code
```javascript
lowerCaseFirst = function (str, locale) {
  if (str == null) {
    return ''
  }

  str = String(str)

  return lowerCase(str.charAt(0), locale) + str.substr(1)
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/lower-case-first.svg?style=flat)](https://npmjs.org/package/lower-case-first)
[![Build status](https://img.shields.io/travis/blakeembrey/lower-case-first.svg?style=flat)](https://travis-ci.org/blakeembrey/lower
-case-first)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/lower-case-first.svg?style=flat)](https://coveralls.io/r/blakeembrey
/lower-case-first?branch=master)

Return the string with the first character lower cased.

'''js
changeCase.lowerCaseFirst('TEST')
//=> "tEST"
'''

### [noCase](https://github.com/blakeembrey/no-case)

[![NPM version](https://img.shields.io/npm/v/no-case.svg?style=flat)](https://npmjs.org/package/no-case)
[![NPM downloads](https://img.shields.io/npm/dm/no-case.svg?style=flat)](https://npmjs.org/package/no-case)
...
```

#### <a name="apidoc.element.change-case.no"></a>[function <span class="apidocSignatureSpan">change-case.</span>no (str, locale, replacement)](#apidoc.element.change-case.no)
- description and source-code
```javascript
no = function (str, locale, replacement) {
  if (str == null) {
    return ''
  }

  replacement = typeof replacement !== 'string' ? ' ' : replacement

  function replace (match, index, value) {
    if (index === 0 || index === (value.length - match.length)) {
      return ''
    }

    return replacement
  }

  str = String(str)
    // Support camel case ("camelCase" -> "camel Case").
    .replace(CAMEL_CASE_REGEXP, '$1 $2')
    // Support odd camel case ("CAMELCase" -> "CAMEL Case").
    .replace(CAMEL_CASE_UPPER_REGEXP, '$1 $2')
    // Remove all non-word characters and replace with a single space.
    .replace(NON_WORD_REGEXP, replace)

  // Lower case the entire string.
  return lowerCase(str, locale)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.noCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>noCase (str, locale, replacement)](#apidoc.element.change-case.noCase)
- description and source-code
```javascript
noCase = function (str, locale, replacement) {
  if (str == null) {
    return ''
  }

  replacement = typeof replacement !== 'string' ? ' ' : replacement

  function replace (match, index, value) {
    if (index === 0 || index === (value.length - match.length)) {
      return ''
    }

    return replacement
  }

  str = String(str)
    // Support camel case ("camelCase" -> "camel Case").
    .replace(CAMEL_CASE_REGEXP, '$1 $2')
    // Support odd camel case ("CAMELCase" -> "CAMEL Case").
    .replace(CAMEL_CASE_UPPER_REGEXP, '$1 $2')
    // Remove all non-word characters and replace with a single space.
    .replace(NON_WORD_REGEXP, replace)

  // Lower case the entire string.
  return lowerCase(str, locale)
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/no-case.svg?style=flat)](https://npmjs.org/package/no-case)
[![Build status](https://img.shields.io/travis/blakeembrey/no-case.svg?style=flat)](https://travci.org/blakeembrey/no-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/no-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/no-case
?branch=master)

Return the string without any casing (lower case, space separated).

'''js
changeCase.noCase('test string')
//=> "test string"
'''

### [paramCase](https://github.com/blakeembrey/param-case)

[![NPM version](https://img.shields.io/npm/v/param-case.svg?style=flat)](https://npmjs.org/package/param-case)
[![NPM downloads](https://img.shields.io/npm/dm/param-case.svg?style=flat)](https://npmjs.org/package/param-case)
...
```

#### <a name="apidoc.element.change-case.param"></a>[function <span class="apidocSignatureSpan">change-case.</span>param (value, locale)](#apidoc.element.change-case.param)
- description and source-code
```javascript
param = function (value, locale) {
  return noCase(value, locale, '-')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.paramCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>paramCase (value, locale)](#apidoc.element.change-case.paramCase)
- description and source-code
```javascript
paramCase = function (value, locale) {
  return noCase(value, locale, '-')
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/param-case.svg?style=flat)](https://npmjs.org/package/param-case)
[![Build status](https://img.shields.io/travis/blakeembrey/param-case.svg?style=flat)](https://travis-ci.org/blakeembrey/param-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/param-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/param
-case?branch=master)

Return as a lower case, dash separated string.

'''js
changeCase.paramCase('test string')
//=> "test-string"
'''

### [pascalCase](https://github.com/blakeembrey/pascal-case)

[![NPM version](https://img.shields.io/npm/v/pascal-case.svg?style=flat)](https://npmjs.org/package/pascal-case)
[![NPM downloads](https://img.shields.io/npm/dm/pascal-case.svg?style=flat)](https://npmjs.org/package/pascal-case)
...
```

#### <a name="apidoc.element.change-case.pascal"></a>[function <span class="apidocSignatureSpan">change-case.</span>pascal (value, locale, mergeNumbers)](#apidoc.element.change-case.pascal)
- description and source-code
```javascript
pascal = function (value, locale, mergeNumbers) {
  return upperCaseFirst(camelCase(value, locale, mergeNumbers), locale)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.pascalCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>pascalCase (value, locale, mergeNumbers)](#apidoc.element.change-case.pascalCase)
- description and source-code
```javascript
pascalCase = function (value, locale, mergeNumbers) {
  return upperCaseFirst(camelCase(value, locale, mergeNumbers), locale)
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/pascal-case.svg?style=flat)](https://npmjs.org/package/pascal-case)
[![Build status](https://img.shields.io/travis/blakeembrey/pascal-case.svg?style=flat)](https://travis-ci.org/blakeembrey/pascal
-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/pascal-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/pascal
-case?branch=master)

Return as a string denoted in the same fashion as 'camelCase', but with the first letter also capitalized.

'''js
changeCase.pascalCase('test string')
//=> "TestString"
'''

### [pathCase](https://github.com/blakeembrey/path-case)

[![NPM version](https://img.shields.io/npm/v/path-case.svg?style=flat)](https://npmjs.org/package/path-case)
[![NPM downloads](https://img.shields.io/npm/dm/path-case.svg?style=flat)](https://npmjs.org/package/path-case)
...
```

#### <a name="apidoc.element.change-case.path"></a>[function <span class="apidocSignatureSpan">change-case.</span>path (value, locale)](#apidoc.element.change-case.path)
- description and source-code
```javascript
path = function (value, locale) {
  return noCase(value, locale, '/')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.pathCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>pathCase (value, locale)](#apidoc.element.change-case.pathCase)
- description and source-code
```javascript
pathCase = function (value, locale) {
  return noCase(value, locale, '/')
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/path-case.svg?style=flat)](https://npmjs.org/package/path-case)
[![Build status](https://img.shields.io/travis/blakeembrey/path-case.svg?style=flat)](https://travis-ci.org/blakeembrey/path-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/path-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/path
-case?branch=master)

Return as a lower case, slash separated string.

'''js
changeCase.pathCase('test string')
//=> "test/string"
'''

### [sentenceCase](https://github.com/blakeembrey/sentence-case)

[![NPM version](https://img.shields.io/npm/v/sentence-case.svg?style=flat)](https://npmjs.org/package/sentence-case)
[![NPM downloads](https://img.shields.io/npm/dm/sentence-case.svg?style=flat)](https://npmjs.org/package/sentence-case)
...
```

#### <a name="apidoc.element.change-case.sentence"></a>[function <span class="apidocSignatureSpan">change-case.</span>sentence (value, locale)](#apidoc.element.change-case.sentence)
- description and source-code
```javascript
sentence = function (value, locale) {
  return upperCaseFirst(noCase(value, locale), locale)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.sentenceCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>sentenceCase (value, locale)](#apidoc.element.change-case.sentenceCase)
- description and source-code
```javascript
sentenceCase = function (value, locale) {
  return upperCaseFirst(noCase(value, locale), locale)
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/sentence-case.svg?style=flat)](https://npmjs.org/package/sentence-case)
[![Build status](https://img.shields.io/travis/blakeembrey/sentence-case.svg?style=flat)](https://travis-ci.org/blakeembrey/sentence
-case)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/sentence-case.svg?style=flat)](https://coveralls.io/r/blakeembrey
/sentence-case?branch=master)

Return as a lower case, space separated string with the first letter upper case.

'''js
changeCase.sentenceCase('testString')
//=> "Test string"
'''

### [snakeCase](https://github.com/blakeembrey/snake-case)

[![NPM version](https://img.shields.io/npm/v/snake-case.svg?style=flat)](https://npmjs.org/package/snake-case)
[![NPM downloads](https://img.shields.io/npm/dm/snake-case.svg?style=flat)](https://npmjs.org/package/snake-case)
...
```

#### <a name="apidoc.element.change-case.snake"></a>[function <span class="apidocSignatureSpan">change-case.</span>snake (value, locale)](#apidoc.element.change-case.snake)
- description and source-code
```javascript
snake = function (value, locale) {
  return noCase(value, locale, '_')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.snakeCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>snakeCase (value, locale)](#apidoc.element.change-case.snakeCase)
- description and source-code
```javascript
snakeCase = function (value, locale) {
  return noCase(value, locale, '_')
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/snake-case.svg?style=flat)](https://npmjs.org/package/snake-case)
[![Build status](https://img.shields.io/travis/blakeembrey/snake-case.svg?style=flat)](https://travis-ci.org/blakeembrey/snake-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/snake-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/snake
-case?branch=master)

Return as a lower case, underscore separated string.

'''js
changeCase.snakeCase('test string')
//=> "test_string"
'''

### [swapCase](https://github.com/blakeembrey/swap-case)

[![NPM version](https://img.shields.io/npm/v/swap-case.svg?style=flat)](https://npmjs.org/package/swap-case)
[![NPM downloads](https://img.shields.io/npm/dm/swap-case.svg?style=flat)](https://npmjs.org/package/swap-case)
...
```

#### <a name="apidoc.element.change-case.swap"></a>[function <span class="apidocSignatureSpan">change-case.</span>swap (str, locale)](#apidoc.element.change-case.swap)
- description and source-code
```javascript
swap = function (str, locale) {
  if (str == null) {
    return ''
  }

  var result = ''

  for (var i = 0; i < str.length; i++) {
    var c = str[i]
    var u = upperCase(c, locale)

    result += u === c ? lowerCase(c, locale) : u
  }

  return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.swapCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>swapCase (str, locale)](#apidoc.element.change-case.swapCase)
- description and source-code
```javascript
swapCase = function (str, locale) {
  if (str == null) {
    return ''
  }

  var result = ''

  for (var i = 0; i < str.length; i++) {
    var c = str[i]
    var u = upperCase(c, locale)

    result += u === c ? lowerCase(c, locale) : u
  }

  return result
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/swap-case.svg?style=flat)](https://npmjs.org/package/swap-case)
[![Build status](https://img.shields.io/travis/blakeembrey/swap-case.svg?style=flat)](https://travis-ci.org/blakeembrey/swap-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/swap-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/swap
-case?branch=master)

Return as a string with every character case reversed.

'''js
changeCase.swapCase('Test String')
//=> "tEST sTRING"
'''

### [titleCase](https://github.com/blakeembrey/title-case)

[![NPM version](https://img.shields.io/npm/v/title-case.svg?style=flat)](https://npmjs.org/package/title-case)
[![NPM downloads](https://img.shields.io/npm/dm/title-case.svg?style=flat)](https://npmjs.org/package/title-case)
...
```

#### <a name="apidoc.element.change-case.title"></a>[function <span class="apidocSignatureSpan">change-case.</span>title (value, locale)](#apidoc.element.change-case.title)
- description and source-code
```javascript
title = function (value, locale) {
  return noCase(value, locale).replace(/^.| ./g, function (m) {
    return upperCase(m, locale)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.titleCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>titleCase (value, locale)](#apidoc.element.change-case.titleCase)
- description and source-code
```javascript
titleCase = function (value, locale) {
  return noCase(value, locale).replace(/^.| ./g, function (m) {
    return upperCase(m, locale)
  })
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/title-case.svg?style=flat)](https://npmjs.org/package/title-case)
[![Build status](https://img.shields.io/travis/blakeembrey/title-case.svg?style=flat)](https://travis-ci.org/blakeembrey/title-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/title-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/title
-case?branch=master)

Return as a space separated string with the first character of every word upper cased.

'''js
changeCase.titleCase('a simple test')
//=> "A Simple Test"
'''

### [upperCase](https://github.com/blakeembrey/upper-case)

[![NPM version](https://img.shields.io/npm/v/upper-case.svg?style=flat)](https://npmjs.org/package/upper-case)
[![NPM downloads](https://img.shields.io/npm/dm/upper-case.svg?style=flat)](https://npmjs.org/package/upper-case)
...
```

#### <a name="apidoc.element.change-case.ucFirst"></a>[function <span class="apidocSignatureSpan">change-case.</span>ucFirst (str, locale)](#apidoc.element.change-case.ucFirst)
- description and source-code
```javascript
ucFirst = function (str, locale) {
  if (str == null) {
    return ''
  }

  str = String(str)

  return upperCase(str.charAt(0), locale) + str.substr(1)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.upper"></a>[function <span class="apidocSignatureSpan">change-case.</span>upper (str, locale)](#apidoc.element.change-case.upper)
- description and source-code
```javascript
upper = function (str, locale) {
  var lang = LANGUAGES[locale]

  str = str == null ? '' : String(str)

  if (lang) {
    str = str.replace(lang.regexp, function (m) { return lang.map[m] })
  }

  return str.toUpperCase()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.change-case.upperCase"></a>[function <span class="apidocSignatureSpan">change-case.</span>upperCase (str, locale)](#apidoc.element.change-case.upperCase)
- description and source-code
```javascript
upperCase = function (str, locale) {
  var lang = LANGUAGES[locale]

  str = str == null ? '' : String(str)

  if (lang) {
    str = str.replace(lang.regexp, function (m) { return lang.map[m] })
  }

  return str.toUpperCase()
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/upper-case.svg?style=flat)](https://npmjs.org/package/upper-case)
[![Build status](https://img.shields.io/travis/blakeembrey/upper-case.svg?style=flat)](https://travci.org/blakeembrey/upper-case
)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/upper-case.svg?style=flat)](https://coveralls.io/r/blakeembrey/upper
-case?branch=master)

Return the string in upper case.

'''js
changeCase.upperCase('test string')
//=> "TEST STRING"
'''

### [upperCaseFirst](https://github.com/blakeembrey/upper-case-first)

[![NPM version](https://img.shields.io/npm/v/upper-case-first.svg?style=flat)](https://npmjs.org/package/upper-case-first)
[![NPM downloads](https://img.shields.io/npm/dm/upper-case-first.svg?style=flat)](https://npmjs.org/package/upper-case-first)
...
```

#### <a name="apidoc.element.change-case.upperCaseFirst"></a>[function <span class="apidocSignatureSpan">change-case.</span>upperCaseFirst (str, locale)](#apidoc.element.change-case.upperCaseFirst)
- description and source-code
```javascript
upperCaseFirst = function (str, locale) {
  if (str == null) {
    return ''
  }

  str = String(str)

  return upperCase(str.charAt(0), locale) + str.substr(1)
}
```
- example usage
```shell
...
[![NPM downloads](https://img.shields.io/npm/dm/upper-case-first.svg?style=flat)](https://npmjs.org/package/upper-case-first)
[![Build status](https://img.shields.io/travis/blakeembrey/upper-case-first.svg?style=flat)](https://travis-ci.org/blakeembrey/upper
-case-first)
[![Test coverage](https://img.shields.io/coveralls/blakeembrey/upper-case-first.svg?style=flat)](https://coveralls.io/r/blakeembrey
/upper-case-first?branch=master)

Return the string with the first character upper cased.

'''js
changeCase.upperCaseFirst('test')
//=> "Test"
'''

## Related

* [Meteor](https://github.com/Konecty/change-case)
* [Atom](https://github.com/robhurring/atom-change-case)
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
