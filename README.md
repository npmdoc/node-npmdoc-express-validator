# api documentation for  [express-validator (v3.1.2)](https://github.com/ctavan/express-validator)  [![npm package](https://img.shields.io/npm/v/npmdoc-express-validator.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-express-validator) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-validator.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-validator)
#### Express middleware for the validator module.

[![NPM](https://nodei.co/npm/express-validator.png?downloads=true)](https://www.npmjs.com/package/express-validator)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-validator/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-express-validator_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-validator/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-express-validator/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Christoph Tavan",
        "email": "dev@tavan.de"
    },
    "bugs": {
        "url": "https://github.com/ctavan/express-validator/issues"
    },
    "contributors": [
        {
            "name": "Chris O'Hara",
            "email": "cohara87@gmail.com"
        },
        {
            "name": "@orfaust"
        },
        {
            "name": "@zero21xxx"
        },
        {
            "name": "Roman Kalyakin",
            "email": "roman@kalyakin.com"
        },
        {
            "name": "Rusty Bailey",
            "email": "rustylbailey@gmail.com"
        },
        {
            "name": "Gustavo Henke",
            "email": "guhenke@gmail.com"
        },
        {
            "name": "Ayman Nedjmeddine",
            "email": "theycallmethedr@gmail.com"
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
        "express": "4.12.3",
        "jscs": "1.13.1",
        "jshint": "2.7.0",
        "mocha": "2.2.4",
        "nyc": "8.4.0",
        "supertest": "0.15.0",
        "typescript": "~2.0.10"
    },
    "directories": {},
    "dist": {
        "shasum": "bae23dfa11191398d5fcada3dd7c54f28428195a",
        "tarball": "https://registry.npmjs.org/express-validator/-/express-validator-3.1.2.tgz"
    },
    "engines": {
        "node": ">= 0.10"
    },
    "gitHead": "54a5c4629aa4e1c37a3c635ea481a195e0f9e72d",
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
            "name": "ctavan",
            "email": "dev@tavan.de"
        },
        {
            "name": "gustavohenke",
            "email": "guhenke@gmail.com"
        },
        {
            "name": "rustybailey",
            "email": "rustylbailey@gmail.com"
        }
    ],
    "name": "express-validator",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ctavan/express-validator.git"
    },
    "scripts": {
        "jscs": "jscs ./test ./lib",
        "jshint": "jshint ./test ./lib",
        "report-coverage": "cat coverage/lcov.info | coveralls",
        "test": "nyc mocha && tsc",
        "travis-build": "npm test && npm run jshint && npm run jscs"
    },
    "types": "./index.d.ts",
    "version": "3.1.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module express-validator](#apidoc.module.express-validator)
1.  object <span class="apidocSignatureSpan">express-validator.</span>utils
1.  object <span class="apidocSignatureSpan">express-validator.</span>validator

