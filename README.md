# npmdoc-postcss

#### basic api documentation for  [postcss (v5.2.17)](http://postcss.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-postcss.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-postcss) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-postcss.svg)](https://travis-ci.org/npmdoc/node-npmdoc-postcss)

#### Tool for transforming styles with JS plugins

[![NPM](https://nodei.co/npm/postcss.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/postcss)

- [https://npmdoc.github.io/node-npmdoc-postcss/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-postcss/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-postcss/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-postcss/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-postcss/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-postcss/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrey Sitnik"
    },
    "browser": {
        "fs": false
    },
    "bugs": {
        "url": "https://github.com/postcss/postcss/issues"
    },
    "dependencies": {
        "chalk": "^1.1.3",
        "js-base64": "^2.1.9",
        "source-map": "^0.5.6",
        "supports-color": "^3.2.3"
    },
    "description": "Tool for transforming styles with JS plugins",
    "devDependencies": {
        "ava": "^0.17.0",
        "babel-core": "^6.24.0",
        "babel-eslint": "^7.1.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-precompile-charcodes": "^1.0.0",
        "babel-preset-es2015": "^6.24.0",
        "chalk": "^1.1.3",
        "concat-with-sourcemaps": "^1.0.4",
        "del": "^2.2.2",
        "docdash": "^0.4.0",
        "eslint": "^3.18.0",
        "eslint-config-postcss": "^2.0.2",
        "fs-extra": "^1.0.0",
        "gulp": "^3.9.1",
        "gulp-ava": "^0.15.0",
        "gulp-babel": "^6.1.2",
        "gulp-changed": "^1.3.2",
        "gulp-eslint": "^3.0.1",
        "gulp-run": "^1.7.1",
        "gulp-sourcemaps": "^2.4.1",
        "jsdoc": "^3.4.3",
        "lint-staged": "^3.4.0",
        "postcss-parser-tests": "^5.0.11",
        "pre-commit": "^1.2.2",
        "run-sequence": "^1.2.2",
        "sinon": "^2.0.0",
        "strip-ansi": "^3.0.1",
        "yaspeller-ci": "^0.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cf4f597b864d65c8a492b2eabe9d706c879c388b",
        "tarball": "https://registry.npmjs.org/postcss/-/postcss-5.2.17.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "homepage": "http://postcss.org/",
    "keywords": [
        "css",
        "postcss",
        "rework",
        "preprocessor",
        "parser",
        "source map",
        "transform",
        "manipulation",
        "transpiler"
    ],
    "license": "MIT",
    "lint-staged": {
        "test/*.js": "eslint",
        "lib/*.es6": "eslint",
        "*.md": "yaspeller-ci"
    },
    "main": "lib/postcss",
    "maintainers": [
        {
            "name": "ai"
        },
        {
            "name": "beneb"
        }
    ],
    "name": "postcss",
    "optionalDependencies": {},
    "pre-commit": [
        "lint-staged"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/postcss/postcss.git"
    },
    "scripts": {
        "lint-staged": "lint-staged",
        "test": "gulp"
    },
    "types": "lib/postcss.d.ts",
    "version": "5.2.17",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