#### [module express-validator.utils](#apidoc.module.express-validator.utils)
1.  [function <span class="apidocSignatureSpan">express-validator.utils.</span>decorateAsValidationResult (obj, errors)](#apidoc.element.express-validator.utils.decorateAsValidationResult)
1.  [function <span class="apidocSignatureSpan">express-validator.utils.</span>formatParamOutput (param)](#apidoc.element.express-validator.utils.formatParamOutput)

#### [module express-validator.validator](#apidoc.module.express-validator.validator)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>blacklist ()](#apidoc.element.express-validator.validator.blacklist)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>contains ()](#apidoc.element.express-validator.validator.contains)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>equals ()](#apidoc.element.express-validator.validator.equals)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>escape ()](#apidoc.element.express-validator.validator.escape)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>extend (name, fn)](#apidoc.element.express-validator.validator.extend)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>init ()](#apidoc.element.express-validator.validator.init)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isAfter ()](#apidoc.element.express-validator.validator.isAfter)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isAlpha ()](#apidoc.element.express-validator.validator.isAlpha)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isAlphanumeric ()](#apidoc.element.express-validator.validator.isAlphanumeric)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isAscii ()](#apidoc.element.express-validator.validator.isAscii)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isBase64 ()](#apidoc.element.express-validator.validator.isBase64)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isBefore ()](#apidoc.element.express-validator.validator.isBefore)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isBoolean ()](#apidoc.element.express-validator.validator.isBoolean)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isByteLength ()](#apidoc.element.express-validator.validator.isByteLength)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isCreditCard ()](#apidoc.element.express-validator.validator.isCreditCard)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isCurrency ()](#apidoc.element.express-validator.validator.isCurrency)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isDataURI ()](#apidoc.element.express-validator.validator.isDataURI)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isDate ()](#apidoc.element.express-validator.validator.isDate)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isDecimal ()](#apidoc.element.express-validator.validator.isDecimal)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isDivisibleBy ()](#apidoc.element.express-validator.validator.isDivisibleBy)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isEmail ()](#apidoc.element.express-validator.validator.isEmail)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isEmpty ()](#apidoc.element.express-validator.validator.isEmpty)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isFQDN ()](#apidoc.element.express-validator.validator.isFQDN)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isFloat ()](#apidoc.element.express-validator.validator.isFloat)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isFullWidth ()](#apidoc.element.express-validator.validator.isFullWidth)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isHalfWidth ()](#apidoc.element.express-validator.validator.isHalfWidth)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isHexColor ()](#apidoc.element.express-validator.validator.isHexColor)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isHexadecimal ()](#apidoc.element.express-validator.validator.isHexadecimal)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isIP ()](#apidoc.element.express-validator.validator.isIP)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isISBN ()](#apidoc.element.express-validator.validator.isISBN)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isISIN ()](#apidoc.element.express-validator.validator.isISIN)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isISO8601 ()](#apidoc.element.express-validator.validator.isISO8601)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isISSN ()](#apidoc.element.express-validator.validator.isISSN)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isIn ()](#apidoc.element.express-validator.validator.isIn)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isInt ()](#apidoc.element.express-validator.validator.isInt)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isJSON ()](#apidoc.element.express-validator.validator.isJSON)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isLength ()](#apidoc.element.express-validator.validator.isLength)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isLowercase ()](#apidoc.element.express-validator.validator.isLowercase)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isMACAddress ()](#apidoc.element.express-validator.validator.isMACAddress)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isMD5 ()](#apidoc.element.express-validator.validator.isMD5)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isMobilePhone ()](#apidoc.element.express-validator.validator.isMobilePhone)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isMongoId ()](#apidoc.element.express-validator.validator.isMongoId)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isMultibyte ()](#apidoc.element.express-validator.validator.isMultibyte)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isNumeric ()](#apidoc.element.express-validator.validator.isNumeric)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isSurrogatePair ()](#apidoc.element.express-validator.validator.isSurrogatePair)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isURL ()](#apidoc.element.express-validator.validator.isURL)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isUUID ()](#apidoc.element.express-validator.validator.isUUID)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isUppercase ()](#apidoc.element.express-validator.validator.isUppercase)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isVariableWidth ()](#apidoc.element.express-validator.validator.isVariableWidth)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>isWhitelisted ()](#apidoc.element.express-validator.validator.isWhitelisted)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>ltrim ()](#apidoc.element.express-validator.validator.ltrim)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>matches ()](#apidoc.element.express-validator.validator.matches)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>normalizeEmail ()](#apidoc.element.express-validator.validator.normalizeEmail)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>rtrim ()](#apidoc.element.express-validator.validator.rtrim)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>stripLow ()](#apidoc.element.express-validator.validator.stripLow)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>toBoolean ()](#apidoc.element.express-validator.validator.toBoolean)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>toDate (date)](#apidoc.element.express-validator.validator.toDate)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>toFloat ()](#apidoc.element.express-validator.validator.toFloat)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>toInt ()](#apidoc.element.express-validator.validator.toInt)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>toString (input)](#apidoc.element.express-validator.validator.toString)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>trim ()](#apidoc.element.express-validator.validator.trim)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>unescape ()](#apidoc.element.express-validator.validator.unescape)
1.  [function <span class="apidocSignatureSpan">express-validator.validator.</span>whitelist ()](#apidoc.element.express-validator.validator.whitelist)
1.  string <span class="apidocSignatureSpan">express-validator.validator.</span>version



# <a name="apidoc.module.express-validator"></a>[module express-validator](#apidoc.module.express-validator)



# <a name="apidoc.module.express-validator.utils"></a>[module express-validator.utils](#apidoc.module.express-validator.utils)

#### <a name="apidoc.element.express-validator.utils.decorateAsValidationResult"></a>[function <span class="apidocSignatureSpan">express-validator.utils.</span>decorateAsValidationResult (obj, errors)](#apidoc.element.express-validator.utils.decorateAsValidationResult)
- description and source-code
```javascript
function decorateAsValidationResult(obj, errors) {
  var onlyFirstError = false;

  obj.isEmpty = function isEmpty() {
    return !errors.length;
  };

  obj.array = function allErrors() {
    var used = {};
    return !onlyFirstError ? errors : errors.filter(function(error) {
      if (used[error.param]) {
        return false;
      }

      used[error.param] = true;
      return true;
    });
  };

  obj.mapped = function mappedErrors() {
    return errors.reduce(function(mapping, error) {
      if (!onlyFirstError || !mapping[error.param]) {
        mapping[error.param] = error;
      }

      return mapping;
    }, {});
  };

  obj.useFirstErrorOnly = function useFirstErrorOnly(flag) {
    onlyFirstError = flag === undefined || flag;
    return obj;
  };

  obj.throw = function throwError() {
    if (errors.length) {
      throw decorateAsValidationResult(new Error('Validation failed'), errors);
    }
  };

  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.utils.formatParamOutput"></a>[function <span class="apidocSignatureSpan">express-validator.utils.</span>formatParamOutput (param)](#apidoc.element.express-validator.utils.formatParamOutput)
- description and source-code
```javascript
function formatParamOutput(param) {
  if (Array.isArray(param)) {
    param = param.reduce(function(prev, curr) {
      var part = '';
      if (validator.isInt(curr)) {
        part = '[' + curr + ']';
      } else {
        if (prev) {
          part = '.' + curr;
        } else {
          part = curr;
        }
      }

      return prev + part;
    });
  }

  return param;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-validator.validator"></a>[module express-validator.validator](#apidoc.module.express-validator.validator)

#### <a name="apidoc.element.express-validator.validator.blacklist"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>blacklist ()](#apidoc.element.express-validator.validator.blacklist)
- description and source-code
```javascript
blacklist = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.contains"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>contains ()](#apidoc.element.express-validator.validator.contains)
- description and source-code
```javascript
contains = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
   req.check('testparam', 'Error Message').notEmpty().isInt();
   req.check('testparam.child', 'Error Message').isInt(); // find nested params
   req.check(['testparam', 'child'], 'Error Message').isInt(); // find nested params
'''

Starts the validation of the specifed parameter, will look for the parameter in 'req' in the order 'params', 'query', 'body', then
 validate, you can use 'dot-notation' or an array to access nested values.

If a validator takes in params, you would call it like 'req.assert('reqParam').contains('thisString');'.

Validators are appended and can be chained. See [chriso/validator.js](https://github.com/chriso/validator.js) for available validators
, or [add your own](#customvalidators).

#### req.assert();
Alias for [req.check()](#reqcheck).

#### req.validate();
...
```

#### <a name="apidoc.element.express-validator.validator.equals"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>equals ()](#apidoc.element.express-validator.validator.equals)
- description and source-code
```javascript
equals = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.escape"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>escape ()](#apidoc.element.express-validator.validator.escape)
- description and source-code
```javascript
escape = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...

#### req.sanitize();
'''javascript

req.body.comment = 'a <span>comment</span>';
req.body.username = '   a user    ';

req.sanitize('comment').escape(); // returns 'a &lt;span&gt;comment&lt;/span&gt;'
req.sanitize('username').trim(); // returns 'a user'

console.log(req.body.comment); // 'a &lt;span&gt;comment&lt;/span&gt;'
console.log(req.body.username); // 'a user'

'''
...
```

#### <a name="apidoc.element.express-validator.validator.extend"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>extend (name, fn)](#apidoc.element.express-validator.validator.extend)
- description and source-code
```javascript
extend = function (name, fn) {
  validator[name] = function() {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.init"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>init ()](#apidoc.element.express-validator.validator.init)
- description and source-code
```javascript
init = function () {
  for (var name in validator) {
  if (typeof validator[name] !== 'function' || name === 'toString' ||
    name === 'toDate' || name === 'extend' || name === 'init' ||
    name === 'isServerSide') {
      continue;
  }
  validator.extend(name, validator[name]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isAfter"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isAfter ()](#apidoc.element.express-validator.validator.isAfter)
- description and source-code
```javascript
isAfter = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isAlpha"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isAlpha ()](#apidoc.element.express-validator.validator.isAlpha)
- description and source-code
```javascript
isAlpha = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
app.post('/:urlparam', function(req, res) {

// VALIDATION
// checkBody only checks req.body; none of the other req parameters
// Similarly checkParams only checks in req.params (URL params) and
// checkQuery only checks req.query (GET params).
req.checkBody('postparam', 'Invalid postparam').notEmpty().isInt();
req.checkParams('urlparam', 'Invalid urlparam').isAlpha();
req.checkQuery('getparam', 'Invalid getparam').isInt();

// OR assert can be used to check on all 3 types of params.
// req.assert('postparam', 'Invalid postparam').notEmpty().isInt();
// req.assert('urlparam', 'Invalid urlparam').isAlpha();
// req.assert('getparam', 'Invalid getparam').isInt();
...
```

#### <a name="apidoc.element.express-validator.validator.isAlphanumeric"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isAlphanumeric ()](#apidoc.element.express-validator.validator.isAlphanumeric)
- description and source-code
```javascript
isAlphanumeric = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isAscii"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isAscii ()](#apidoc.element.express-validator.validator.isAscii)
- description and source-code
```javascript
isAscii = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isBase64"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isBase64 ()](#apidoc.element.express-validator.validator.isBase64)
- description and source-code
```javascript
isBase64 = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isBefore"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isBefore ()](#apidoc.element.express-validator.validator.isBefore)
- description and source-code
```javascript
isBefore = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isBoolean"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isBoolean ()](#apidoc.element.express-validator.validator.isBoolean)
- description and source-code
```javascript
isBoolean = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isByteLength"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isByteLength ()](#apidoc.element.express-validator.validator.isByteLength)
- description and source-code
```javascript
isByteLength = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isCreditCard"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isCreditCard ()](#apidoc.element.express-validator.validator.isCreditCard)
- description and source-code
```javascript
isCreditCard = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isCurrency"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isCurrency ()](#apidoc.element.express-validator.validator.isCurrency)
- description and source-code
```javascript
isCurrency = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isDataURI"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isDataURI ()](#apidoc.element.express-validator.validator.isDataURI)
- description and source-code
```javascript
isDataURI = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isDate"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isDate ()](#apidoc.element.express-validator.validator.isDate)
- description and source-code
```javascript
isDate = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isDecimal"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isDecimal ()](#apidoc.element.express-validator.validator.isDecimal)
- description and source-code
```javascript
isDecimal = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isDivisibleBy"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isDivisibleBy ()](#apidoc.element.express-validator.validator.isDivisibleBy)
- description and source-code
```javascript
isDivisibleBy = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
'%1' is replaced with the first parameter to the validator
'%2' is replaced with the second parameter to the validator
etc...

Example:
'''javascript
req.assert('number', '%0 is not an integer').isInt();
req.assert('number', '%0 is not divisible by %1').isDivisibleBy(5);
'''

*Note:* string replacement does **not** work with the '.withMessage()' syntax. If you'd like to have per-validator error messages
 with string formatting, please use the [Validation by Schema](#validation-by-schema) method instead.

### Per-validation messages

You can provide an error message for a single validation with '.withMessage()'. This can be chained with the rest of your validation
, and if you don't use it for one of the validations then it will fall back to the default.
...
```

#### <a name="apidoc.element.express-validator.validator.isEmail"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isEmail ()](#apidoc.element.express-validator.validator.isEmail)
- description and source-code
```javascript
isEmail = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
## Validation result

### Result API
The method 'req.getValidationResult()' returns a Promise which resolves to a result object.

'''js
req.assert('email', 'required').notEmpty();
req.assert('email', 'valid email required').isEmail();
req.assert('password', '6 to 20 characters required').len(6, 20);

req.getValidationResult().then(function(result) {
  // do something with the validation result
});
'''
...
```

#### <a name="apidoc.element.express-validator.validator.isEmpty"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isEmpty ()](#apidoc.element.express-validator.validator.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...

// OR find the relevent param in all areas
req.sanitize('postparam').toBoolean();

// Alternatively use 'var result = yield req.getValidationResult();'
// when using generators e.g. with co-express
req.getValidationResult().then(function(result) {
  if (!result.isEmpty()) {
    res.send('There have been validation errors: ' + util.inspect(result.array()), 400);
    return;
  }
  res.json({
    urlparam: req.params.urlparam,
    getparam: req.params.getparam,
    postparam: req.params.postparam
...
```

#### <a name="apidoc.element.express-validator.validator.isFQDN"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isFQDN ()](#apidoc.element.express-validator.validator.isFQDN)
- description and source-code
```javascript
isFQDN = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isFloat"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isFloat ()](#apidoc.element.express-validator.validator.isFloat)
- description and source-code
```javascript
isFloat = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isFullWidth"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isFullWidth ()](#apidoc.element.express-validator.validator.isFullWidth)
- description and source-code
```javascript
isFullWidth = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isHalfWidth"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isHalfWidth ()](#apidoc.element.express-validator.validator.isHalfWidth)
- description and source-code
```javascript
isHalfWidth = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isHexColor"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isHexColor ()](#apidoc.element.express-validator.validator.isHexColor)
- description and source-code
```javascript
isHexColor = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isHexadecimal"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isHexadecimal ()](#apidoc.element.express-validator.validator.isHexadecimal)
- description and source-code
```javascript
isHexadecimal = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isIP"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isIP ()](#apidoc.element.express-validator.validator.isIP)
- description and source-code
```javascript
isIP = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isISBN"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isISBN ()](#apidoc.element.express-validator.validator.isISBN)
- description and source-code
```javascript
isISBN = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isISIN"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isISIN ()](#apidoc.element.express-validator.validator.isISIN)
- description and source-code
```javascript
isISIN = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isISO8601"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isISO8601 ()](#apidoc.element.express-validator.validator.isISO8601)
- description and source-code
```javascript
isISO8601 = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isISSN"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isISSN ()](#apidoc.element.express-validator.validator.isISSN)
- description and source-code
```javascript
isISSN = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isIn"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isIn ()](#apidoc.element.express-validator.validator.isIn)
- description and source-code
```javascript
isIn = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isInt"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isInt ()](#apidoc.element.express-validator.validator.isInt)
- description and source-code
```javascript
isInt = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...

app.post('/:urlparam', function(req, res) {

// VALIDATION
// checkBody only checks req.body; none of the other req parameters
// Similarly checkParams only checks in req.params (URL params) and
// checkQuery only checks req.query (GET params).
req.checkBody('postparam', 'Invalid postparam').notEmpty().isInt();
req.checkParams('urlparam', 'Invalid urlparam').isAlpha();
req.checkQuery('getparam', 'Invalid getparam').isInt();

// OR assert can be used to check on all 3 types of params.
// req.assert('postparam', 'Invalid postparam').notEmpty().isInt();
// req.assert('urlparam', 'Invalid urlparam').isAlpha();
// req.assert('getparam', 'Invalid getparam').isInt();
...
```

#### <a name="apidoc.element.express-validator.validator.isJSON"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isJSON ()](#apidoc.element.express-validator.validator.isJSON)
- description and source-code
```javascript
isJSON = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isLength"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isLength ()](#apidoc.element.express-validator.validator.isLength)
- description and source-code
```javascript
isLength = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isLowercase"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isLowercase ()](#apidoc.element.express-validator.validator.isLowercase)
- description and source-code
```javascript
isLowercase = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isMACAddress"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isMACAddress ()](#apidoc.element.express-validator.validator.isMACAddress)
- description and source-code
```javascript
isMACAddress = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isMD5"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isMD5 ()](#apidoc.element.express-validator.validator.isMD5)
- description and source-code
```javascript
isMD5 = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isMobilePhone"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isMobilePhone ()](#apidoc.element.express-validator.validator.isMobilePhone)
- description and source-code
```javascript
isMobilePhone = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isMongoId"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isMongoId ()](#apidoc.element.express-validator.validator.isMongoId)
- description and source-code
```javascript
isMongoId = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isMultibyte"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isMultibyte ()](#apidoc.element.express-validator.validator.isMultibyte)
- description and source-code
```javascript
isMultibyte = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isNumeric"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isNumeric ()](#apidoc.element.express-validator.validator.isNumeric)
- description and source-code
```javascript
isNumeric = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isSurrogatePair"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isSurrogatePair ()](#apidoc.element.express-validator.validator.isSurrogatePair)
- description and source-code
```javascript
isSurrogatePair = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isURL"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isURL ()](#apidoc.element.express-validator.validator.isURL)
- description and source-code
```javascript
isURL = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isUUID"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isUUID ()](#apidoc.element.express-validator.validator.isUUID)
- description and source-code
```javascript
isUUID = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isUppercase"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isUppercase ()](#apidoc.element.express-validator.validator.isUppercase)
- description and source-code
```javascript
isUppercase = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isVariableWidth"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isVariableWidth ()](#apidoc.element.express-validator.validator.isVariableWidth)
- description and source-code
```javascript
isVariableWidth = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.isWhitelisted"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>isWhitelisted ()](#apidoc.element.express-validator.validator.isWhitelisted)
- description and source-code
```javascript
isWhitelisted = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.ltrim"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>ltrim ()](#apidoc.element.express-validator.validator.ltrim)
- description and source-code
```javascript
ltrim = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.matches"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>matches ()](#apidoc.element.express-validator.validator.matches)
- description and source-code
```javascript
matches = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.normalizeEmail"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>normalizeEmail ()](#apidoc.element.express-validator.validator.normalizeEmail)
- description and source-code
```javascript
normalizeEmail = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.rtrim"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>rtrim ()](#apidoc.element.express-validator.validator.rtrim)
- description and source-code
```javascript
rtrim = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.stripLow"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>stripLow ()](#apidoc.element.express-validator.validator.stripLow)
- description and source-code
```javascript
stripLow = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.toBoolean"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>toBoolean ()](#apidoc.element.express-validator.validator.toBoolean)
- description and source-code
```javascript
toBoolean = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
// req.assert('postparam', 'Invalid postparam').notEmpty().isInt();
// req.assert('urlparam', 'Invalid urlparam').isAlpha();
// req.assert('getparam', 'Invalid getparam').isInt();

// SANITIZATION
// as with validation these will only validate the corresponding
// request object
req.sanitizeBody('postparam').toBoolean();
req.sanitizeParams('urlparam').toBoolean();
req.sanitizeQuery('getparam').toBoolean();

// OR find the relevent param in all areas
req.sanitize('postparam').toBoolean();

// Alternatively use 'var result = yield req.getValidationResult();'
...
```

#### <a name="apidoc.element.express-validator.validator.toDate"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>toDate (date)](#apidoc.element.express-validator.validator.toDate)
- description and source-code
```javascript
toDate = function (date) {
  if (Object.prototype.toString.call(date) === '[object Date]') {
    return date;
  }
  date = Date.parse(date);
  return !isNaN(date) ? new Date(date) : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.toFloat"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>toFloat ()](#apidoc.element.express-validator.validator.toFloat)
- description and source-code
```javascript
toFloat = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.toInt"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>toInt ()](#apidoc.element.express-validator.validator.toInt)
- description and source-code
```javascript
toInt = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.toString"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>toString (input)](#apidoc.element.express-validator.validator.toString)
- description and source-code
```javascript
toString = function (input) {
  if (typeof input === 'object' && input !== null && input.toString) {
    input = input.toString();
  } else if (input === null || typeof input === 'undefined' || (isNaN(input) && !input.length)) {
    input = '';
  }
  return '' + input;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.trim"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>trim ()](#apidoc.element.express-validator.validator.trim)
- description and source-code
```javascript
trim = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
#### req.sanitize();
'''javascript

req.body.comment = 'a <span>comment</span>';
req.body.username = '   a user    ';

req.sanitize('comment').escape(); // returns 'a &lt;span&gt;comment&lt;/span&gt;'
req.sanitize('username').trim(); // returns 'a user'

console.log(req.body.comment); // 'a &lt;span&gt;comment&lt;/span&gt;'
console.log(req.body.username); // 'a user'

'''

Sanitizes the specified parameter (using 'dot-notation' or array), the parameter will be updated to the sanitized result. Cannot
 be chained, and will return the result. See [chriso/validator.js](https://github.com/chriso/validator.js) for available sanitizers
, or [add your own](#customsanitizers).
...
```

#### <a name="apidoc.element.express-validator.validator.unescape"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>unescape ()](#apidoc.element.express-validator.validator.unescape)
- description and source-code
```javascript
unescape = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-validator.validator.whitelist"></a>[function <span class="apidocSignatureSpan">express-validator.validator.</span>whitelist ()](#apidoc.element.express-validator.validator.whitelist)
- description and source-code
```javascript
whitelist = function () {
  var args = Array.prototype.slice.call(arguments);
  args[0] = validator.toString(args[0]);
  return fn.apply(validator, args);
}
```
- example usage
```shell
...
console.log(req.body.comment); // 'a &lt;span&gt;comment&lt;/span&gt;'
console.log(req.body.username); // 'a user'

'''

Sanitizes the specified parameter (using 'dot-notation' or array), the parameter will be updated to the sanitized result. Cannot
 be chained, and will return the result. See [chriso/validator.js](https://github.com/chriso/validator.js) for available sanitizers
, or [add your own](#customsanitizers).

If a sanitizer takes in params, you would call it like 'req.sanitize('reqParam').whitelist(['a', 'b', 'c']);'.

If the parameter is present in multiple places with the same name e.g. 'req.params.comment' & 'req.query.comment', they will all
 be sanitized.

#### req.filter();
Alias for [req.sanitize()](#reqsanitize).

#### req.sanitizeBody();
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
