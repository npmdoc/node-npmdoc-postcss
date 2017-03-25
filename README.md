# api documentation for  [postcss (v5.2.16)](http://postcss.org/)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-postcss.svg)](https://travis-ci.org/npmdoc/node-npmdoc-postcss)
#### Tool for transforming styles with JS plugins

[![NPM](https://nodei.co/npm/postcss.png?downloads=true)](https://www.npmjs.com/package/postcss)

[![apidoc](https://npmdoc.github.io/node-npmdoc-postcss/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-postcss_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-postcss/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-postcss/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Andrey Sitnik",
        "email": "andrey@sitnik.ru"
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
        "babel-core": "^6.23.1",
        "babel-eslint": "^7.1.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-precompile-charcodes": "^1.0.0",
        "babel-preset-es2015": "^6.22.0",
        "chalk": "^1.1.3",
        "concat-with-sourcemaps": "^1.0.4",
        "del": "^2.2.2",
        "docdash": "^0.4.0",
        "eslint": "^3.17.1",
        "eslint-config-postcss": "^2.0.2",
        "fs-extra": "^2.0.0",
        "gulp": "^3.9.1",
        "gulp-ava": "^0.15.0",
        "gulp-babel": "^6.1.2",
        "gulp-changed": "^1.3.2",
        "gulp-eslint": "^3.0.1",
        "gulp-run": "^1.7.1",
        "gulp-sourcemaps": "^2.4.1",
        "jsdoc": "^3.4.3",
        "lint-staged": "^3.3.1",
        "postcss-parser-tests": "^5.0.11",
        "pre-commit": "^1.2.2",
        "run-sequence": "^1.2.2",
        "sinon": "^1.17.7",
        "strip-ansi": "^3.0.1",
        "yaspeller-ci": "^0.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "732b3100000f9ff8379a48a53839ed097376ad57",
        "tarball": "https://registry.npmjs.org/postcss/-/postcss-5.2.16.tgz"
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
            "name": "ai",
            "email": "andrey@sitnik.ru"
        },
        {
            "name": "beneb",
            "email": "beneb.info@gmail.com"
        }
    ],
    "name": "postcss",
    "optionalDependencies": {},
    "pre-commit": [
        "lint-staged"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/postcss/postcss.git"
    },
    "scripts": {
        "lint-staged": "lint-staged",
        "test": "gulp"
    },
    "types": "lib/postcss.d.ts",
    "version": "5.2.16"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module postcss](#apidoc.module.postcss)
1.  [function <span class="apidocSignatureSpan">postcss.</span>atRule (defaults)](#apidoc.element.postcss.atRule)
1.  [function <span class="apidocSignatureSpan">postcss.</span>at_rule (defaults)](#apidoc.element.postcss.at_rule)
1.  [function <span class="apidocSignatureSpan">postcss.</span>comment (defaults)](#apidoc.element.postcss.comment)
1.  [function <span class="apidocSignatureSpan">postcss.</span>container ()](#apidoc.element.postcss.container)
1.  [function <span class="apidocSignatureSpan">postcss.</span>css_syntax_error (message, line, column, source, file, plugin)](#apidoc.element.postcss.css_syntax_error)
1.  [function <span class="apidocSignatureSpan">postcss.</span>decl (defaults)](#apidoc.element.postcss.decl)
1.  [function <span class="apidocSignatureSpan">postcss.</span>input (css)](#apidoc.element.postcss.input)
1.  [function <span class="apidocSignatureSpan">postcss.</span>lazy_result (processor, css, opts)](#apidoc.element.postcss.lazy_result)
1.  [function <span class="apidocSignatureSpan">postcss.</span>map_generator (stringify, root, opts)](#apidoc.element.postcss.map_generator)
1.  [function <span class="apidocSignatureSpan">postcss.</span>node ()](#apidoc.element.postcss.node)
1.  [function <span class="apidocSignatureSpan">postcss.</span>parse (css, opts)](#apidoc.element.postcss.parse)
1.  [function <span class="apidocSignatureSpan">postcss.</span>parser (input)](#apidoc.element.postcss.parser)
1.  [function <span class="apidocSignatureSpan">postcss.</span>plugin (name, initializer)](#apidoc.element.postcss.plugin)
1.  [function <span class="apidocSignatureSpan">postcss.</span>previous_map (css, opts)](#apidoc.element.postcss.previous_map)
1.  [function <span class="apidocSignatureSpan">postcss.</span>processor ()](#apidoc.element.postcss.processor)
1.  [function <span class="apidocSignatureSpan">postcss.</span>result (processor, root, opts)](#apidoc.element.postcss.result)
1.  [function <span class="apidocSignatureSpan">postcss.</span>root (defaults)](#apidoc.element.postcss.root)
1.  [function <span class="apidocSignatureSpan">postcss.</span>rule (defaults)](#apidoc.element.postcss.rule)
1.  [function <span class="apidocSignatureSpan">postcss.</span>stringifier (builder)](#apidoc.element.postcss.stringifier)
1.  [function <span class="apidocSignatureSpan">postcss.</span>stringify (node, builder)](#apidoc.element.postcss.stringify)
1.  [function <span class="apidocSignatureSpan">postcss.</span>warning (text)](#apidoc.element.postcss.warning)
1.  object <span class="apidocSignatureSpan">postcss.</span>at_rule.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>container.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>css_syntax_error.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>input.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>lazy_result.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>list
1.  object <span class="apidocSignatureSpan">postcss.</span>map_generator.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>node.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>parser.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>previous_map.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>processor.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>result.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>root.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>stringifier.prototype
1.  object <span class="apidocSignatureSpan">postcss.</span>vendor
1.  object <span class="apidocSignatureSpan">postcss.</span>warning.prototype

#### [module postcss.at_rule](#apidoc.module.postcss.at_rule)
1.  [function <span class="apidocSignatureSpan">postcss.</span>at_rule (defaults)](#apidoc.element.postcss.at_rule.at_rule)

#### [module postcss.at_rule.prototype](#apidoc.module.postcss.at_rule.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.at_rule.prototype.</span>append ()](#apidoc.element.postcss.at_rule.prototype.append)
1.  [function <span class="apidocSignatureSpan">postcss.at_rule.prototype.</span>prepend ()](#apidoc.element.postcss.at_rule.prototype.prepend)

#### [module postcss.container](#apidoc.module.postcss.container)
1.  [function <span class="apidocSignatureSpan">postcss.</span>container ()](#apidoc.element.postcss.container.container)

#### [module postcss.container.prototype](#apidoc.module.postcss.container.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>append ()](#apidoc.element.postcss.container.prototype.append)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>cleanRaws (keepBetween)](#apidoc.element.postcss.container.prototype.cleanRaws)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>each (callback)](#apidoc.element.postcss.container.prototype.each)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachAtRule (name, callback)](#apidoc.element.postcss.container.prototype.eachAtRule)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachComment (callback)](#apidoc.element.postcss.container.prototype.eachComment)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachDecl (prop, callback)](#apidoc.element.postcss.container.prototype.eachDecl)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachInside (callback)](#apidoc.element.postcss.container.prototype.eachInside)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachRule (selector, callback)](#apidoc.element.postcss.container.prototype.eachRule)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>every (condition)](#apidoc.element.postcss.container.prototype.every)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>index (child)](#apidoc.element.postcss.container.prototype.index)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>insertAfter (exist, add)](#apidoc.element.postcss.container.prototype.insertAfter)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>insertBefore (exist, add)](#apidoc.element.postcss.container.prototype.insertBefore)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>normalize (nodes, sample)](#apidoc.element.postcss.container.prototype.normalize)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>prepend ()](#apidoc.element.postcss.container.prototype.prepend)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>push (child)](#apidoc.element.postcss.container.prototype.push)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>rebuild (node, parent)](#apidoc.element.postcss.container.prototype.rebuild)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>remove (child)](#apidoc.element.postcss.container.prototype.remove)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>removeAll ()](#apidoc.element.postcss.container.prototype.removeAll)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>removeChild (child)](#apidoc.element.postcss.container.prototype.removeChild)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>replaceValues (pattern, opts, callback)](#apidoc.element.postcss.container.prototype.replaceValues)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>some (condition)](#apidoc.element.postcss.container.prototype.some)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walk (callback)](#apidoc.element.postcss.container.prototype.walk)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkAtRules (name, callback)](#apidoc.element.postcss.container.prototype.walkAtRules)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkComments (callback)](#apidoc.element.postcss.container.prototype.walkComments)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkDecls (prop, callback)](#apidoc.element.postcss.container.prototype.walkDecls)
1.  [function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkRules (selector, callback)](#apidoc.element.postcss.container.prototype.walkRules)

#### [module postcss.css_syntax_error](#apidoc.module.postcss.css_syntax_error)
1.  [function <span class="apidocSignatureSpan">postcss.</span>css_syntax_error (message, line, column, source, file, plugin)](#apidoc.element.postcss.css_syntax_error.css_syntax_error)

#### [module postcss.css_syntax_error.prototype](#apidoc.module.postcss.css_syntax_error.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.css_syntax_error.prototype.</span>setMessage ()](#apidoc.element.postcss.css_syntax_error.prototype.setMessage)
1.  [function <span class="apidocSignatureSpan">postcss.css_syntax_error.prototype.</span>showSourceCode (color)](#apidoc.element.postcss.css_syntax_error.prototype.showSourceCode)
1.  [function <span class="apidocSignatureSpan">postcss.css_syntax_error.prototype.</span>toString ()](#apidoc.element.postcss.css_syntax_error.prototype.toString)

#### [module postcss.input](#apidoc.module.postcss.input)
1.  [function <span class="apidocSignatureSpan">postcss.</span>input (css)](#apidoc.element.postcss.input.input)

#### [module postcss.input.prototype](#apidoc.module.postcss.input.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.input.prototype.</span>error (message, line, column)](#apidoc.element.postcss.input.prototype.error)
1.  [function <span class="apidocSignatureSpan">postcss.input.prototype.</span>mapResolve (file)](#apidoc.element.postcss.input.prototype.mapResolve)
1.  [function <span class="apidocSignatureSpan">postcss.input.prototype.</span>origin (line, column)](#apidoc.element.postcss.input.prototype.origin)

#### [module postcss.lazy_result](#apidoc.module.postcss.lazy_result)
1.  [function <span class="apidocSignatureSpan">postcss.</span>lazy_result (processor, css, opts)](#apidoc.element.postcss.lazy_result.lazy_result)

#### [module postcss.lazy_result.prototype](#apidoc.module.postcss.lazy_result.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>async ()](#apidoc.element.postcss.lazy_result.prototype.async)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>asyncTick (resolve, reject)](#apidoc.element.postcss.lazy_result.prototype.asyncTick)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>catch (onRejected)](#apidoc.element.postcss.lazy_result.prototype.catch)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>handleError (error, plugin)](#apidoc.element.postcss.lazy_result.prototype.handleError)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>run (plugin)](#apidoc.element.postcss.lazy_result.prototype.run)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>stringify ()](#apidoc.element.postcss.lazy_result.prototype.stringify)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>sync ()](#apidoc.element.postcss.lazy_result.prototype.sync)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>then (onFulfilled, onRejected)](#apidoc.element.postcss.lazy_result.prototype.then)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>toString ()](#apidoc.element.postcss.lazy_result.prototype.toString)
1.  [function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>warnings ()](#apidoc.element.postcss.lazy_result.prototype.warnings)

#### [module postcss.list](#apidoc.module.postcss.list)
1.  [function <span class="apidocSignatureSpan">postcss.list.</span>comma (string)](#apidoc.element.postcss.list.comma)
1.  [function <span class="apidocSignatureSpan">postcss.list.</span>space (string)](#apidoc.element.postcss.list.space)
1.  [function <span class="apidocSignatureSpan">postcss.list.</span>split (string, separators, last)](#apidoc.element.postcss.list.split)

#### [module postcss.map_generator](#apidoc.module.postcss.map_generator)
1.  [function <span class="apidocSignatureSpan">postcss.</span>map_generator (stringify, root, opts)](#apidoc.element.postcss.map_generator.map_generator)

#### [module postcss.map_generator.prototype](#apidoc.module.postcss.map_generator.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>addAnnotation ()](#apidoc.element.postcss.map_generator.prototype.addAnnotation)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>applyPrevMaps ()](#apidoc.element.postcss.map_generator.prototype.applyPrevMaps)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>clearAnnotation ()](#apidoc.element.postcss.map_generator.prototype.clearAnnotation)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>generate ()](#apidoc.element.postcss.map_generator.prototype.generate)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>generateMap ()](#apidoc.element.postcss.map_generator.prototype.generateMap)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>generateString ()](#apidoc.element.postcss.map_generator.prototype.generateString)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isAnnotation ()](#apidoc.element.postcss.map_generator.prototype.isAnnotation)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isInline ()](#apidoc.element.postcss.map_generator.prototype.isInline)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isMap ()](#apidoc.element.postcss.map_generator.prototype.isMap)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isSourcesContent ()](#apidoc.element.postcss.map_generator.prototype.isSourcesContent)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>outputFile ()](#apidoc.element.postcss.map_generator.prototype.outputFile)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>previous ()](#apidoc.element.postcss.map_generator.prototype.previous)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>relative (file)](#apidoc.element.postcss.map_generator.prototype.relative)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>setSourcesContent ()](#apidoc.element.postcss.map_generator.prototype.setSourcesContent)
1.  [function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>sourcePath (node)](#apidoc.element.postcss.map_generator.prototype.sourcePath)

#### [module postcss.node](#apidoc.module.postcss.node)
1.  [function <span class="apidocSignatureSpan">postcss.</span>node ()](#apidoc.element.postcss.node.node)

#### [module postcss.node.prototype](#apidoc.module.postcss.node.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cleanRaws (keepBetween)](#apidoc.element.postcss.node.prototype.cleanRaws)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cleanStyles (keepBetween)](#apidoc.element.postcss.node.prototype.cleanStyles)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>clone ()](#apidoc.element.postcss.node.prototype.clone)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cloneAfter ()](#apidoc.element.postcss.node.prototype.cloneAfter)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cloneBefore ()](#apidoc.element.postcss.node.prototype.cloneBefore)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>error (message)](#apidoc.element.postcss.node.prototype.error)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>moveAfter (otherNode)](#apidoc.element.postcss.node.prototype.moveAfter)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>moveBefore (otherNode)](#apidoc.element.postcss.node.prototype.moveBefore)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>moveTo (newParent)](#apidoc.element.postcss.node.prototype.moveTo)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>next ()](#apidoc.element.postcss.node.prototype.next)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>positionBy (opts)](#apidoc.element.postcss.node.prototype.positionBy)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>positionInside (index)](#apidoc.element.postcss.node.prototype.positionInside)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>prev ()](#apidoc.element.postcss.node.prototype.prev)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>raw (prop, defaultType)](#apidoc.element.postcss.node.prototype.raw)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>remove ()](#apidoc.element.postcss.node.prototype.remove)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>removeSelf ()](#apidoc.element.postcss.node.prototype.removeSelf)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>replace (nodes)](#apidoc.element.postcss.node.prototype.replace)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>replaceWith ()](#apidoc.element.postcss.node.prototype.replaceWith)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>root ()](#apidoc.element.postcss.node.prototype.root)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>style (own, detect)](#apidoc.element.postcss.node.prototype.style)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>toJSON ()](#apidoc.element.postcss.node.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>toString ()](#apidoc.element.postcss.node.prototype.toString)
1.  [function <span class="apidocSignatureSpan">postcss.node.prototype.</span>warn (result, text, opts)](#apidoc.element.postcss.node.prototype.warn)

#### [module postcss.parser](#apidoc.module.postcss.parser)
1.  [function <span class="apidocSignatureSpan">postcss.</span>parser (input)](#apidoc.element.postcss.parser.parser)

#### [module postcss.parser.prototype](#apidoc.module.postcss.parser.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>atrule (token)](#apidoc.element.postcss.parser.prototype.atrule)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>checkMissedSemicolon (tokens)](#apidoc.element.postcss.parser.prototype.checkMissedSemicolon)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>colon (tokens)](#apidoc.element.postcss.parser.prototype.colon)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>comment (token)](#apidoc.element.postcss.parser.prototype.comment)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>decl (tokens)](#apidoc.element.postcss.parser.prototype.decl)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>doubleColon (token)](#apidoc.element.postcss.parser.prototype.doubleColon)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>emptyRule (token)](#apidoc.element.postcss.parser.prototype.emptyRule)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>end (token)](#apidoc.element.postcss.parser.prototype.end)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>endFile ()](#apidoc.element.postcss.parser.prototype.endFile)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>init (node, line, column)](#apidoc.element.postcss.parser.prototype.init)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>loop ()](#apidoc.element.postcss.parser.prototype.loop)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>other ()](#apidoc.element.postcss.parser.prototype.other)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>precheckMissedSemicolon (tokens)](#apidoc.element.postcss.parser.prototype.precheckMissedSemicolon)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>raw (node, prop, tokens)](#apidoc.element.postcss.parser.prototype.raw)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>rule (tokens)](#apidoc.element.postcss.parser.prototype.rule)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>spacesAndCommentsFromEnd (tokens)](#apidoc.element.postcss.parser.prototype.spacesAndCommentsFromEnd)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>spacesAndCommentsFromStart (tokens)](#apidoc.element.postcss.parser.prototype.spacesAndCommentsFromStart)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>spacesFromEnd (tokens)](#apidoc.element.postcss.parser.prototype.spacesFromEnd)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>stringFrom (tokens, from)](#apidoc.element.postcss.parser.prototype.stringFrom)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>tokenize ()](#apidoc.element.postcss.parser.prototype.tokenize)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unclosedBlock ()](#apidoc.element.postcss.parser.prototype.unclosedBlock)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unclosedBracket (bracket)](#apidoc.element.postcss.parser.prototype.unclosedBracket)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unexpectedClose (token)](#apidoc.element.postcss.parser.prototype.unexpectedClose)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unknownWord (start)](#apidoc.element.postcss.parser.prototype.unknownWord)
1.  [function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unnamedAtrule (node, token)](#apidoc.element.postcss.parser.prototype.unnamedAtrule)

#### [module postcss.previous_map](#apidoc.module.postcss.previous_map)
1.  [function <span class="apidocSignatureSpan">postcss.</span>previous_map (css, opts)](#apidoc.element.postcss.previous_map.previous_map)

#### [module postcss.previous_map.prototype](#apidoc.module.postcss.previous_map.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>consumer ()](#apidoc.element.postcss.previous_map.prototype.consumer)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>decodeInline (text)](#apidoc.element.postcss.previous_map.prototype.decodeInline)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>isMap (map)](#apidoc.element.postcss.previous_map.prototype.isMap)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>loadAnnotation (css)](#apidoc.element.postcss.previous_map.prototype.loadAnnotation)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>loadMap (file, prev)](#apidoc.element.postcss.previous_map.prototype.loadMap)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>startWith (string, start)](#apidoc.element.postcss.previous_map.prototype.startWith)
1.  [function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>withContent ()](#apidoc.element.postcss.previous_map.prototype.withContent)

#### [module postcss.processor](#apidoc.module.postcss.processor)
1.  [function <span class="apidocSignatureSpan">postcss.</span>processor ()](#apidoc.element.postcss.processor.processor)

#### [module postcss.processor.prototype](#apidoc.module.postcss.processor.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.processor.prototype.</span>normalize (plugins)](#apidoc.element.postcss.processor.prototype.normalize)
1.  [function <span class="apidocSignatureSpan">postcss.processor.prototype.</span>process (css)](#apidoc.element.postcss.processor.prototype.process)
1.  [function <span class="apidocSignatureSpan">postcss.processor.prototype.</span>use (plugin)](#apidoc.element.postcss.processor.prototype.use)

#### [module postcss.result](#apidoc.module.postcss.result)
1.  [function <span class="apidocSignatureSpan">postcss.</span>result (processor, root, opts)](#apidoc.element.postcss.result.result)

#### [module postcss.result.prototype](#apidoc.module.postcss.result.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.result.prototype.</span>toString ()](#apidoc.element.postcss.result.prototype.toString)
1.  [function <span class="apidocSignatureSpan">postcss.result.prototype.</span>warn (text)](#apidoc.element.postcss.result.prototype.warn)
1.  [function <span class="apidocSignatureSpan">postcss.result.prototype.</span>warnings ()](#apidoc.element.postcss.result.prototype.warnings)

#### [module postcss.root](#apidoc.module.postcss.root)
1.  [function <span class="apidocSignatureSpan">postcss.</span>root (defaults)](#apidoc.element.postcss.root.root)

#### [module postcss.root.prototype](#apidoc.module.postcss.root.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.root.prototype.</span>normalize (child, sample, type)](#apidoc.element.postcss.root.prototype.normalize)
1.  [function <span class="apidocSignatureSpan">postcss.root.prototype.</span>prevMap ()](#apidoc.element.postcss.root.prototype.prevMap)
1.  [function <span class="apidocSignatureSpan">postcss.root.prototype.</span>remove (child)](#apidoc.element.postcss.root.prototype.remove)
1.  [function <span class="apidocSignatureSpan">postcss.root.prototype.</span>removeChild (child)](#apidoc.element.postcss.root.prototype.removeChild)
1.  [function <span class="apidocSignatureSpan">postcss.root.prototype.</span>toResult ()](#apidoc.element.postcss.root.prototype.toResult)

#### [module postcss.stringifier](#apidoc.module.postcss.stringifier)
1.  [function <span class="apidocSignatureSpan">postcss.</span>stringifier (builder)](#apidoc.element.postcss.stringifier.stringifier)

#### [module postcss.stringifier.prototype](#apidoc.module.postcss.stringifier.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>atrule (node, semicolon)](#apidoc.element.postcss.stringifier.prototype.atrule)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>beforeAfter (node, detect)](#apidoc.element.postcss.stringifier.prototype.beforeAfter)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>block (node, start)](#apidoc.element.postcss.stringifier.prototype.block)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>body (node)](#apidoc.element.postcss.stringifier.prototype.body)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>comment (node)](#apidoc.element.postcss.stringifier.prototype.comment)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>decl (node, semicolon)](#apidoc.element.postcss.stringifier.prototype.decl)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>raw (node, own, detect)](#apidoc.element.postcss.stringifier.prototype.raw)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeClose (root)](#apidoc.element.postcss.stringifier.prototype.rawBeforeClose)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeComment (root, node)](#apidoc.element.postcss.stringifier.prototype.rawBeforeComment)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeDecl (root, node)](#apidoc.element.postcss.stringifier.prototype.rawBeforeDecl)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeOpen (root)](#apidoc.element.postcss.stringifier.prototype.rawBeforeOpen)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeRule (root)](#apidoc.element.postcss.stringifier.prototype.rawBeforeRule)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawColon (root)](#apidoc.element.postcss.stringifier.prototype.rawColon)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawEmptyBody (root)](#apidoc.element.postcss.stringifier.prototype.rawEmptyBody)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawIndent (root)](#apidoc.element.postcss.stringifier.prototype.rawIndent)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawSemicolon (root)](#apidoc.element.postcss.stringifier.prototype.rawSemicolon)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawValue (node, prop)](#apidoc.element.postcss.stringifier.prototype.rawValue)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>root (node)](#apidoc.element.postcss.stringifier.prototype.root)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rule (node)](#apidoc.element.postcss.stringifier.prototype.rule)
1.  [function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>stringify (node, semicolon)](#apidoc.element.postcss.stringifier.prototype.stringify)

#### [module postcss.vendor](#apidoc.module.postcss.vendor)
1.  [function <span class="apidocSignatureSpan">postcss.vendor.</span>prefix (prop)](#apidoc.element.postcss.vendor.prefix)
1.  [function <span class="apidocSignatureSpan">postcss.vendor.</span>unprefixed (prop)](#apidoc.element.postcss.vendor.unprefixed)

#### [module postcss.warning](#apidoc.module.postcss.warning)
1.  [function <span class="apidocSignatureSpan">postcss.</span>warning (text)](#apidoc.element.postcss.warning.warning)

#### [module postcss.warning.prototype](#apidoc.module.postcss.warning.prototype)
1.  [function <span class="apidocSignatureSpan">postcss.warning.prototype.</span>toString ()](#apidoc.element.postcss.warning.prototype.toString)



# <a name="apidoc.module.postcss"></a>[module postcss](#apidoc.module.postcss)

#### <a name="apidoc.element.postcss.atRule"></a>[function <span class="apidocSignatureSpan">postcss.</span>atRule (defaults)](#apidoc.element.postcss.atRule)
- description and source-code
```javascript
atRule = function (defaults) {
  return new _atRule2.default(defaults);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.at_rule"></a>[function <span class="apidocSignatureSpan">postcss.</span>at_rule (defaults)](#apidoc.element.postcss.at_rule)
- description and source-code
```javascript
function AtRule(defaults) {
    _classCallCheck(this, AtRule);

    var _this = _possibleConstructorReturn(this, _Container.call(this, defaults));

    _this.type = 'atrule';
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.comment"></a>[function <span class="apidocSignatureSpan">postcss.</span>comment (defaults)](#apidoc.element.postcss.comment)
- description and source-code
```javascript
comment = function (defaults) {
  return new _comment2.default(defaults);
}
```
- example usage
```shell
...
    break;

case '}':
    this.end(token);
    break;

case 'comment':
    this.comment(token);
    break;

case 'at-word':
    this.atrule(token);
    break;

case '{':
...
```

#### <a name="apidoc.element.postcss.container"></a>[function <span class="apidocSignatureSpan">postcss.</span>container ()](#apidoc.element.postcss.container)
- description and source-code
```javascript
function Container() {
    _classCallCheck(this, Container);

    return _possibleConstructorReturn(this, _Node.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.css_syntax_error"></a>[function <span class="apidocSignatureSpan">postcss.</span>css_syntax_error (message, line, column, source, file, plugin)](#apidoc.element.postcss.css_syntax_error)
- description and source-code
```javascript
function CssSyntaxError(message, line, column, source, file, plugin) {
    _classCallCheck(this, CssSyntaxError);

<span class="apidocCodeCommentSpan">    /**
     * @member {string} - Always equal to ''CssSyntaxError''. You should
     *                    always check error type
     *                    by 'error.name === 'CssSyntaxError'' instead of
     *                    'error instanceof CssSyntaxError', because
     *                    npm could have several PostCSS versions.
     *
     * @example
     * if ( error.name === 'CssSyntaxError' ) {
     *   error //=> CssSyntaxError
     * }
     */
</span>    this.name = 'CssSyntaxError';
    /**
     * @member {string} - Error message.
     *
     * @example
     * error.message //=> 'Unclosed block'
     */
    this.reason = message;

    if (file) {
        /**
         * @member {string} - Absolute path to the broken file.
         *
         * @example
         * error.file       //=> 'a.sass'
         * error.input.file //=> 'a.css'
         */
        this.file = file;
    }
    if (source) {
        /**
         * @member {string} - Source code of the broken file.
         *
         * @example
         * error.source       //=> 'a { b {} }'
         * error.input.column //=> 'a b { }'
         */
        this.source = source;
    }
    if (plugin) {
        /**
         * @member {string} - Plugin name, if error came from plugin.
         *
         * @example
         * error.plugin //=> 'postcss-vars'
         */
        this.plugin = plugin;
    }
    if (typeof line !== 'undefined' && typeof column !== 'undefined') {
        /**
         * @member {number} - Source line of the error.
         *
         * @example
         * error.line       //=> 2
         * error.input.line //=> 4
         */
        this.line = line;
        /**
         * @member {number} - Source column of the error.
         *
         * @example
         * error.column       //=> 1
         * error.input.column //=> 4
         */
        this.column = column;
    }

    this.setMessage();

    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, CssSyntaxError);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.decl"></a>[function <span class="apidocSignatureSpan">postcss.</span>decl (defaults)](#apidoc.element.postcss.decl)
- description and source-code
```javascript
decl = function (defaults) {
  return new _declaration2.default(defaults);
}
```
- example usage
```shell
...
* Inserts new nodes to the end of the container.
*
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.append(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
...
```

#### <a name="apidoc.element.postcss.input"></a>[function <span class="apidocSignatureSpan">postcss.</span>input (css)](#apidoc.element.postcss.input)
- description and source-code
```javascript
function Input(css) {
    var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

    _classCallCheck(this, Input);

<span class="apidocCodeCommentSpan">    /**
     * @member {string} - input CSS source
     *
     * @example
     * const input = postcss.parse('a{}', { from: file }).input;
     * input.css //=> "a{}";
     */
</span>    this.css = css.toString();

    if (this.css[0] === '\uFEFF' || this.css[0] === '\uFFFE') {
        this.css = this.css.slice(1);
    }

    if (opts.from) {
        if (/^\w+:\/\//.test(opts.from)) {
            /**
             * @member {string} - The absolute path to the CSS source file
             *                    defined with the 'from' option.
             *
             * @example
             * const root = postcss.parse(css, { from: 'a.css' });
             * root.source.input.file //=> '/home/ai/a.css'
             */
            this.file = opts.from;
        } else {
            this.file = _path2.default.resolve(opts.from);
        }
    }

    var map = new _previousMap2.default(this.css, opts);
    if (map.text) {
        /**
         * @member {PreviousMap} - The input source map passed from
         *                         a compilation step before PostCSS
         *                         (for example, from Sass compiler).
         *
         * @example
         * root.source.input.map.consumer().sources //=> ['a.sass']
         */
        this.map = map;
        var file = map.consumer().file;
        if (!this.file && file) this.file = this.mapResolve(file);
    }

    if (!this.file) {
        sequence += 1;
        /**
         * @member {string} - The unique ID of the CSS source. It will be
         *                    created if 'from' option is not provided
         *                    (because PostCSS does not know the file path).
         *
         * @example
         * const root = postcss.parse(css);
         * root.source.input.file //=> undefined
         * root.source.input.id   //=> "<input css 1>"
         */
        this.id = '<input css ' + sequence + '>';
    }
    if (this.map) this.map.file = this.from;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.lazy_result"></a>[function <span class="apidocSignatureSpan">postcss.</span>lazy_result (processor, css, opts)](#apidoc.element.postcss.lazy_result)
- description and source-code
```javascript
function LazyResult(processor, css, opts) {
    _classCallCheck(this, LazyResult);

    this.stringified = false;
    this.processed = false;

    var root = void 0;
    if ((typeof css === 'undefined' ? 'undefined' : _typeof(css)) === 'object' && css.type === 'root') {
        root = css;
    } else if (css instanceof LazyResult || css instanceof _result2.default) {
        root = css.root;
        if (css.map) {
            if (typeof opts.map === 'undefined') opts.map = {};
            if (!opts.map.inline) opts.map.inline = false;
            opts.map.prev = css.map;
        }
    } else {
        var parser = _parse2.default;
        if (opts.syntax) parser = opts.syntax.parse;
        if (opts.parser) parser = opts.parser;
        if (parser.parse) parser = parser.parse;

        try {
            root = parser(css, opts);
        } catch (error) {
            this.error = error;
        }
    }

    this.result = new _result2.default(processor, root, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.map_generator"></a>[function <span class="apidocSignatureSpan">postcss.</span>map_generator (stringify, root, opts)](#apidoc.element.postcss.map_generator)
- description and source-code
```javascript
function MapGenerator(stringify, root, opts) {
    _classCallCheck(this, MapGenerator);

    this.stringify = stringify;
    this.mapOpts = opts.map || {};
    this.root = root;
    this.opts = opts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node"></a>[function <span class="apidocSignatureSpan">postcss.</span>node ()](#apidoc.element.postcss.node)
- description and source-code
```javascript
function Node() {
    var defaults = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    _classCallCheck(this, Node);

    this.raws = {};
    if ((typeof defaults === 'undefined' ? 'undefined' : _typeof(defaults)) !== 'object' && typeof defaults !== 'undefined') {
        throw new Error('PostCSS nodes constructor accepts object, not ' + JSON.stringify(defaults));
    }
    for (var name in defaults) {
        this[name] = defaults[name];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.parse"></a>[function <span class="apidocSignatureSpan">postcss.</span>parse (css, opts)](#apidoc.element.postcss.parse)
- description and source-code
```javascript
function parse(css, opts) {
    if (opts && opts.safe) {
        throw new Error('Option safe was removed. ' + 'Use parser: require("postcss-safe-parser")');
    }

    var input = new _input2.default(css, opts);

    var parser = new _parser2.default(input);
    try {
        parser.tokenize();
        parser.loop();
    } catch (e) {
        if (e.name === 'CssSyntaxError' && opts && opts.from) {
            if (/\.scss$/i.test(opts.from)) {
                e.message += '\nYou tried to parse SCSS with ' + 'the standard CSS parser; ' + 'try again with the postcss-scss
parser';
            } else if (/\.less$/i.test(opts.from)) {
                e.message += '\nYou tried to parse Less with ' + 'the standard CSS parser; ' + 'try again with the postcss-less
parser';
            }
        }
        throw e;
    }

    return parser.root;
}
```
- example usage
```shell
...
*
* If it’s followed in the CSS by a {} block, this node will have
* a nodes property representing its children.
*
* @extends Container
*
* @example
* const root = postcss.parse('@charset "UTF-8"; @media print {}');
*
* const charset = root.first;
* charset.type  //=> 'atrule'
* charset.nodes //=> undefined
*
* const media = root.last;
* media.nodes   //=> []
...
```

#### <a name="apidoc.element.postcss.parser"></a>[function <span class="apidocSignatureSpan">postcss.</span>parser (input)](#apidoc.element.postcss.parser)
- description and source-code
```javascript
function Parser(input) {
    _classCallCheck(this, Parser);

    this.input = input;

    this.pos = 0;
    this.root = new _root2.default();
    this.current = this.root;
    this.spaces = '';
    this.semicolon = false;

    this.root.source = { input: input, start: { line: 1, column: 1 } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.plugin"></a>[function <span class="apidocSignatureSpan">postcss.</span>plugin (name, initializer)](#apidoc.element.postcss.plugin)
- description and source-code
```javascript
function plugin(name, initializer) {
  var creator = function creator() {
    var transformer = initializer.apply(undefined, arguments);
    transformer.postcssPlugin = name;
    transformer.postcssVersion = new _processor2.default().version;
    return transformer;
  };

  var cache = void 0;
  Object.defineProperty(creator, 'postcss', {
    get: function get() {
      if (!cache) cache = creator();
      return cache;
    }
  });

  creator.process = function (root, opts) {
    return postcss([creator(opts)]).process(root, opts);
  };

  return creator;
}
```
- example usage
```shell
...
*                               be highlighted as the source of the warning
* @param {number} opts.index  - an index inside a node’s string that should
*                               be highlighted as the source of the warning
*
* @return {Warning} created warning object
*
* @example
* const plugin = postcss.plugin('postcss-deprecated', () => {
*   return (root, result) => {
*     root.walkDecls('bad', decl => {
*       decl.warn(result, 'Deprecated property bad');
*     });
*   };
* });
*/
...
```

#### <a name="apidoc.element.postcss.previous_map"></a>[function <span class="apidocSignatureSpan">postcss.</span>previous_map (css, opts)](#apidoc.element.postcss.previous_map)
- description and source-code
```javascript
function PreviousMap(css, opts) {
    _classCallCheck(this, PreviousMap);

    this.loadAnnotation(css);
<span class="apidocCodeCommentSpan">    /**
     * @member {boolean} - Was source map inlined by data-uri to input CSS.
     */
</span>    this.inline = this.startWith(this.annotation, 'data:');

    var prev = opts.map ? opts.map.prev : undefined;
    var text = this.loadMap(opts.from, prev);
    if (text) this.text = text;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.processor"></a>[function <span class="apidocSignatureSpan">postcss.</span>processor ()](#apidoc.element.postcss.processor)
- description and source-code
```javascript
function Processor() {
  var plugins = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : [];

  _classCallCheck(this, Processor);

<span class="apidocCodeCommentSpan">  /**
   * @member {string} - Current PostCSS version.
   *
   * @example
   * if ( result.processor.version.split('.')[0] !== '5' ) {
   *   throw new Error('This plugin works only with PostCSS 5');
   * }
   */
</span>  this.version = '5.2.16';
  /**
   * @member {pluginFunction[]} - Plugins added to this processor.
   *
   * @example
   * const processor = postcss([autoprefixer, precss]);
   * processor.plugins.length //=> 2
   */
  this.plugins = this.normalize(plugins);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.result"></a>[function <span class="apidocSignatureSpan">postcss.</span>result (processor, root, opts)](#apidoc.element.postcss.result)
- description and source-code
```javascript
function Result(processor, root, opts) {
  _classCallCheck(this, Result);

<span class="apidocCodeCommentSpan">  /**
   * @member {Processor} - The Processor instance used
   *                       for this transformation.
   *
   * @example
   * for ( let plugin of result.processor.plugins) {
   *   if ( plugin.postcssPlugin === 'postcss-bad' ) {
   *     throw 'postcss-good is incompatible with postcss-bad';
   *   }
   * });
   */
</span>  this.processor = processor;
  /**
   * @member {Message[]} - Contains messages from plugins
   *                       (e.g., warnings or custom messages).
   *                       Each message should have type
   *                       and plugin properties.
   *
   * @example
   * postcss.plugin('postcss-min-browser', () => {
   *   return (root, result) => {
   *     var browsers = detectMinBrowsersByCanIUse(root);
   *     result.messages.push({
   *       type:    'min-browser',
   *       plugin:  'postcss-min-browser',
   *       browsers: browsers
   *     });
   *   };
   * });
   */
  this.messages = [];
  /**
   * @member {Root} - Root node after all transformations.
   *
   * @example
   * root.toResult().root == root;
   */
  this.root = root;
  /**
   * @member {processOptions} - Options from the {@link Processor#process}
   *                            or {@link Root#toResult} call
   *                            that produced this Result instance.
   *
   * @example
   * root.toResult(opts).opts == opts;
   */
  this.opts = opts;
  /**
   * @member {string} - A CSS string representing of {@link Result#root}.
   *
   * @example
   * postcss.parse('a{}').toResult().css //=> "a{}"
   */
  this.css = undefined;
  /**
   * @member {SourceMapGenerator} - An instance of 'SourceMapGenerator'
   *                                class from the 'source-map' library,
   *                                representing changes
   *                                to the {@link Result#root} instance.
   *
   * @example
   * result.map.toJSON() //=> { version: 3, file: 'a.css', … }
   *
   * @example
   * if ( result.map ) {
   *   fs.writeFileSync(result.opts.to + '.map', result.map.toString());
   * }
   */
  this.map = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.root"></a>[function <span class="apidocSignatureSpan">postcss.</span>root (defaults)](#apidoc.element.postcss.root)
- description and source-code
```javascript
root = function (defaults) {
  return new _root2.default(defaults);
}
```
- example usage
```shell
...
 * It will also clean the 'between' property
 * if 'newParent' is in another {@link Root}.
 *
 * @param {Container} newParent - container node where the current node
 *                                will be moved
 *
 * @example
 * atrule.moveTo(atrule.root());
 *
 * @return {Node} current node to methods chain
 */


Node.prototype.moveTo = function moveTo(newParent) {
    this.cleanRaws(this.root() === newParent.root());
...
```

#### <a name="apidoc.element.postcss.rule"></a>[function <span class="apidocSignatureSpan">postcss.</span>rule (defaults)](#apidoc.element.postcss.rule)
- description and source-code
```javascript
rule = function (defaults) {
  return new _rule2.default(defaults);
}
```
- example usage
```shell
...
     *
     * @param {stringifier|syntax} [stringifier] - a syntax to use
     *                                             in string generation
     *
     * @return {string} CSS string of this node
     *
     * @example
     * postcss.rule({ selector: 'a' }).toString() //=> "a {}"
     */


    Node.prototype.toString = function toString() {
var stringifier = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : _stringify2.default;

if (stringifier.stringify) stringifier = stringifier.stringify;
...
```

#### <a name="apidoc.element.postcss.stringifier"></a>[function <span class="apidocSignatureSpan">postcss.</span>stringifier (builder)](#apidoc.element.postcss.stringifier)
- description and source-code
```javascript
function Stringifier(builder) {
    _classCallCheck(this, Stringifier);

    this.builder = builder;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringify"></a>[function <span class="apidocSignatureSpan">postcss.</span>stringify (node, builder)](#apidoc.element.postcss.stringify)
- description and source-code
```javascript
function stringify(node, builder) {
    var str = new _stringifier2.default(builder);
    str.stringify(node);
}
```
- example usage
```shell
...
var _this2 = this;

if (this.processed) {
    return new Promise(function (resolve, reject) {
        if (_this2.error) {
            reject(_this2.error);
        } else {
            resolve(_this2.stringify());
        }
    });
}
if (this.processing) {
    return this.processing;
}
...
```

#### <a name="apidoc.element.postcss.warning"></a>[function <span class="apidocSignatureSpan">postcss.</span>warning (text)](#apidoc.element.postcss.warning)
- description and source-code
```javascript
function Warning(text) {
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  _classCallCheck(this, Warning);

<span class="apidocCodeCommentSpan">  /**
   * @member {string} - Type to filter warnings from
   *                    {@link Result#messages}. Always equal
   *                    to '"warning"'.
   *
   * @example
   * const nonWarning = result.messages.filter(i => i.type !== 'warning')
   */
</span>  this.type = 'warning';
  /**
   * @member {string} - The warning message.
   *
   * @example
   * warning.text //=> 'Try to avoid !important'
   */
  this.text = text;

  if (opts.node && opts.node.source) {
    var pos = opts.node.positionBy(opts);
    /**
     * @member {number} - Line in the input file
     *                    with this warning’s source
     *
     * @example
     * warning.line //=> 5
     */
    this.line = pos.line;
    /**
     * @member {number} - Column in the input file
     *                    with this warning’s source.
     *
     * @example
     * warning.column //=> 6
     */
    this.column = pos.column;
  }

  for (var opt in opts) {
    this[opt] = opts[opt];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.at_rule"></a>[module postcss.at_rule](#apidoc.module.postcss.at_rule)

#### <a name="apidoc.element.postcss.at_rule.at_rule"></a>[function <span class="apidocSignatureSpan">postcss.</span>at_rule (defaults)](#apidoc.element.postcss.at_rule.at_rule)
- description and source-code
```javascript
function AtRule(defaults) {
    _classCallCheck(this, AtRule);

    var _this = _possibleConstructorReturn(this, _Container.call(this, defaults));

    _this.type = 'atrule';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.at_rule.prototype"></a>[module postcss.at_rule.prototype](#apidoc.module.postcss.at_rule.prototype)

#### <a name="apidoc.element.postcss.at_rule.prototype.append"></a>[function <span class="apidocSignatureSpan">postcss.at_rule.prototype.</span>append ()](#apidoc.element.postcss.at_rule.prototype.append)
- description and source-code
```javascript
function append() {
    var _Container$prototype$;

    if (!this.nodes) this.nodes = [];

    for (var _len = arguments.length, children = Array(_len), _key = 0; _key < _len; _key++) {
        children[_key] = arguments[_key];
    }

    return (_Container$prototype$ = _Container.prototype.append).call.apply(_Container$prototype$, [this].concat(children));
}
```
- example usage
```shell
...
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.append(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
*
* root.append('a {}');
...
```

#### <a name="apidoc.element.postcss.at_rule.prototype.prepend"></a>[function <span class="apidocSignatureSpan">postcss.at_rule.prototype.</span>prepend ()](#apidoc.element.postcss.at_rule.prototype.prepend)
- description and source-code
```javascript
function prepend() {
    var _Container$prototype$2;

    if (!this.nodes) this.nodes = [];

    for (var _len2 = arguments.length, children = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
        children[_key2] = arguments[_key2];
    }

    return (_Container$prototype$2 = _Container.prototype.prepend).call.apply(_Container$prototype$2, [this].concat(children));
}
```
- example usage
```shell
...
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.prepend(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
*
* root.append('a {}');
...
```



# <a name="apidoc.module.postcss.container"></a>[module postcss.container](#apidoc.module.postcss.container)

#### <a name="apidoc.element.postcss.container.container"></a>[function <span class="apidocSignatureSpan">postcss.</span>container ()](#apidoc.element.postcss.container.container)
- description and source-code
```javascript
function Container() {
    _classCallCheck(this, Container);

    return _possibleConstructorReturn(this, _Node.apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.container.prototype"></a>[module postcss.container.prototype](#apidoc.module.postcss.container.prototype)

#### <a name="apidoc.element.postcss.container.prototype.append"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>append ()](#apidoc.element.postcss.container.prototype.append)
- description and source-code
```javascript
function append() {
    for (var _len = arguments.length, children = Array(_len), _key = 0; _key < _len; _key++) {
        children[_key] = arguments[_key];
    }

    for (var _iterator = children, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator[Symbol
.iterator]();;) {
        var _ref;

        if (_isArray) {
            if (_i >= _iterator.length) break;
            _ref = _iterator[_i++];
        } else {
            _i = _iterator.next();
            if (_i.done) break;
            _ref = _i.value;
        }

        var child = _ref;

        var nodes = this.normalize(child, this.last);
        for (var _iterator2 = nodes, _isArray2 = Array.isArray(_iterator2), _i2 = 0, _iterator2 = _isArray2 ? _iterator2 : _iterator2
[Symbol.iterator]();;) {
            var _ref2;

            if (_isArray2) {
                if (_i2 >= _iterator2.length) break;
                _ref2 = _iterator2[_i2++];
            } else {
                _i2 = _iterator2.next();
                if (_i2.done) break;
                _ref2 = _i2.value;
            }

            var node = _ref2;
            this.nodes.push(node);
        }
    }
    return this;
}
```
- example usage
```shell
...
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.append(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
*
* root.append('a {}');
...
```

#### <a name="apidoc.element.postcss.container.prototype.cleanRaws"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>cleanRaws (keepBetween)](#apidoc.element.postcss.container.prototype.cleanRaws)
- description and source-code
```javascript
function cleanRaws(keepBetween) {
    _Node.prototype.cleanRaws.call(this, keepBetween);
    if (this.nodes) {
        for (var _iterator5 = this.nodes, _isArray5 = Array.isArray(_iterator5), _i5 = 0, _iterator5 = _isArray5 ? _iterator5 :
_iterator5[Symbol.iterator]();;) {
            var _ref5;

            if (_isArray5) {
                if (_i5 >= _iterator5.length) break;
                _ref5 = _iterator5[_i5++];
            } else {
                _i5 = _iterator5.next();
                if (_i5.done) break;
                _ref5 = _i5.value;
            }

            var node = _ref5;
            node.cleanRaws(keepBetween);
        }
    }
}
```
- example usage
```shell
...
            } else {
                _i5 = _iterator5.next();
                if (_i5.done) break;
                _ref5 = _i5.value;
            }

            var node = _ref5;
            node.cleanRaws(keepBetween);
        }
    }
};

/**
 * Insert new node before old node within the container.
 *
...
```

#### <a name="apidoc.element.postcss.container.prototype.each"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>each (callback)](#apidoc.element.postcss.container.prototype.each)
- description and source-code
```javascript
function each(callback) {
    if (!this.lastEach) this.lastEach = 0;
    if (!this.indexes) this.indexes = {};

    this.lastEach += 1;
    var id = this.lastEach;
    this.indexes[id] = 0;

    if (!this.nodes) return undefined;

    var index = void 0,
        result = void 0;
    while (this.indexes[id] < this.nodes.length) {
        index = this.indexes[id];
        result = callback(this.nodes[index], index);
        if (result === false) break;

        this.indexes[id] += 1;
    }

    delete this.indexes[id];

    return result;
}
```
- example usage
```shell
...
 *
 * for ( let decl of rule.nodes ) {
 *     decl.cloneBefore({ prop: '-webkit-' + decl.prop });
 *     // Cycle will be infinite, because cloneBefore moves the current node
 *     // to the next index
 * }
 *
 * rule.each(decl => {
 *     decl.cloneBefore({ prop: '-webkit-' + decl.prop });
 *     // Will be executed only for color and z-index
 * });
 */


Container.prototype.each = function each(callback) {
...
```

#### <a name="apidoc.element.postcss.container.prototype.eachAtRule"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachAtRule (name, callback)](#apidoc.element.postcss.container.prototype.eachAtRule)
- description and source-code
```javascript
function eachAtRule(name, callback) {
    (0, _warnOnce2.default)('Container#eachAtRule is deprecated. ' + 'Use Container#walkAtRules instead.');
    return this.walkAtRules(name, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.container.prototype.eachComment"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachComment (callback)](#apidoc.element.postcss.container.prototype.eachComment)
- description and source-code
```javascript
function eachComment(callback) {
    (0, _warnOnce2.default)('Container#eachComment is deprecated. ' + 'Use Container#walkComments instead.');
    return this.walkComments(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.container.prototype.eachDecl"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachDecl (prop, callback)](#apidoc.element.postcss.container.prototype.eachDecl)
- description and source-code
```javascript
function eachDecl(prop, callback) {
    (0, _warnOnce2.default)('Container#eachDecl is deprecated. ' + 'Use Container#walkDecls instead.');
    return this.walkDecls(prop, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.container.prototype.eachInside"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachInside (callback)](#apidoc.element.postcss.container.prototype.eachInside)
- description and source-code
```javascript
function eachInside(callback) {
    (0, _warnOnce2.default)('Container#eachInside is deprecated. ' + 'Use Container#walk instead.');
    return this.walk(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.container.prototype.eachRule"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>eachRule (selector, callback)](#apidoc.element.postcss.container.prototype.eachRule)
- description and source-code
```javascript
function eachRule(selector, callback) {
    (0, _warnOnce2.default)('Container#eachRule is deprecated. ' + 'Use Container#walkRules instead.');
    return this.walkRules(selector, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.container.prototype.every"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>every (condition)](#apidoc.element.postcss.container.prototype.every)
- description and source-code
```javascript
function every(condition) {
    return this.nodes.every(condition);
}
```
- example usage
```shell
...
 * for all of the container’s children.
 *
 * @param {childCondition} condition - iterator returns true or false.
 *
 * @return {boolean} is every child pass condition
 *
 * @example
 * const noPrefixes = rule.every(i => i.prop[0] !== '-');
 */


Container.prototype.every = function every(condition) {
    return this.nodes.every(condition);
};
...
```

#### <a name="apidoc.element.postcss.container.prototype.index"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>index (child)](#apidoc.element.postcss.container.prototype.index)
- description and source-code
```javascript
function index(child) {
    if (typeof child === 'number') {
        return child;
    } else {
        return this.nodes.indexOf(child);
    }
}
```
- example usage
```shell
...
     *
     * @example
     * rule.insertBefore(decl, decl.clone({ prop: '-webkit-' + decl.prop }));
     */


    Container.prototype.insertBefore = function insertBefore(exist, add) {
        exist = this.index(exist);

        var type = exist === 0 ? 'prepend' : false;
        var nodes = this.normalize(add, this.nodes[exist], type).reverse();
        for (var _iterator6 = nodes, _isArray6 = Array.isArray(_iterator6), _i6 = 0, _iterator6 = _isArray6 ? _iterator6 : _iterator6
[Symbol.iterator]();;) {
var _ref6;

if (_isArray6) {
...
```

#### <a name="apidoc.element.postcss.container.prototype.insertAfter"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>insertAfter (exist, add)](#apidoc.element.postcss.container.prototype.insertAfter)
- description and source-code
```javascript
function insertAfter(exist, add) {
    exist = this.index(exist);

    var nodes = this.normalize(add, this.nodes[exist]).reverse();
    for (var _iterator7 = nodes, _isArray7 = Array.isArray(_iterator7), _i7 = 0, _iterator7 = _isArray7 ? _iterator7 : _iterator7
[Symbol.iterator]();;) {
        var _ref7;

        if (_isArray7) {
            if (_i7 >= _iterator7.length) break;
            _ref7 = _iterator7[_i7++];
        } else {
            _i7 = _iterator7.next();
            if (_i7.done) break;
            _ref7 = _i7.value;
        }

        var node = _ref7;
        this.nodes.splice(exist + 1, 0, node);
    }var index = void 0;
    for (var id in this.indexes) {
        index = this.indexes[id];
        if (exist < index) {
            this.indexes[id] = index + nodes.length;
        }
    }

    return this;
}
```
- example usage
```shell
...
 */


Node.prototype.cloneAfter = function cloneAfter() {
    var overrides = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    var cloned = this.clone(overrides);
    this.parent.insertAfter(this, cloned);
    return cloned;
};

/**
 * Inserts node(s) before the current node and removes the current node.
 *
 * @param {...Node} nodes - node(s) to replace current one
...
```

#### <a name="apidoc.element.postcss.container.prototype.insertBefore"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>insertBefore (exist, add)](#apidoc.element.postcss.container.prototype.insertBefore)
- description and source-code
```javascript
function insertBefore(exist, add) {
    exist = this.index(exist);

    var type = exist === 0 ? 'prepend' : false;
    var nodes = this.normalize(add, this.nodes[exist], type).reverse();
    for (var _iterator6 = nodes, _isArray6 = Array.isArray(_iterator6), _i6 = 0, _iterator6 = _isArray6 ? _iterator6 : _iterator6
[Symbol.iterator]();;) {
        var _ref6;

        if (_isArray6) {
            if (_i6 >= _iterator6.length) break;
            _ref6 = _iterator6[_i6++];
        } else {
            _i6 = _iterator6.next();
            if (_i6.done) break;
            _ref6 = _i6.value;
        }

        var node = _ref6;
        this.nodes.splice(exist, 0, node);
    }var index = void 0;
    for (var id in this.indexes) {
        index = this.indexes[id];
        if (exist <= index) {
            this.indexes[id] = index + nodes.length;
        }
    }

    return this;
}
```
- example usage
```shell
...
     *
     * @param {Node|number} exist             - child or child’s index.
     * @param {Node|object|string|Node[]} add - new node
     *
     * @return {Node} this node for methods chain
     *
     * @example
     * rule.insertBefore(decl, decl.clone({ prop: '-webkit-' + decl.prop }));
     */


    Container.prototype.insertBefore = function insertBefore(exist, add) {
exist = this.index(exist);

var type = exist === 0 ? 'prepend' : false;
...
```

#### <a name="apidoc.element.postcss.container.prototype.normalize"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>normalize (nodes, sample)](#apidoc.element.postcss.container.prototype.normalize)
- description and source-code
```javascript
function normalize(nodes, sample) {
    var _this2 = this;

    if (typeof nodes === 'string') {
        var parse = require('./parse');
        nodes = cleanSource(parse(nodes).nodes);
    } else if (!Array.isArray(nodes)) {
        if (nodes.type === 'root') {
            nodes = nodes.nodes;
        } else if (nodes.type) {
            nodes = [nodes];
        } else if (nodes.prop) {
            if (typeof nodes.value === 'undefined') {
                throw new Error('Value field is missed in node creation');
            } else if (typeof nodes.value !== 'string') {
                nodes.value = String(nodes.value);
            }
            nodes = [new _declaration2.default(nodes)];
        } else if (nodes.selector) {
            var Rule = require('./rule');
            nodes = [new Rule(nodes)];
        } else if (nodes.name) {
            var AtRule = require('./at-rule');
            nodes = [new AtRule(nodes)];
        } else if (nodes.text) {
            nodes = [new _comment2.default(nodes)];
        } else {
            throw new Error('Unknown node type in node creation');
        }
    }

    var processed = nodes.map(function (i) {
        if (typeof i.raws === 'undefined') i = _this2.rebuild(i);

        if (i.parent) i = i.clone();
        if (typeof i.raws.before === 'undefined') {
            if (sample && typeof sample.raws.before !== 'undefined') {
                i.raws.before = sample.raws.before.replace(/[^\s]/g, '');
            }
        }
        i.parent = _this2;
        return i;
    });

    return processed;
}
```
- example usage
```shell
...
_i = _iterator.next();
if (_i.done) break;
_ref = _i.value;
            }

            var child = _ref;

            var nodes = this.normalize(child, this.last);
            for (var _iterator2 = nodes, _isArray2 = Array.isArray(_iterator2), _i2 = 0, _iterator2 = _isArray2 ? _iterator2 : _iterator2
[Symbol.iterator]();;) {
var _ref2;

if (_isArray2) {
    if (_i2 >= _iterator2.length) break;
    _ref2 = _iterator2[_i2++];
} else {
...
```

#### <a name="apidoc.element.postcss.container.prototype.prepend"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>prepend ()](#apidoc.element.postcss.container.prototype.prepend)
- description and source-code
```javascript
function prepend() {
    for (var _len2 = arguments.length, children = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
        children[_key2] = arguments[_key2];
    }

    children = children.reverse();
    for (var _iterator3 = children, _isArray3 = Array.isArray(_iterator3), _i3 = 0, _iterator3 = _isArray3 ? _iterator3 : _iterator3
[Symbol.iterator]();;) {
        var _ref3;

        if (_isArray3) {
            if (_i3 >= _iterator3.length) break;
            _ref3 = _iterator3[_i3++];
        } else {
            _i3 = _iterator3.next();
            if (_i3.done) break;
            _ref3 = _i3.value;
        }

        var child = _ref3;

        var nodes = this.normalize(child, this.first, 'prepend').reverse();
        for (var _iterator4 = nodes, _isArray4 = Array.isArray(_iterator4), _i4 = 0, _iterator4 = _isArray4 ? _iterator4 : _iterator4
[Symbol.iterator]();;) {
            var _ref4;

            if (_isArray4) {
                if (_i4 >= _iterator4.length) break;
                _ref4 = _iterator4[_i4++];
            } else {
                _i4 = _iterator4.next();
                if (_i4.done) break;
                _ref4 = _i4.value;
            }

            var node = _ref4;
            this.nodes.unshift(node);
        }for (var id in this.indexes) {
            this.indexes[id] = this.indexes[id] + nodes.length;
        }
    }
    return this;
}
```
- example usage
```shell
...
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.prepend(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
*
* root.append('a {}');
...
```

#### <a name="apidoc.element.postcss.container.prototype.push"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>push (child)](#apidoc.element.postcss.container.prototype.push)
- description and source-code
```javascript
function push(child) {
    child.parent = this;
    this.nodes.push(child);
    return this;
}
```
- example usage
```shell
...
    _classCallCheck(this, Container);

    return _possibleConstructorReturn(this, _Node.apply(this, arguments));
}

Container.prototype.push = function push(child) {
    child.parent = this;
    this.nodes.push(child);
    return this;
};

/**
 * Iterates through the container’s immediate children,
 * calling 'callback' for each child.
 *
...
```

#### <a name="apidoc.element.postcss.container.prototype.rebuild"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>rebuild (node, parent)](#apidoc.element.postcss.container.prototype.rebuild)
- description and source-code
```javascript
function rebuild(node, parent) {
    var _this3 = this;

    var fix = void 0;
    if (node.type === 'root') {
        var Root = require('./root');
        fix = new Root();
    } else if (node.type === 'atrule') {
        var AtRule = require('./at-rule');
        fix = new AtRule();
    } else if (node.type === 'rule') {
        var Rule = require('./rule');
        fix = new Rule();
    } else if (node.type === 'decl') {
        fix = new _declaration2.default();
    } else if (node.type === 'comment') {
        fix = new _comment2.default();
    }

    for (var i in node) {
        if (i === 'nodes') {
            fix.nodes = node.nodes.map(function (j) {
                return _this3.rebuild(j, fix);
            });
        } else if (i === 'parent' && parent) {
            fix.parent = parent;
        } else if (node.hasOwnProperty(i)) {
            fix[i] = node[i];
        }
    }

    return fix;
}
```
- example usage
```shell
...
    nodes = [new _comment2.default(nodes)];
} else {
    throw new Error('Unknown node type in node creation');
}
        }

        var processed = nodes.map(function (i) {
if (typeof i.raws === 'undefined') i = _this2.rebuild(i);

if (i.parent) i = i.clone();
if (typeof i.raws.before === 'undefined') {
    if (sample && typeof sample.raws.before !== 'undefined') {
        i.raws.before = sample.raws.before.replace(/[^\s]/g, '');
    }
}
...
```

#### <a name="apidoc.element.postcss.container.prototype.remove"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>remove (child)](#apidoc.element.postcss.container.prototype.remove)
- description and source-code
```javascript
function remove(child) {
    if (typeof child !== 'undefined') {
        (0, _warnOnce2.default)('Container#remove is deprecated. ' + 'Use Container#removeChild');
        this.removeChild(child);
    } else {
        _Node.prototype.remove.call(this);
    }
    return this;
}
```
- example usage
```shell
...
*
* @example
* root.walkDecls(decl => {
*   checkPropertySupport(decl.prop);
* });
*
* root.walkDecls('border-radius', decl => {
*   decl.remove();
* });
*
* root.walkDecls(/^background/, decl => {
*   decl.value = takeFirstColorFromGradient(decl.value);
* });
*/
...
```

#### <a name="apidoc.element.postcss.container.prototype.removeAll"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>removeAll ()](#apidoc.element.postcss.container.prototype.removeAll)
- description and source-code
```javascript
function removeAll() {
    for (var _iterator8 = this.nodes, _isArray8 = Array.isArray(_iterator8), _i8 = 0, _iterator8 = _isArray8 ? _iterator8 : _iterator8
[Symbol.iterator]();;) {
        var _ref8;

        if (_isArray8) {
            if (_i8 >= _iterator8.length) break;
            _ref8 = _iterator8[_i8++];
        } else {
            _i8 = _iterator8.next();
            if (_i8.done) break;
            _ref8 = _i8.value;
        }

        var node = _ref8;
        node.parent = undefined;
    }this.nodes = [];
    return this;
}
```
- example usage
```shell
...
/**
 * Removes all children from the container
 * and cleans their parent properties.
 *
 * @return {Node} this node for methods chain
 *
 * @example
 * rule.removeAll();
 * rule.nodes.length //=> 0
 */


Container.prototype.removeAll = function removeAll() {
    for (var _iterator8 = this.nodes, _isArray8 = Array.isArray(_iterator8), _i8 = 0, _iterator8 = _isArray8 ? _iterator8 : _iterator8
[Symbol.iterator]();;) {
        var _ref8;
...
```

#### <a name="apidoc.element.postcss.container.prototype.removeChild"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>removeChild (child)](#apidoc.element.postcss.container.prototype.removeChild)
- description and source-code
```javascript
function removeChild(child) {
    child = this.index(child);
    this.nodes[child].parent = undefined;
    this.nodes.splice(child, 1);

    var index = void 0;
    for (var id in this.indexes) {
        index = this.indexes[id];
        if (index >= child) {
            this.indexes[id] = index - 1;
        }
    }

    return this;
}
```
- example usage
```shell
...

    return this;
};

Container.prototype.remove = function remove(child) {
    if (typeof child !== 'undefined') {
        (0, _warnOnce2.default)('Container#remove is deprecated. ' + 'Use Container#removeChild');
        this.removeChild(child);
    } else {
        _Node.prototype.remove.call(this);
    }
    return this;
};

/**
...
```

#### <a name="apidoc.element.postcss.container.prototype.replaceValues"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>replaceValues (pattern, opts, callback)](#apidoc.element.postcss.container.prototype.replaceValues)
- description and source-code
```javascript
function replaceValues(pattern, opts, callback) {
    if (!callback) {
        callback = opts;
        opts = {};
    }

    this.walkDecls(function (decl) {
        if (opts.props && opts.props.indexOf(decl.prop) === -1) return;
        if (opts.fast && decl.value.indexOf(opts.fast) === -1) return;

        decl.value = decl.value.replace(pattern, callback);
    });

    return this;
}
```
- example usage
```shell
...
 *                                       the same arguments as those
 *                                       passed to a function parameter
 *                                       of 'String#replace'.
 *
 * @return {Node} this node for methods chain
 *
 * @example
 * root.replaceValues(/\d+rem/, { fast: 'rem' }, string => {
 *   return 15 * parseInt(string) + 'px';
 * });
 */


Container.prototype.replaceValues = function replaceValues(pattern, opts, callback) {
    if (!callback) {
...
```

#### <a name="apidoc.element.postcss.container.prototype.some"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>some (condition)](#apidoc.element.postcss.container.prototype.some)
- description and source-code
```javascript
function some(condition) {
    return this.nodes.some(condition);
}
```
- example usage
```shell
...
 * of the container’s children.
 *
 * @param {childCondition} condition - iterator returns true or false.
 *
 * @return {boolean} is some child pass condition
 *
 * @example
 * const hasPrefix = rule.some(i => i.prop[0] === '-');
 */


Container.prototype.some = function some(condition) {
    return this.nodes.some(condition);
};
...
```

#### <a name="apidoc.element.postcss.container.prototype.walk"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walk (callback)](#apidoc.element.postcss.container.prototype.walk)
- description and source-code
```javascript
function walk(callback) {
    return this.each(function (child, i) {
        var result = callback(child, i);
        if (result !== false && child.walk) {
            result = child.walk(callback);
        }
        return result;
    });
}
```
- example usage
```shell
...
 * use {@link Container#each}.
 *
 * @param {childIterator} callback - iterator receives each node and index
 *
 * @return {false|undefined} returns 'false' if iteration was broke
 *
 * @example
 * root.walk(node => {
 *   // Traverses all descendant nodes.
 * });
 */


Container.prototype.walk = function walk(callback) {
    return this.each(function (child, i) {
...
```

#### <a name="apidoc.element.postcss.container.prototype.walkAtRules"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkAtRules (name, callback)](#apidoc.element.postcss.container.prototype.walkAtRules)
- description and source-code
```javascript
function walkAtRules(name, callback) {
    if (!callback) {
        callback = name;
        return this.walk(function (child, i) {
            if (child.type === 'atrule') {
                return callback(child, i);
            }
        });
    } else if (name instanceof RegExp) {
        return this.walk(function (child, i) {
            if (child.type === 'atrule' && name.test(child.name)) {
                return callback(child, i);
            }
        });
    } else {
        return this.walk(function (child, i) {
            if (child.type === 'atrule' && child.name === name) {
                return callback(child, i);
            }
        });
    }
}
```
- example usage
```shell
...
* @param {string|RegExp} [name]   - string or regular expression
*                                   to filter at-rules by name
* @param {childIterator} callback - iterator receives each node and index
*
* @return {false|undefined} returns 'false' if iteration was broke
*
* @example
* root.walkAtRules(rule => {
*   if ( isOld(rule.name) ) rule.remove();
* });
*
* let first = false;
* root.walkAtRules('charset', rule => {
*   if ( !first ) {
*     first = true;
...
```

#### <a name="apidoc.element.postcss.container.prototype.walkComments"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkComments (callback)](#apidoc.element.postcss.container.prototype.walkComments)
- description and source-code
```javascript
function walkComments(callback) {
    return this.walk(function (child, i) {
        if (child.type === 'comment') {
            return callback(child, i);
        }
    });
}
```
- example usage
```shell
...
 * to use if you are mutating arrays during iteration.
 *
 * @param {childIterator} callback - iterator receives each node and index
 *
 * @return {false|undefined} returns 'false' if iteration was broke
 *
 * @example
 * root.walkComments(comment => {
 *   comment.remove();
 * });
 */


Container.prototype.walkComments = function walkComments(callback) {
    return this.walk(function (child, i) {
...
```

#### <a name="apidoc.element.postcss.container.prototype.walkDecls"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkDecls (prop, callback)](#apidoc.element.postcss.container.prototype.walkDecls)
- description and source-code
```javascript
function walkDecls(prop, callback) {
    if (!callback) {
        callback = prop;
        return this.walk(function (child, i) {
            if (child.type === 'decl') {
                return callback(child, i);
            }
        });
    } else if (prop instanceof RegExp) {
        return this.walk(function (child, i) {
            if (child.type === 'decl' && prop.test(child.prop)) {
                return callback(child, i);
            }
        });
    } else {
        return this.walk(function (child, i) {
            if (child.type === 'decl' && child.prop === prop) {
                return callback(child, i);
            }
        });
    }
}
```
- example usage
```shell
...
* @param {string|RegExp} [prop]   - string or regular expression
*                                   to filter declarations by property name
* @param {childIterator} callback - iterator receives each node and index
*
* @return {false|undefined} returns 'false' if iteration was broke
*
* @example
* root.walkDecls(decl => {
*   checkPropertySupport(decl.prop);
* });
*
* root.walkDecls('border-radius', decl => {
*   decl.remove();
* });
*
...
```

#### <a name="apidoc.element.postcss.container.prototype.walkRules"></a>[function <span class="apidocSignatureSpan">postcss.container.prototype.</span>walkRules (selector, callback)](#apidoc.element.postcss.container.prototype.walkRules)
- description and source-code
```javascript
function walkRules(selector, callback) {
    if (!callback) {
        callback = selector;

        return this.walk(function (child, i) {
            if (child.type === 'rule') {
                return callback(child, i);
            }
        });
    } else if (selector instanceof RegExp) {
        return this.walk(function (child, i) {
            if (child.type === 'rule' && selector.test(child.selector)) {
                return callback(child, i);
            }
        });
    } else {
        return this.walk(function (child, i) {
            if (child.type === 'rule' && child.selector === selector) {
                return callback(child, i);
            }
        });
    }
}
```
- example usage
```shell
...
 *                                     to filter rules by selector
 * @param {childIterator} callback   - iterator receives each node and index
 *
 * @return {false|undefined} returns 'false' if iteration was broke
 *
 * @example
 * const selectors = [];
 * root.walkRules(rule => {
 *   selectors.push(rule.selector);
 * });
 * console.log('Your CSS uses ${selectors.length} selectors');
 */


Container.prototype.walkRules = function walkRules(selector, callback) {
...
```



# <a name="apidoc.module.postcss.css_syntax_error"></a>[module postcss.css_syntax_error](#apidoc.module.postcss.css_syntax_error)

#### <a name="apidoc.element.postcss.css_syntax_error.css_syntax_error"></a>[function <span class="apidocSignatureSpan">postcss.</span>css_syntax_error (message, line, column, source, file, plugin)](#apidoc.element.postcss.css_syntax_error.css_syntax_error)
- description and source-code
```javascript
function CssSyntaxError(message, line, column, source, file, plugin) {
    _classCallCheck(this, CssSyntaxError);

<span class="apidocCodeCommentSpan">    /**
     * @member {string} - Always equal to ''CssSyntaxError''. You should
     *                    always check error type
     *                    by 'error.name === 'CssSyntaxError'' instead of
     *                    'error instanceof CssSyntaxError', because
     *                    npm could have several PostCSS versions.
     *
     * @example
     * if ( error.name === 'CssSyntaxError' ) {
     *   error //=> CssSyntaxError
     * }
     */
</span>    this.name = 'CssSyntaxError';
    /**
     * @member {string} - Error message.
     *
     * @example
     * error.message //=> 'Unclosed block'
     */
    this.reason = message;

    if (file) {
        /**
         * @member {string} - Absolute path to the broken file.
         *
         * @example
         * error.file       //=> 'a.sass'
         * error.input.file //=> 'a.css'
         */
        this.file = file;
    }
    if (source) {
        /**
         * @member {string} - Source code of the broken file.
         *
         * @example
         * error.source       //=> 'a { b {} }'
         * error.input.column //=> 'a b { }'
         */
        this.source = source;
    }
    if (plugin) {
        /**
         * @member {string} - Plugin name, if error came from plugin.
         *
         * @example
         * error.plugin //=> 'postcss-vars'
         */
        this.plugin = plugin;
    }
    if (typeof line !== 'undefined' && typeof column !== 'undefined') {
        /**
         * @member {number} - Source line of the error.
         *
         * @example
         * error.line       //=> 2
         * error.input.line //=> 4
         */
        this.line = line;
        /**
         * @member {number} - Source column of the error.
         *
         * @example
         * error.column       //=> 1
         * error.input.column //=> 4
         */
        this.column = column;
    }

    this.setMessage();

    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, CssSyntaxError);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.css_syntax_error.prototype"></a>[module postcss.css_syntax_error.prototype](#apidoc.module.postcss.css_syntax_error.prototype)

#### <a name="apidoc.element.postcss.css_syntax_error.prototype.setMessage"></a>[function <span class="apidocSignatureSpan">postcss.css_syntax_error.prototype.</span>setMessage ()](#apidoc.element.postcss.css_syntax_error.prototype.setMessage)
- description and source-code
```javascript
function setMessage() {
<span class="apidocCodeCommentSpan">    /**
     * @member {string} - Full error text in the GNU error format
     *                    with plugin, file, line and column.
     *
     * @example
     * error.message //=> 'a.css:1:1: Unclosed block'
     */
</span>    this.message = this.plugin ? this.plugin + ': ' : '';
    this.message += this.file ? this.file : '<css input>';
    if (typeof this.line !== 'undefined') {
        this.message += ':' + this.line + ':' + this.column;
    }
    this.message += ': ' + this.reason;
}
```
- example usage
```shell
...
         * @example
         * error.column       //=> 1
         * error.input.column //=> 4
         */
        this.column = column;
    }

    this.setMessage();

    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, CssSyntaxError);
    }
}

CssSyntaxError.prototype.setMessage = function setMessage() {
...
```

#### <a name="apidoc.element.postcss.css_syntax_error.prototype.showSourceCode"></a>[function <span class="apidocSignatureSpan">postcss.css_syntax_error.prototype.</span>showSourceCode (color)](#apidoc.element.postcss.css_syntax_error.prototype.showSourceCode)
- description and source-code
```javascript
function showSourceCode(color) {
    var _this = this;

    if (!this.source) return '';

    var css = this.source;
    if (typeof color === 'undefined') color = _supportsColor2.default;
    if (color) css = (0, _terminalHighlight2.default)(css);

    var lines = css.split(/\r?\n/);
    var start = Math.max(this.line - 3, 0);
    var end = Math.min(this.line + 2, lines.length);

    var maxWidth = String(end).length;
    var colors = new _chalk2.default.constructor({ enabled: true });

    function mark(text) {
        if (color) {
            return colors.red.bold(text);
        } else {
            return text;
        }
    }
    function aside(text) {
        if (color) {
            return colors.gray(text);
        } else {
            return text;
        }
    }

    return lines.slice(start, end).map(function (line, index) {
        var number = start + 1 + index;
        var gutter = ' ' + (' ' + number).slice(-maxWidth) + ' | ';
        if (number === _this.line) {
            var spacing = aside(gutter.replace(/\d/g, ' ')) + line.slice(0, _this.column - 1).replace(/[^\t]/g, ' ');
            return mark('>') + aside(gutter) + line + '\n ' + spacing + mark('^');
        } else {
            return ' ' + aside(gutter) + line;
        }
    }).join('\n');
}
```
- example usage
```shell
...
*
* @param {boolean} [color] whether arrow will be colored red by terminal
*                          color codes. By default, PostCSS will detect
*                          color support by 'process.stdout.isTTY'
*                          and 'process.env.NODE_DISABLE_COLORS'.
*
* @example
* error.showSourceCode() //=> "  4 | }
*                        //      5 | a {
*                        //    > 6 |   bad
*                        //        |   ^
*                        //      7 | }
*                        //      8 | b {"
*
* @return {string} few lines of CSS source that caused the error
...
```

#### <a name="apidoc.element.postcss.css_syntax_error.prototype.toString"></a>[function <span class="apidocSignatureSpan">postcss.css_syntax_error.prototype.</span>toString ()](#apidoc.element.postcss.css_syntax_error.prototype.toString)
- description and source-code
```javascript
function toString() {
    var code = this.showSourceCode();
    if (code) {
        code = '\n\n' + code + '\n';
    }
    return this.name + ': ' + this.message + code;
}
```
- example usage
```shell
...
    }).join('\n');
};

/**
 * Returns error position, message and source code of the broken part.
 *
 * @example
 * error.toString() //=> "CssSyntaxError: app.css:1:1: Unclosed block
 *                  //    > 1 | a {
 *                  //        | ^"
 *
 * @return {string} error position, message and source code
 */
...
```



# <a name="apidoc.module.postcss.input"></a>[module postcss.input](#apidoc.module.postcss.input)

#### <a name="apidoc.element.postcss.input.input"></a>[function <span class="apidocSignatureSpan">postcss.</span>input (css)](#apidoc.element.postcss.input.input)
- description and source-code
```javascript
function Input(css) {
    var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

    _classCallCheck(this, Input);

<span class="apidocCodeCommentSpan">    /**
     * @member {string} - input CSS source
     *
     * @example
     * const input = postcss.parse('a{}', { from: file }).input;
     * input.css //=> "a{}";
     */
</span>    this.css = css.toString();

    if (this.css[0] === '\uFEFF' || this.css[0] === '\uFFFE') {
        this.css = this.css.slice(1);
    }

    if (opts.from) {
        if (/^\w+:\/\//.test(opts.from)) {
            /**
             * @member {string} - The absolute path to the CSS source file
             *                    defined with the 'from' option.
             *
             * @example
             * const root = postcss.parse(css, { from: 'a.css' });
             * root.source.input.file //=> '/home/ai/a.css'
             */
            this.file = opts.from;
        } else {
            this.file = _path2.default.resolve(opts.from);
        }
    }

    var map = new _previousMap2.default(this.css, opts);
    if (map.text) {
        /**
         * @member {PreviousMap} - The input source map passed from
         *                         a compilation step before PostCSS
         *                         (for example, from Sass compiler).
         *
         * @example
         * root.source.input.map.consumer().sources //=> ['a.sass']
         */
        this.map = map;
        var file = map.consumer().file;
        if (!this.file && file) this.file = this.mapResolve(file);
    }

    if (!this.file) {
        sequence += 1;
        /**
         * @member {string} - The unique ID of the CSS source. It will be
         *                    created if 'from' option is not provided
         *                    (because PostCSS does not know the file path).
         *
         * @example
         * const root = postcss.parse(css);
         * root.source.input.file //=> undefined
         * root.source.input.id   //=> "<input css 1>"
         */
        this.id = '<input css ' + sequence + '>';
    }
    if (this.map) this.map.file = this.from;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.input.prototype"></a>[module postcss.input.prototype](#apidoc.module.postcss.input.prototype)

#### <a name="apidoc.element.postcss.input.prototype.error"></a>[function <span class="apidocSignatureSpan">postcss.input.prototype.</span>error (message, line, column)](#apidoc.element.postcss.input.prototype.error)
- description and source-code
```javascript
function error(message, line, column) {
    var opts = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

    var result = void 0;
    var origin = this.origin(line, column);
    if (origin) {
        result = new _cssSyntaxError2.default(message, origin.line, origin.column, origin.source, origin.file, opts.plugin);
    } else {
        result = new _cssSyntaxError2.default(message, line, column, this.css, this.file, opts.plugin);
    }

    result.input = { line: line, column: column, source: this.css };
    if (this.file) result.input.file = this.file;

    return result;
}
```
- example usage
```shell
...
 *   if ( error.name === 'CssSyntaxError' ) {
 *     error //=> CssSyntaxError
 *   }
 * }
 *
 * @example
 * // Raising error from plugin
 * throw node.error('Unknown variable', { plugin: 'postcss-vars' });
 */
var CssSyntaxError = function () {

/**
 * @param {string} message  - error message
 * @param {number} [line]   - source line of the error
 * @param {number} [column] - source column of the error
...
```

#### <a name="apidoc.element.postcss.input.prototype.mapResolve"></a>[function <span class="apidocSignatureSpan">postcss.input.prototype.</span>mapResolve (file)](#apidoc.element.postcss.input.prototype.mapResolve)
- description and source-code
```javascript
function mapResolve(file) {
    if (/^\w+:\/\//.test(file)) {
        return file;
    } else {
        return _path2.default.resolve(this.map.consumer().sourceRoot || '.', file);
    }
}
```
- example usage
```shell
...
     *                         (for example, from Sass compiler).
     *
     * @example
     * root.source.input.map.consumer().sources //=> ['a.sass']
     */
    this.map = map;
    var file = map.consumer().file;
    if (!this.file && file) this.file = this.mapResolve(file);
}

if (!this.file) {
    sequence += 1;
    /**
     * @member {string} - The unique ID of the CSS source. It will be
     *                    created if 'from' option is not provided
...
```

#### <a name="apidoc.element.postcss.input.prototype.origin"></a>[function <span class="apidocSignatureSpan">postcss.input.prototype.</span>origin (line, column)](#apidoc.element.postcss.input.prototype.origin)
- description and source-code
```javascript
function origin(line, column) {
    if (!this.map) return false;
    var consumer = this.map.consumer();

    var from = consumer.originalPositionFor({ line: line, column: column });
    if (!from.source) return false;

    var result = {
        file: this.mapResolve(from.source),
        line: from.line,
        column: from.column
    };

    var source = consumer.sourceContentFor(from.source);
    if (source) result.source = source;

    return result;
}
```
- example usage
```shell
...
if (this.map) this.map.file = this.from;
    }

    Input.prototype.error = function error(message, line, column) {
var opts = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

var result = void 0;
var origin = this.origin(line, column);
if (origin) {
    result = new _cssSyntaxError2.default(message, origin.line, origin.column, origin.source, origin.file, opts.plugin);
} else {
    result = new _cssSyntaxError2.default(message, line, column, this.css, this.file, opts.plugin);
}

result.input = { line: line, column: column, source: this.css };
...
```



# <a name="apidoc.module.postcss.lazy_result"></a>[module postcss.lazy_result](#apidoc.module.postcss.lazy_result)

#### <a name="apidoc.element.postcss.lazy_result.lazy_result"></a>[function <span class="apidocSignatureSpan">postcss.</span>lazy_result (processor, css, opts)](#apidoc.element.postcss.lazy_result.lazy_result)
- description and source-code
```javascript
function LazyResult(processor, css, opts) {
    _classCallCheck(this, LazyResult);

    this.stringified = false;
    this.processed = false;

    var root = void 0;
    if ((typeof css === 'undefined' ? 'undefined' : _typeof(css)) === 'object' && css.type === 'root') {
        root = css;
    } else if (css instanceof LazyResult || css instanceof _result2.default) {
        root = css.root;
        if (css.map) {
            if (typeof opts.map === 'undefined') opts.map = {};
            if (!opts.map.inline) opts.map.inline = false;
            opts.map.prev = css.map;
        }
    } else {
        var parser = _parse2.default;
        if (opts.syntax) parser = opts.syntax.parse;
        if (opts.parser) parser = opts.parser;
        if (parser.parse) parser = parser.parse;

        try {
            root = parser(css, opts);
        } catch (error) {
            this.error = error;
        }
    }

    this.result = new _result2.default(processor, root, opts);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.lazy_result.prototype"></a>[module postcss.lazy_result.prototype](#apidoc.module.postcss.lazy_result.prototype)

#### <a name="apidoc.element.postcss.lazy_result.prototype.async"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>async ()](#apidoc.element.postcss.lazy_result.prototype.async)
- description and source-code
```javascript
function async() {
    var _this2 = this;

    if (this.processed) {
        return new Promise(function (resolve, reject) {
            if (_this2.error) {
                reject(_this2.error);
            } else {
                resolve(_this2.stringify());
            }
        });
    }
    if (this.processing) {
        return this.processing;
    }

    this.processing = new Promise(function (resolve, reject) {
        if (_this2.error) return reject(_this2.error);
        _this2.plugin = 0;
        _this2.asyncTick(resolve, reject);
    }).then(function () {
        _this2.processed = true;
        return _this2.stringify();
    });

    return this.processing;
}
```
- example usage
```shell
...
 * postcss([cssnext]).process(css).then(result => {
 *   console.log(result.css);
 * });
 */


LazyResult.prototype.then = function then(onFulfilled, onRejected) {
    return this.async().then(onFulfilled, onRejected);
};

/**
 * Processes input CSS through synchronous and asynchronous plugins
 * and calls onRejected for each error thrown in any plugin.
 *
 * It implements standard Promise API.
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.asyncTick"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>asyncTick (resolve, reject)](#apidoc.element.postcss.lazy_result.prototype.asyncTick)
- description and source-code
```javascript
function asyncTick(resolve, reject) {
    var _this = this;

    if (this.plugin >= this.processor.plugins.length) {
        this.processed = true;
        return resolve();
    }

    try {
        var plugin = this.processor.plugins[this.plugin];
        var promise = this.run(plugin);
        this.plugin += 1;

        if (isPromise(promise)) {
            promise.then(function () {
                _this.asyncTick(resolve, reject);
            }).catch(function (error) {
                _this.handleError(error, plugin);
                _this.processed = true;
                reject(error);
            });
        } else {
            this.asyncTick(resolve, reject);
        }
    } catch (error) {
        this.processed = true;
        reject(error);
    }
}
```
- example usage
```shell
...
        try {
var plugin = this.processor.plugins[this.plugin];
var promise = this.run(plugin);
this.plugin += 1;

if (isPromise(promise)) {
    promise.then(function () {
        _this.asyncTick(resolve, reject);
    }).catch(function (error) {
        _this.handleError(error, plugin);
        _this.processed = true;
        reject(error);
    });
} else {
    this.asyncTick(resolve, reject);
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.catch"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>catch (onRejected)](#apidoc.element.postcss.lazy_result.prototype.catch)
- description and source-code
```javascript
function _catch(onRejected) {
    return this.async().catch(onRejected);
}
```
- example usage
```shell
...
 * @param {onRejected} onRejected - callback will be executed on any error
 *
 * @return {Promise} Promise API to make queue
 *
 * @example
 * postcss([cssnext]).process(css).then(result => {
 *   console.log(result.css);
 * }).catch(error => {
 *   console.error(error);
 * });
 */


LazyResult.prototype.catch = function _catch(onRejected) {
    return this.async().catch(onRejected);
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.handleError"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>handleError (error, plugin)](#apidoc.element.postcss.lazy_result.prototype.handleError)
- description and source-code
```javascript
function handleError(error, plugin) {
    try {
        this.error = error;
        if (error.name === 'CssSyntaxError' && !error.plugin) {
            error.plugin = plugin.postcssPlugin;
            error.setMessage();
        } else if (plugin.postcssVersion) {
            var pluginName = plugin.postcssPlugin;
            var pluginVer = plugin.postcssVersion;
            var runtimeVer = this.result.processor.version;
            var a = pluginVer.split('.');
            var b = runtimeVer.split('.');

            if (a[0] !== b[0] || parseInt(a[1]) > parseInt(b[1])) {
                (0, _warnOnce2.default)('Your current PostCSS version ' + 'is ' + runtimeVer + ', but ' + pluginName + ' ' + 'uses
 ' + pluginVer + '. Perhaps this is ' + 'the source of the error below.');
            }
        }
    } catch (err) {
        if (console && console.error) console.error(err);
    }
}
```
- example usage
```shell
...
    var promise = this.run(plugin);
    this.plugin += 1;

    if (isPromise(promise)) {
        promise.then(function () {
            _this.asyncTick(resolve, reject);
        }).catch(function (error) {
            _this.handleError(error, plugin);
            _this.processed = true;
            reject(error);
        });
    } else {
        this.asyncTick(resolve, reject);
    }
} catch (error) {
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.run"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>run (plugin)](#apidoc.element.postcss.lazy_result.prototype.run)
- description and source-code
```javascript
function run(plugin) {
    this.result.lastPlugin = plugin;

    try {
        return plugin(this.result.root, this.result);
    } catch (error) {
        this.handleError(error, plugin);
        throw error;
    }
}
```
- example usage
```shell
...
        if (this.plugin >= this.processor.plugins.length) {
this.processed = true;
return resolve();
        }

        try {
var plugin = this.processor.plugins[this.plugin];
var promise = this.run(plugin);
this.plugin += 1;

if (isPromise(promise)) {
    promise.then(function () {
        _this.asyncTick(resolve, reject);
    }).catch(function (error) {
        _this.handleError(error, plugin);
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.stringify"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>stringify ()](#apidoc.element.postcss.lazy_result.prototype.stringify)
- description and source-code
```javascript
function stringify() {
    if (this.stringified) return this.result;
    this.stringified = true;

    this.sync();

    var opts = this.result.opts;
    var str = _stringify3.default;
    if (opts.syntax) str = opts.syntax.stringify;
    if (opts.stringifier) str = opts.stringifier;
    if (str.stringify) str = str.stringify;

    var map = new _mapGenerator2.default(str, this.result.root, this.result.opts);
    var data = map.generate();
    this.result.css = data[0];
    this.result.map = data[1];

    return this.result;
}
```
- example usage
```shell
...
var _this2 = this;

if (this.processed) {
    return new Promise(function (resolve, reject) {
        if (_this2.error) {
            reject(_this2.error);
        } else {
            resolve(_this2.stringify());
        }
    });
}
if (this.processing) {
    return this.processing;
}
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.sync"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>sync ()](#apidoc.element.postcss.lazy_result.prototype.sync)
- description and source-code
```javascript
function sync() {
    if (this.processed) return this.result;
    this.processed = true;

    if (this.processing) {
        throw new Error('Use process(css).then(cb) to work with async plugins');
    }

    if (this.error) throw this.error;

    for (var _iterator = this.result.processor.plugins, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator
 : _iterator[Symbol.iterator]();;) {
        var _ref;

        if (_isArray) {
            if (_i >= _iterator.length) break;
            _ref = _iterator[_i++];
        } else {
            _i = _iterator.next();
            if (_i.done) break;
            _ref = _i.value;
        }

        var plugin = _ref;

        var promise = this.run(plugin);
        if (isPromise(promise)) {
            throw new Error('Use process(css).then(cb) to work with async plugins');
        }
    }

    return this.result;
}
```
- example usage
```shell
...
PostCSS and plugins files into a single file.

To apply PostCSS plugins to React Inline Styles, JSS, Radium
and other CSS-in-JS, you can use ['postcss-js'] and transforms style objects.

'''js
var postcss  = require('postcss-js');
var prefixer = postcss.sync([ require('autoprefixer') ]);

prefixer({ display: 'flex' }); //=> { display: ['-webkit-box', '-webkit-flex', '-ms-flexbox', 'flex'] }
'''

['postcss-js']: https://github.com/postcss/postcss-js
[Browserify]:   http://browserify.org/
[webpack]:      https://webpack.github.io/
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.then"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>then (onFulfilled, onRejected)](#apidoc.element.postcss.lazy_result.prototype.then)
- description and source-code
```javascript
function then(onFulfilled, onRejected) {
    return this.async().then(onFulfilled, onRejected);
}
```
- example usage
```shell
...
const postcss = require('postcss');
const precss = require('precss');
const autoprefixer = require('autoprefixer');

fs.readFile('src/app.css', (err, css) => {
    postcss([precss, autoprefixer])
        .process(css, { from: 'src/app.css', to: 'dest/app.css' })
        .then(result => {
            fs.writeFile('dest/app.css', result.css);
            if ( result.map ) fs.writeFile('dest/app.css.map', result.map);
        });
});
'''

Read the [PostCSS API documentation] for more details about the JS API.
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.toString"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>toString ()](#apidoc.element.postcss.lazy_result.prototype.toString)
- description and source-code
```javascript
function toString() {
    return this.css;
}
```
- example usage
```shell
...
    }).join('\n');
};

/**
 * Returns error position, message and source code of the broken part.
 *
 * @example
 * error.toString() //=> "CssSyntaxError: app.css:1:1: Unclosed block
 *                  //    > 1 | a {
 *                  //        | ^"
 *
 * @return {string} error position, message and source code
 */
...
```

#### <a name="apidoc.element.postcss.lazy_result.prototype.warnings"></a>[function <span class="apidocSignatureSpan">postcss.lazy_result.prototype.</span>warnings ()](#apidoc.element.postcss.lazy_result.prototype.warnings)
- description and source-code
```javascript
function warnings() {
    return this.sync().warnings();
}
```
- example usage
```shell
...
/**
 * Processes input CSS through synchronous plugins
 * and calls {@link Result#warnings()}.
 *
 * @return {Warning[]} warnings from plugins
 */
LazyResult.prototype.warnings = function warnings() {
    return this.sync().warnings();
};

/**
 * Alias for the {@link LazyResult#css} property.
 *
 * @example
 * lazy + '' === lazy.css;
...
```



# <a name="apidoc.module.postcss.list"></a>[module postcss.list](#apidoc.module.postcss.list)

#### <a name="apidoc.element.postcss.list.comma"></a>[function <span class="apidocSignatureSpan">postcss.list.</span>comma (string)](#apidoc.element.postcss.list.comma)
- description and source-code
```javascript
function comma(string) {
    var comma = ',';
    return list.split(string, [comma], true);
}
```
- example usage
```shell
...
 * rule.selector //=> 'a, strong'
 */


_createClass(Rule, [{
    key: 'selectors',
    get: function get() {
        return _list2.default.comma(this.selector);
    },
    set: function set(values) {
        var match = this.selector ? this.selector.match(/,\s*/) : null;
        var sep = match ? match[0] : ',' + this.raw('between', 'beforeOpen');
        this.selector = values.join(sep);
    }
}, {
...
```

#### <a name="apidoc.element.postcss.list.space"></a>[function <span class="apidocSignatureSpan">postcss.list.</span>space (string)](#apidoc.element.postcss.list.space)
- description and source-code
```javascript
function space(string) {
    var spaces = [' ', '\n', '\t'];
    return list.split(string, spaces);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.list.split"></a>[function <span class="apidocSignatureSpan">postcss.list.</span>split (string, separators, last)](#apidoc.element.postcss.list.split)
- description and source-code
```javascript
function split(string, separators, last) {
    var array = [];
    var current = '';
    var split = false;

    var func = 0;
    var quote = false;
    var escape = false;

    for (var i = 0; i < string.length; i++) {
        var letter = string[i];

        if (quote) {
            if (escape) {
                escape = false;
            } else if (letter === '\\') {
                escape = true;
            } else if (letter === quote) {
                quote = false;
            }
        } else if (letter === '"' || letter === '\'') {
            quote = letter;
        } else if (letter === '(') {
            func += 1;
        } else if (letter === ')') {
            if (func > 0) func -= 1;
        } else if (func === 0) {
            if (separators.indexOf(letter) !== -1) split = true;
        }

        if (split) {
            if (current !== '') array.push(current.trim());
            current = '';
            split = false;
        } else {
            current += letter;
        }
    }

    if (last || current !== '') array.push(current.trim());
    return array;
}
```
- example usage
```shell
...

if (!this.source) return '';

var css = this.source;
if (typeof color === 'undefined') color = _supportsColor2.default;
if (color) css = (0, _terminalHighlight2.default)(css);

var lines = css.split(/\r?\n/);
var start = Math.max(this.line - 3, 0);
var end = Math.min(this.line + 2, lines.length);

var maxWidth = String(end).length;
var colors = new _chalk2.default.constructor({ enabled: true });

function mark(text) {
...
```



# <a name="apidoc.module.postcss.map_generator"></a>[module postcss.map_generator](#apidoc.module.postcss.map_generator)

#### <a name="apidoc.element.postcss.map_generator.map_generator"></a>[function <span class="apidocSignatureSpan">postcss.</span>map_generator (stringify, root, opts)](#apidoc.element.postcss.map_generator.map_generator)
- description and source-code
```javascript
function MapGenerator(stringify, root, opts) {
    _classCallCheck(this, MapGenerator);

    this.stringify = stringify;
    this.mapOpts = opts.map || {};
    this.root = root;
    this.opts = opts;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.map_generator.prototype"></a>[module postcss.map_generator.prototype](#apidoc.module.postcss.map_generator.prototype)

#### <a name="apidoc.element.postcss.map_generator.prototype.addAnnotation"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>addAnnotation ()](#apidoc.element.postcss.map_generator.prototype.addAnnotation)
- description and source-code
```javascript
function addAnnotation() {
    var content = void 0;

    if (this.isInline()) {
        content = 'data:application/json;base64,' + _jsBase.Base64.encode(this.map.toString());
    } else if (typeof this.mapOpts.annotation === 'string') {
        content = this.mapOpts.annotation;
    } else {
        content = this.outputFile() + '.map';
    }

    var eol = '\n';
    if (this.css.indexOf('\r\n') !== -1) eol = '\r\n';

    this.css += eol + '/*# sourceMappingURL=' + content + ' */';
}
```
- example usage
```shell
...
    }
};

MapGenerator.prototype.generateMap = function generateMap() {
    this.generateString();
    if (this.isSourcesContent()) this.setSourcesContent();
    if (this.previous().length > 0) this.applyPrevMaps();
    if (this.isAnnotation()) this.addAnnotation();

    if (this.isInline()) {
        return [this.css];
    } else {
        return [this.css, this.map];
    }
};
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.applyPrevMaps"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>applyPrevMaps ()](#apidoc.element.postcss.map_generator.prototype.applyPrevMaps)
- description and source-code
```javascript
function applyPrevMaps() {
    for (var _iterator = this.previous(), _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator
[Symbol.iterator]();;) {
        var _ref;

        if (_isArray) {
            if (_i >= _iterator.length) break;
            _ref = _iterator[_i++];
        } else {
            _i = _iterator.next();
            if (_i.done) break;
            _ref = _i.value;
        }

        var prev = _ref;

        var from = this.relative(prev.file);
        var root = prev.root || _path2.default.dirname(prev.file);
        var map = void 0;

        if (this.mapOpts.sourcesContent === false) {
            map = new _sourceMap2.default.SourceMapConsumer(prev.text);
            if (map.sourcesContent) {
                map.sourcesContent = map.sourcesContent.map(function () {
                    return null;
                });
            }
        } else {
            map = prev.consumer();
        }

        this.map.applySourceMap(map, from, this.relative(root));
    }
}
```
- example usage
```shell
...
    return 'to.css';
}
    };

    MapGenerator.prototype.generateMap = function generateMap() {
this.generateString();
if (this.isSourcesContent()) this.setSourcesContent();
if (this.previous().length > 0) this.applyPrevMaps();
if (this.isAnnotation()) this.addAnnotation();

if (this.isInline()) {
    return [this.css];
} else {
    return [this.css, this.map];
}
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.clearAnnotation"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>clearAnnotation ()](#apidoc.element.postcss.map_generator.prototype.clearAnnotation)
- description and source-code
```javascript
function clearAnnotation() {
    if (this.mapOpts.annotation === false) return;

    var node = void 0;
    for (var i = this.root.nodes.length - 1; i >= 0; i--) {
        node = this.root.nodes[i];
        if (node.type !== 'comment') continue;
        if (node.text.indexOf('# sourceMappingURL=') === 0) {
            this.root.removeChild(i);
        }
    }
}
```
- example usage
```shell
...
            });
        }
    }
});
    };

    MapGenerator.prototype.generate = function generate() {
this.clearAnnotation();

if (this.isMap()) {
    return this.generateMap();
} else {
    var result = '';
    this.stringify(this.root, function (i) {
        result += i;
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.generate"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>generate ()](#apidoc.element.postcss.map_generator.prototype.generate)
- description and source-code
```javascript
function generate() {
    this.clearAnnotation();

    if (this.isMap()) {
        return this.generateMap();
    } else {
        var result = '';
        this.stringify(this.root, function (i) {
            result += i;
        });
        return [result];
    }
}
```
- example usage
```shell
...
    var opts = this.result.opts;
    var str = _stringify3.default;
    if (opts.syntax) str = opts.syntax.stringify;
    if (opts.stringifier) str = opts.stringifier;
    if (str.stringify) str = str.stringify;

    var map = new _mapGenerator2.default(str, this.result.root, this.result.opts);
    var data = map.generate();
    this.result.css = data[0];
    this.result.map = data[1];

    return this.result;
};

_createClass(LazyResult, [{
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.generateMap"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>generateMap ()](#apidoc.element.postcss.map_generator.prototype.generateMap)
- description and source-code
```javascript
function generateMap() {
    this.generateString();
    if (this.isSourcesContent()) this.setSourcesContent();
    if (this.previous().length > 0) this.applyPrevMaps();
    if (this.isAnnotation()) this.addAnnotation();

    if (this.isInline()) {
        return [this.css];
    } else {
        return [this.css, this.map];
    }
}
```
- example usage
```shell
...
});
    };

    MapGenerator.prototype.generate = function generate() {
this.clearAnnotation();

if (this.isMap()) {
    return this.generateMap();
} else {
    var result = '';
    this.stringify(this.root, function (i) {
        result += i;
    });
    return [result];
}
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.generateString"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>generateString ()](#apidoc.element.postcss.map_generator.prototype.generateString)
- description and source-code
```javascript
function generateString() {
    var _this3 = this;

    this.css = '';
    this.map = new _sourceMap2.default.SourceMapGenerator({ file: this.outputFile() });

    var line = 1;
    var column = 1;

    var lines = void 0,
        last = void 0;
    this.stringify(this.root, function (str, node, type) {
        _this3.css += str;

        if (node && type !== 'end') {
            if (node.source && node.source.start) {
                _this3.map.addMapping({
                    source: _this3.sourcePath(node),
                    generated: { line: line, column: column - 1 },
                    original: {
                        line: node.source.start.line,
                        column: node.source.start.column - 1
                    }
                });
            } else {
                _this3.map.addMapping({
                    source: '<no source>',
                    original: { line: 1, column: 0 },
                    generated: { line: line, column: column - 1 }
                });
            }
        }

        lines = str.match(/\n/g);
        if (lines) {
            line += lines.length;
            last = str.lastIndexOf('\n');
            column = str.length - last;
        } else {
            column += str.length;
        }

        if (node && type !== 'start') {
            if (node.source && node.source.end) {
                _this3.map.addMapping({
                    source: _this3.sourcePath(node),
                    generated: { line: line, column: column - 1 },
                    original: {
                        line: node.source.end.line,
                        column: node.source.end.column
                    }
                });
            } else {
                _this3.map.addMapping({
                    source: '<no source>',
                    original: { line: 1, column: 0 },
                    generated: { line: line, column: column - 1 }
                });
            }
        }
    });
}
```
- example usage
```shell
...
    return this.relative(this.opts.from);
} else {
    return 'to.css';
}
    };

    MapGenerator.prototype.generateMap = function generateMap() {
this.generateString();
if (this.isSourcesContent()) this.setSourcesContent();
if (this.previous().length > 0) this.applyPrevMaps();
if (this.isAnnotation()) this.addAnnotation();

if (this.isInline()) {
    return [this.css];
} else {
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.isAnnotation"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isAnnotation ()](#apidoc.element.postcss.map_generator.prototype.isAnnotation)
- description and source-code
```javascript
function isAnnotation() {
    if (this.isInline()) {
        return true;
    } else if (typeof this.mapOpts.annotation !== 'undefined') {
        return this.mapOpts.annotation;
    } else if (this.previous().length) {
        return this.previous().some(function (i) {
            return i.annotation;
        });
    } else {
        return true;
    }
}
```
- example usage
```shell
...
    }
};

MapGenerator.prototype.generateMap = function generateMap() {
    this.generateString();
    if (this.isSourcesContent()) this.setSourcesContent();
    if (this.previous().length > 0) this.applyPrevMaps();
    if (this.isAnnotation()) this.addAnnotation();

    if (this.isInline()) {
        return [this.css];
    } else {
        return [this.css, this.map];
    }
};
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.isInline"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isInline ()](#apidoc.element.postcss.map_generator.prototype.isInline)
- description and source-code
```javascript
function isInline() {
    if (typeof this.mapOpts.inline !== 'undefined') {
        return this.mapOpts.inline;
    }

    var annotation = this.mapOpts.annotation;
    if (typeof annotation !== 'undefined' && annotation !== true) {
        return false;
    }

    if (this.previous().length) {
        return this.previous().some(function (i) {
            return i.inline;
        });
    } else {
        return true;
    }
}
```
- example usage
```shell
...
        }

        this.map.applySourceMap(map, from, this.relative(root));
    }
};

MapGenerator.prototype.isAnnotation = function isAnnotation() {
    if (this.isInline()) {
        return true;
    } else if (typeof this.mapOpts.annotation !== 'undefined') {
        return this.mapOpts.annotation;
    } else if (this.previous().length) {
        return this.previous().some(function (i) {
            return i.annotation;
        });
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.isMap"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isMap ()](#apidoc.element.postcss.map_generator.prototype.isMap)
- description and source-code
```javascript
function isMap() {
    if (typeof this.opts.map !== 'undefined') {
        return !!this.opts.map;
    } else {
        return this.previous().length > 0;
    }
}
```
- example usage
```shell
...
    }
});
    };

    MapGenerator.prototype.generate = function generate() {
this.clearAnnotation();

if (this.isMap()) {
    return this.generateMap();
} else {
    var result = '';
    this.stringify(this.root, function (i) {
        result += i;
    });
    return [result];
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.isSourcesContent"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>isSourcesContent ()](#apidoc.element.postcss.map_generator.prototype.isSourcesContent)
- description and source-code
```javascript
function isSourcesContent() {
    if (typeof this.mapOpts.sourcesContent !== 'undefined') {
        return this.mapOpts.sourcesContent;
    }
    if (this.previous().length) {
        return this.previous().some(function (i) {
            return i.withContent();
        });
    } else {
        return true;
    }
}
```
- example usage
```shell
...
} else {
    return 'to.css';
}
    };

    MapGenerator.prototype.generateMap = function generateMap() {
this.generateString();
if (this.isSourcesContent()) this.setSourcesContent();
if (this.previous().length > 0) this.applyPrevMaps();
if (this.isAnnotation()) this.addAnnotation();

if (this.isInline()) {
    return [this.css];
} else {
    return [this.css, this.map];
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.outputFile"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>outputFile ()](#apidoc.element.postcss.map_generator.prototype.outputFile)
- description and source-code
```javascript
function outputFile() {
    if (this.opts.to) {
        return this.relative(this.opts.to);
    } else if (this.opts.from) {
        return this.relative(this.opts.from);
    } else {
        return 'to.css';
    }
}
```
- example usage
```shell
...
    var content = void 0;

    if (this.isInline()) {
        content = 'data:application/json;base64,' + _jsBase.Base64.encode(this.map.toString());
    } else if (typeof this.mapOpts.annotation === 'string') {
        content = this.mapOpts.annotation;
    } else {
        content = this.outputFile() + '.map';
    }

    var eol = '\n';
    if (this.css.indexOf('\r\n') !== -1) eol = '\r\n';

    this.css += eol + '/*# sourceMappingURL=' + content + ' */';
};
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.previous"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>previous ()](#apidoc.element.postcss.map_generator.prototype.previous)
- description and source-code
```javascript
function previous() {
    var _this = this;

    if (!this.previousMaps) {
        this.previousMaps = [];
        this.root.walk(function (node) {
            if (node.source && node.source.input.map) {
                var map = node.source.input.map;
                if (_this.previousMaps.indexOf(map) === -1) {
                    _this.previousMaps.push(map);
                }
            }
        });
    }

    return this.previousMaps;
}
```
- example usage
```shell
...
this.opts = opts;
    }

    MapGenerator.prototype.isMap = function isMap() {
if (typeof this.opts.map !== 'undefined') {
    return !!this.opts.map;
} else {
    return this.previous().length > 0;
}
    };

    MapGenerator.prototype.previous = function previous() {
var _this = this;

if (!this.previousMaps) {
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.relative"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>relative (file)](#apidoc.element.postcss.map_generator.prototype.relative)
- description and source-code
```javascript
function relative(file) {
    if (file.indexOf('<') === 0) return file;
    if (/^\w+:\/\//.test(file)) return file;

    var from = this.opts.to ? _path2.default.dirname(this.opts.to) : '.';

    if (typeof this.mapOpts.annotation === 'string') {
        from = _path2.default.dirname(_path2.default.resolve(from, this.mapOpts.annotation));
    }

    file = _path2.default.relative(from, file);
    if (_path2.default.sep === '\\') {
        return file.replace(/\\/g, '/');
    } else {
        return file;
    }
}
```
- example usage
```shell
...

    var already = {};
    this.root.walk(function (node) {
        if (node.source) {
            var from = node.source.input.from;
            if (from && !already[from]) {
                already[from] = true;
                var relative = _this2.relative(from);
                _this2.map.setSourceContent(relative, node.source.input.css);
            }
        }
    });
};

MapGenerator.prototype.applyPrevMaps = function applyPrevMaps() {
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.setSourcesContent"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>setSourcesContent ()](#apidoc.element.postcss.map_generator.prototype.setSourcesContent)
- description and source-code
```javascript
function setSourcesContent() {
    var _this2 = this;

    var already = {};
    this.root.walk(function (node) {
        if (node.source) {
            var from = node.source.input.from;
            if (from && !already[from]) {
                already[from] = true;
                var relative = _this2.relative(from);
                _this2.map.setSourceContent(relative, node.source.input.css);
            }
        }
    });
}
```
- example usage
```shell
...
} else {
    return 'to.css';
}
    };

    MapGenerator.prototype.generateMap = function generateMap() {
this.generateString();
if (this.isSourcesContent()) this.setSourcesContent();
if (this.previous().length > 0) this.applyPrevMaps();
if (this.isAnnotation()) this.addAnnotation();

if (this.isInline()) {
    return [this.css];
} else {
    return [this.css, this.map];
...
```

#### <a name="apidoc.element.postcss.map_generator.prototype.sourcePath"></a>[function <span class="apidocSignatureSpan">postcss.map_generator.prototype.</span>sourcePath (node)](#apidoc.element.postcss.map_generator.prototype.sourcePath)
- description and source-code
```javascript
function sourcePath(node) {
    if (this.mapOpts.from) {
        return this.mapOpts.from;
    } else {
        return this.relative(node.source.input.from);
    }
}
```
- example usage
```shell
...
last = void 0;
        this.stringify(this.root, function (str, node, type) {
_this3.css += str;

if (node && type !== 'end') {
    if (node.source && node.source.start) {
        _this3.map.addMapping({
            source: _this3.sourcePath(node),
            generated: { line: line, column: column - 1 },
            original: {
                line: node.source.start.line,
                column: node.source.start.column - 1
            }
        });
    } else {
...
```



# <a name="apidoc.module.postcss.node"></a>[module postcss.node](#apidoc.module.postcss.node)

#### <a name="apidoc.element.postcss.node.node"></a>[function <span class="apidocSignatureSpan">postcss.</span>node ()](#apidoc.element.postcss.node.node)
- description and source-code
```javascript
function Node() {
    var defaults = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    _classCallCheck(this, Node);

    this.raws = {};
    if ((typeof defaults === 'undefined' ? 'undefined' : _typeof(defaults)) !== 'object' && typeof defaults !== 'undefined') {
        throw new Error('PostCSS nodes constructor accepts object, not ' + JSON.stringify(defaults));
    }
    for (var name in defaults) {
        this[name] = defaults[name];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.node.prototype"></a>[module postcss.node.prototype](#apidoc.module.postcss.node.prototype)

#### <a name="apidoc.element.postcss.node.prototype.cleanRaws"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cleanRaws (keepBetween)](#apidoc.element.postcss.node.prototype.cleanRaws)
- description and source-code
```javascript
function cleanRaws(keepBetween) {
    delete this.raws.before;
    delete this.raws.after;
    if (!keepBetween) delete this.raws.between;
}
```
- example usage
```shell
...
            } else {
                _i5 = _iterator5.next();
                if (_i5.done) break;
                _ref5 = _i5.value;
            }

            var node = _ref5;
            node.cleanRaws(keepBetween);
        }
    }
};

/**
 * Insert new node before old node within the container.
 *
...
```

#### <a name="apidoc.element.postcss.node.prototype.cleanStyles"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cleanStyles (keepBetween)](#apidoc.element.postcss.node.prototype.cleanStyles)
- description and source-code
```javascript
function cleanStyles(keepBetween) {
    (0, _warnOnce2.default)('Node#cleanStyles() is deprecated. Use Node#cleanRaws()');
    return this.cleanRaws(keepBetween);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node.prototype.clone"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>clone ()](#apidoc.element.postcss.node.prototype.clone)
- description and source-code
```javascript
function clone() {
    var overrides = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    var cloned = cloneNode(this);
    for (var name in overrides) {
        cloned[name] = overrides[name];
    }
    return cloned;
}
```
- example usage
```shell
...
     *
     * @param {Node|number} exist             - child or child’s index.
     * @param {Node|object|string|Node[]} add - new node
     *
     * @return {Node} this node for methods chain
     *
     * @example
     * rule.insertBefore(decl, decl.clone({ prop: '-webkit-' + decl.prop }));
     */


    Container.prototype.insertBefore = function insertBefore(exist, add) {
exist = this.index(exist);

var type = exist === 0 ? 'prepend' : false;
...
```

#### <a name="apidoc.element.postcss.node.prototype.cloneAfter"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cloneAfter ()](#apidoc.element.postcss.node.prototype.cloneAfter)
- description and source-code
```javascript
function cloneAfter() {
    var overrides = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    var cloned = this.clone(overrides);
    this.parent.insertAfter(this, cloned);
    return cloned;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node.prototype.cloneBefore"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>cloneBefore ()](#apidoc.element.postcss.node.prototype.cloneBefore)
- description and source-code
```javascript
function cloneBefore() {
    var overrides = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    var cloned = this.clone(overrides);
    this.parent.insertBefore(this, cloned);
    return cloned;
}
```
- example usage
```shell
...
* @return {false|undefined} returns 'false' if iteration was broke
*
* @example
* const root = postcss.parse('a { color: black; z-index: 1 }');
* const rule = root.first;
*
* for ( let decl of rule.nodes ) {
*     decl.cloneBefore({ prop: '-webkit-' + decl.prop });
*     // Cycle will be infinite, because cloneBefore moves the current node
*     // to the next index
* }
*
* rule.each(decl => {
*     decl.cloneBefore({ prop: '-webkit-' + decl.prop });
*     // Will be executed only for color and z-index
...
```

#### <a name="apidoc.element.postcss.node.prototype.error"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>error (message)](#apidoc.element.postcss.node.prototype.error)
- description and source-code
```javascript
function error(message) {
    var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

    if (this.source) {
        var pos = this.positionBy(opts);
        return this.source.input.error(message, pos.line, pos.column, opts);
    } else {
        return new _cssSyntaxError2.default(message);
    }
}
```
- example usage
```shell
...
 *   if ( error.name === 'CssSyntaxError' ) {
 *     error //=> CssSyntaxError
 *   }
 * }
 *
 * @example
 * // Raising error from plugin
 * throw node.error('Unknown variable', { plugin: 'postcss-vars' });
 */
var CssSyntaxError = function () {

/**
 * @param {string} message  - error message
 * @param {number} [line]   - source line of the error
 * @param {number} [column] - source column of the error
...
```

#### <a name="apidoc.element.postcss.node.prototype.moveAfter"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>moveAfter (otherNode)](#apidoc.element.postcss.node.prototype.moveAfter)
- description and source-code
```javascript
function moveAfter(otherNode) {
    this.cleanRaws(this.root() === otherNode.root());
    this.remove();
    otherNode.parent.insertAfter(otherNode, this);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node.prototype.moveBefore"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>moveBefore (otherNode)](#apidoc.element.postcss.node.prototype.moveBefore)
- description and source-code
```javascript
function moveBefore(otherNode) {
    this.cleanRaws(this.root() === otherNode.root());
    this.remove();
    otherNode.parent.insertBefore(otherNode, this);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node.prototype.moveTo"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>moveTo (newParent)](#apidoc.element.postcss.node.prototype.moveTo)
- description and source-code
```javascript
function moveTo(newParent) {
    this.cleanRaws(this.root() === newParent.root());
    this.remove();
    newParent.append(this);
    return this;
}
```
- example usage
```shell
...
 * It will also clean the 'between' property
 * if 'newParent' is in another {@link Root}.
 *
 * @param {Container} newParent - container node where the current node
 *                                will be moved
 *
 * @example
 * atrule.moveTo(atrule.root());
 *
 * @return {Node} current node to methods chain
 */


Node.prototype.moveTo = function moveTo(newParent) {
    this.cleanRaws(this.root() === newParent.root());
...
```

#### <a name="apidoc.element.postcss.node.prototype.next"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>next ()](#apidoc.element.postcss.node.prototype.next)
- description and source-code
```javascript
function next() {
    var index = this.parent.index(this);
    return this.parent.nodes[index + 1];
}
```
- example usage
```shell
...
        for (var _iterator = children, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator
[Symbol.iterator]();;) {
var _ref;

if (_isArray) {
    if (_i >= _iterator.length) break;
    _ref = _iterator[_i++];
} else {
    _i = _iterator.next();
    if (_i.done) break;
    _ref = _i.value;
}

var child = _ref;

var nodes = this.normalize(child, this.last);
...
```

#### <a name="apidoc.element.postcss.node.prototype.positionBy"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>positionBy (opts)](#apidoc.element.postcss.node.prototype.positionBy)
- description and source-code
```javascript
function positionBy(opts) {
    var pos = this.source.start;
    if (opts.index) {
        pos = this.positionInside(opts.index);
    } else if (opts.word) {
        var index = this.toString().indexOf(opts.word);
        if (index !== -1) pos = this.positionInside(index);
    }
    return pos;
}
```
- example usage
```shell
...
 */


Node.prototype.error = function error(message) {
    var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

    if (this.source) {
        var pos = this.positionBy(opts);
        return this.source.input.error(message, pos.line, pos.column, opts);
    } else {
        return new _cssSyntaxError2.default(message);
    }
};

/**
...
```

#### <a name="apidoc.element.postcss.node.prototype.positionInside"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>positionInside (index)](#apidoc.element.postcss.node.prototype.positionInside)
- description and source-code
```javascript
function positionInside(index) {
    var string = this.toString();
    var column = this.source.start.column;
    var line = this.source.start.line;

    for (var i = 0; i < index; i++) {
        if (string[i] === '\n') {
            column = 1;
            line += 1;
        } else {
            column += 1;
        }
    }

    return { line: line, column: column };
}
```
- example usage
```shell
...

    return { line: line, column: column };
};

Node.prototype.positionBy = function positionBy(opts) {
    var pos = this.source.start;
    if (opts.index) {
        pos = this.positionInside(opts.index);
    } else if (opts.word) {
        var index = this.toString().indexOf(opts.word);
        if (index !== -1) pos = this.positionInside(index);
    }
    return pos;
};
...
```

#### <a name="apidoc.element.postcss.node.prototype.prev"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>prev ()](#apidoc.element.postcss.node.prototype.prev)
- description and source-code
```javascript
function prev() {
    var index = this.parent.index(this);
    return this.parent.nodes[index - 1];
}
```
- example usage
```shell
...
/**
 * Returns the previous child of the node’s parent.
 * Returns 'undefined' if the current node is the first child.
 *
 * @return {Node|undefined} previous node
 *
 * @example
 * const annotation = decl.prev();
 * if ( annotation.type == 'comment' ) {
 *  readAnnotation(annotation.text);
 * }
 */


Node.prototype.prev = function prev() {
...
```

#### <a name="apidoc.element.postcss.node.prototype.raw"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>raw (prop, defaultType)](#apidoc.element.postcss.node.prototype.raw)
- description and source-code
```javascript
function raw(prop, defaultType) {
    var str = new _stringifier2.default();
    return str.raw(this, prop, defaultType);
}
```
- example usage
```shell
...
 * @param {string} [defaultType] - name of default value, it can be missed
 *                                 if the value is the same as prop
 *
 * @example
 * const root = postcss.parse('a { background: white }');
 * root.nodes[0].append({ prop: 'color', value: 'black' });
 * root.nodes[0].nodes[1].raws.before   //=> undefined
 * root.nodes[0].nodes[1].raw('before') //=> ' '
 *
 * @return {string} code style value
 */


Node.prototype.raw = function raw(prop, defaultType) {
    var str = new _stringifier2.default();
...
```

#### <a name="apidoc.element.postcss.node.prototype.remove"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>remove ()](#apidoc.element.postcss.node.prototype.remove)
- description and source-code
```javascript
function remove() {
    if (this.parent) {
        this.parent.removeChild(this);
    }
    this.parent = undefined;
    return this;
}
```
- example usage
```shell
...
*
* @example
* root.walkDecls(decl => {
*   checkPropertySupport(decl.prop);
* });
*
* root.walkDecls('border-radius', decl => {
*   decl.remove();
* });
*
* root.walkDecls(/^background/, decl => {
*   decl.value = takeFirstColorFromGradient(decl.value);
* });
*/
...
```

#### <a name="apidoc.element.postcss.node.prototype.removeSelf"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>removeSelf ()](#apidoc.element.postcss.node.prototype.removeSelf)
- description and source-code
```javascript
function removeSelf() {
    (0, _warnOnce2.default)('Node#removeSelf is deprecated. Use Node#remove.');
    return this.remove();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node.prototype.replace"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>replace (nodes)](#apidoc.element.postcss.node.prototype.replace)
- description and source-code
```javascript
function replace(nodes) {
    (0, _warnOnce2.default)('Node#replace is deprecated. Use Node#replaceWith');
    return this.replaceWith(nodes);
}
```
- example usage
```shell
...
        opts = {};
    }

    this.walkDecls(function (decl) {
        if (opts.props && opts.props.indexOf(decl.prop) === -1) return;
        if (opts.fast && decl.value.indexOf(opts.fast) === -1) return;

        decl.value = decl.value.replace(pattern, callback);
    });

    return this;
};

/**
 * Returns 'true' if callback returns 'true'
...
```

#### <a name="apidoc.element.postcss.node.prototype.replaceWith"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>replaceWith ()](#apidoc.element.postcss.node.prototype.replaceWith)
- description and source-code
```javascript
function replaceWith() {
    if (this.parent) {
        for (var _len = arguments.length, nodes = Array(_len), _key = 0; _key < _len; _key++) {
            nodes[_key] = arguments[_key];
        }

        for (var _iterator = nodes, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator[Symbol
.iterator]();;) {
            var _ref;

            if (_isArray) {
                if (_i >= _iterator.length) break;
                _ref = _iterator[_i++];
            } else {
                _i = _iterator.next();
                if (_i.done) break;
                _ref = _i.value;
            }

            var node = _ref;

            this.parent.insertBefore(this, node);
        }

        this.remove();
    }

    return this;
}
```
- example usage
```shell
...
/**
 * Inserts node(s) before the current node and removes the current node.
 *
 * @param {...Node} nodes - node(s) to replace current one
 *
 * @example
 * if ( atrule.name == 'mixin' ) {
 *   atrule.replaceWith(mixinRules[atrule.params]);
 * }
 *
 * @return {Node} current node to methods chain
 */


Node.prototype.replaceWith = function replaceWith() {
...
```

#### <a name="apidoc.element.postcss.node.prototype.root"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>root ()](#apidoc.element.postcss.node.prototype.root)
- description and source-code
```javascript
function root() {
    var result = this;
    while (result.parent) {
        result = result.parent;
    }return result;
}
```
- example usage
```shell
...
 * It will also clean the 'between' property
 * if 'newParent' is in another {@link Root}.
 *
 * @param {Container} newParent - container node where the current node
 *                                will be moved
 *
 * @example
 * atrule.moveTo(atrule.root());
 *
 * @return {Node} current node to methods chain
 */


Node.prototype.moveTo = function moveTo(newParent) {
    this.cleanRaws(this.root() === newParent.root());
...
```

#### <a name="apidoc.element.postcss.node.prototype.style"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>style (own, detect)](#apidoc.element.postcss.node.prototype.style)
- description and source-code
```javascript
function style(own, detect) {
    (0, _warnOnce2.default)('Node#style() is deprecated. Use Node#raw()');
    return this.raw(own, detect);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.node.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>toJSON ()](#apidoc.element.postcss.node.prototype.toJSON)
- description and source-code
```javascript
function toJSON() {
    var fixed = {};

    for (var name in this) {
        if (!this.hasOwnProperty(name)) continue;
        if (name === 'parent') continue;
        var value = this[name];

        if (value instanceof Array) {
            fixed[name] = value.map(function (i) {
                if ((typeof i === 'undefined' ? 'undefined' : _typeof(i)) === 'object' && i.toJSON) {
                    return i.toJSON();
                } else {
                    return i;
                }
            });
        } else if ((typeof value === 'undefined' ? 'undefined' : _typeof(value)) === 'object' && value.toJSON) {
            fixed[name] = value.toJSON();
        } else {
            fixed[name] = value;
        }
    }

    return fixed;
}
```
- example usage
```shell
...
if (!this.hasOwnProperty(name)) continue;
if (name === 'parent') continue;
var value = this[name];

if (value instanceof Array) {
    fixed[name] = value.map(function (i) {
        if ((typeof i === 'undefined' ? 'undefined' : _typeof(i)) === 'object' && i.toJSON) {
            return i.toJSON();
        } else {
            return i;
        }
    });
} else if ((typeof value === 'undefined' ? 'undefined' : _typeof(value)) === 'object' && value.toJSON) {
    fixed[name] = value.toJSON();
} else {
...
```

#### <a name="apidoc.element.postcss.node.prototype.toString"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>toString ()](#apidoc.element.postcss.node.prototype.toString)
- description and source-code
```javascript
function toString() {
    var stringifier = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : _stringify2.default;

    if (stringifier.stringify) stringifier = stringifier.stringify;
    var result = '';
    stringifier(this, function (i) {
        result += i;
    });
    return result;
}
```
- example usage
```shell
...
    }).join('\n');
};

/**
 * Returns error position, message and source code of the broken part.
 *
 * @example
 * error.toString() //=> "CssSyntaxError: app.css:1:1: Unclosed block
 *                  //    > 1 | a {
 *                  //        | ^"
 *
 * @return {string} error position, message and source code
 */
...
```

#### <a name="apidoc.element.postcss.node.prototype.warn"></a>[function <span class="apidocSignatureSpan">postcss.node.prototype.</span>warn (result, text, opts)](#apidoc.element.postcss.node.prototype.warn)
- description and source-code
```javascript
function warn(result, text, opts) {
    var data = { node: this };
    for (var i in opts) {
        data[i] = opts[i];
    }return result.warn(text, data);
}
```
- example usage
```shell
...
 *
 * @return {Warning} created warning object
 *
 * @example
 * const plugin = postcss.plugin('postcss-deprecated', () => {
 *   return (root, result) => {
 *     root.walkDecls('bad', decl => {
 *       decl.warn(result, 'Deprecated property bad');
 *     });
 *   };
 * });
 */


Node.prototype.warn = function warn(result, text, opts) {
...
```



# <a name="apidoc.module.postcss.parser"></a>[module postcss.parser](#apidoc.module.postcss.parser)

#### <a name="apidoc.element.postcss.parser.parser"></a>[function <span class="apidocSignatureSpan">postcss.</span>parser (input)](#apidoc.element.postcss.parser.parser)
- description and source-code
```javascript
function Parser(input) {
    _classCallCheck(this, Parser);

    this.input = input;

    this.pos = 0;
    this.root = new _root2.default();
    this.current = this.root;
    this.spaces = '';
    this.semicolon = false;

    this.root.source = { input: input, start: { line: 1, column: 1 } };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.parser.prototype"></a>[module postcss.parser.prototype](#apidoc.module.postcss.parser.prototype)

#### <a name="apidoc.element.postcss.parser.prototype.atrule"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>atrule (token)](#apidoc.element.postcss.parser.prototype.atrule)
- description and source-code
```javascript
function atrule(token) {
    var node = new _atRule2.default();
    node.name = token[1].slice(1);
    if (node.name === '') {
        this.unnamedAtrule(node, token);
    }
    this.init(node, token[2], token[3]);

    var last = false;
    var open = false;
    var params = [];

    this.pos += 1;
    while (this.pos < this.tokens.length) {
        token = this.tokens[this.pos];

        if (token[0] === ';') {
            node.source.end = { line: token[2], column: token[3] };
            this.semicolon = true;
            break;
        } else if (token[0] === '{') {
            open = true;
            break;
        } else if (token[0] === '}') {
            this.end(token);
            break;
        } else {
            params.push(token);
        }

        this.pos += 1;
    }
    if (this.pos === this.tokens.length) {
        last = true;
    }

    node.raws.between = this.spacesAndCommentsFromEnd(params);
    if (params.length) {
        node.raws.afterName = this.spacesAndCommentsFromStart(params);
        this.raw(node, 'params', params);
        if (last) {
            token = params[params.length - 1];
            node.source.end = { line: token[4], column: token[5] };
            this.spaces = node.raws.between;
            node.raws.between = '';
        }
    } else {
        node.raws.afterName = '';
        node.params = '';
    }

    if (open) {
        node.nodes = [];
        this.current = node;
    }
}
```
- example usage
```shell
...
    break;

case 'comment':
    this.comment(token);
    break;

case 'at-word':
    this.atrule(token);
    break;

case '{':
    this.emptyRule(token);
    break;

default:
...
```

#### <a name="apidoc.element.postcss.parser.prototype.checkMissedSemicolon"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>checkMissedSemicolon (tokens)](#apidoc.element.postcss.parser.prototype.checkMissedSemicolon)
- description and source-code
```javascript
function checkMissedSemicolon(tokens) {
    var colon = this.colon(tokens);
    if (colon === false) return;

    var founded = 0;
    var token = void 0;
    for (var j = colon - 1; j >= 0; j--) {
        token = tokens[j];
        if (token[0] !== 'space') {
            founded += 1;
            if (founded === 2) break;
        }
    }
    throw this.input.error('Missed semicolon', token[2], token[3]);
}
```
- example usage
```shell
...
        if (token[0] !== 'space' && token[0] !== 'comment') {
            break;
        }
    }

    this.raw(node, 'value', tokens);

    if (node.value.indexOf(':') !== -1) this.checkMissedSemicolon(tokens);
};

Parser.prototype.atrule = function atrule(token) {
    var node = new _atRule2.default();
    node.name = token[1].slice(1);
    if (node.name === '') {
        this.unnamedAtrule(node, token);
...
```

#### <a name="apidoc.element.postcss.parser.prototype.colon"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>colon (tokens)](#apidoc.element.postcss.parser.prototype.colon)
- description and source-code
```javascript
function colon(tokens) {
    var brackets = 0;
    var token = void 0,
        type = void 0,
        prev = void 0;
    for (var i = 0; i < tokens.length; i++) {
        token = tokens[i];
        type = token[0];

        if (type === '(') {
            brackets += 1;
        } else if (type === ')') {
            brackets -= 1;
        } else if (brackets === 0 && type === ':') {
            if (!prev) {
                this.doubleColon(token);
            } else if (prev[0] === 'word' && prev[1] === 'progid') {
                continue;
            } else {
                return i;
            }
        }

        prev = token;
    }
    return false;
}
```
- example usage
```shell
...

    Parser.prototype.precheckMissedSemicolon = function precheckMissedSemicolon(tokens) {
// Hook for Safe Parser
tokens;
    };

    Parser.prototype.checkMissedSemicolon = function checkMissedSemicolon(tokens) {
var colon = this.colon(tokens);
if (colon === false) return;

var founded = 0;
var token = void 0;
for (var j = colon - 1; j >= 0; j--) {
    token = tokens[j];
    if (token[0] !== 'space') {
...
```

#### <a name="apidoc.element.postcss.parser.prototype.comment"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>comment (token)](#apidoc.element.postcss.parser.prototype.comment)
- description and source-code
```javascript
function comment(token) {
    var node = new _comment2.default();
    this.init(node, token[2], token[3]);
    node.source.end = { line: token[4], column: token[5] };

    var text = token[1].slice(2, -2);
    if (/^\s*$/.test(text)) {
        node.text = '';
        node.raws.left = text;
        node.raws.right = '';
    } else {
        var match = text.match(/^(\s*)([^]*[^\s])(\s*)$/);
        node.text = match[2];
        node.raws.left = match[1];
        node.raws.right = match[3];
    }
}
```
- example usage
```shell
...
    break;

case '}':
    this.end(token);
    break;

case 'comment':
    this.comment(token);
    break;

case 'at-word':
    this.atrule(token);
    break;

case '{':
...
```

#### <a name="apidoc.element.postcss.parser.prototype.decl"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>decl (tokens)](#apidoc.element.postcss.parser.prototype.decl)
- description and source-code
```javascript
function decl(tokens) {
    var node = new _declaration2.default();
    this.init(node);

    var last = tokens[tokens.length - 1];
    if (last[0] === ';') {
        this.semicolon = true;
        tokens.pop();
    }
    if (last[4]) {
        node.source.end = { line: last[4], column: last[5] };
    } else {
        node.source.end = { line: last[2], column: last[3] };
    }

    while (tokens[0][0] !== 'word') {
        node.raws.before += tokens.shift()[1];
    }
    node.source.start = { line: tokens[0][2], column: tokens[0][3] };

    node.prop = '';
    while (tokens.length) {
        var type = tokens[0][0];
        if (type === ':' || type === 'space' || type === 'comment') {
            break;
        }
        node.prop += tokens.shift()[1];
    }

    node.raws.between = '';

    var token = void 0;
    while (tokens.length) {
        token = tokens.shift();

        if (token[0] === ':') {
            node.raws.between += token[1];
            break;
        } else {
            node.raws.between += token[1];
        }
    }

    if (node.prop[0] === '_' || node.prop[0] === '*') {
        node.raws.before += node.prop[0];
        node.prop = node.prop.slice(1);
    }
    node.raws.between += this.spacesAndCommentsFromStart(tokens);
    this.precheckMissedSemicolon(tokens);

    for (var i = tokens.length - 1; i > 0; i--) {
        token = tokens[i];
        if (token[1] === '!important') {
            node.important = true;
            var string = this.stringFrom(tokens, i);
            string = this.spacesFromEnd(tokens) + string;
            if (string !== ' !important') node.raws.important = string;
            break;
        } else if (token[1] === 'important') {
            var cache = tokens.slice(0);
            var str = '';
            for (var j = i; j > 0; j--) {
                var _type = cache[j][0];
                if (str.trim().indexOf('!') === 0 && _type !== 'space') {
                    break;
                }
                str = cache.pop()[1] + str;
            }
            if (str.trim().indexOf('!') === 0) {
                node.important = true;
                node.raws.important = str;
                tokens = cache;
            }
        }

        if (token[0] !== 'space' && token[0] !== 'comment') {
            break;
        }
    }

    this.raw(node, 'value', tokens);

    if (node.value.indexOf(':') !== -1) this.checkMissedSemicolon(tokens);
}
```
- example usage
```shell
...
* Inserts new nodes to the end of the container.
*
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.append(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
...
```

#### <a name="apidoc.element.postcss.parser.prototype.doubleColon"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>doubleColon (token)](#apidoc.element.postcss.parser.prototype.doubleColon)
- description and source-code
```javascript
function doubleColon(token) {
    throw this.input.error('Double colon', token[2], token[3]);
}
```
- example usage
```shell
...

if (type === '(') {
    brackets += 1;
} else if (type === ')') {
    brackets -= 1;
} else if (brackets === 0 && type === ':') {
    if (!prev) {
        this.doubleColon(token);
    } else if (prev[0] === 'word' && prev[1] === 'progid') {
        continue;
    } else {
        return i;
    }
}
...
```

#### <a name="apidoc.element.postcss.parser.prototype.emptyRule"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>emptyRule (token)](#apidoc.element.postcss.parser.prototype.emptyRule)
- description and source-code
```javascript
function emptyRule(token) {
    var node = new _rule2.default();
    this.init(node, token[2], token[3]);
    node.selector = '';
    node.raws.between = '';
    this.current = node;
}
```
- example usage
```shell
...
        break;

    case 'at-word':
        this.atrule(token);
        break;

    case '{':
        this.emptyRule(token);
        break;

    default:
        this.other();
        break;
}
...
```

#### <a name="apidoc.element.postcss.parser.prototype.end"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>end (token)](#apidoc.element.postcss.parser.prototype.end)
- description and source-code
```javascript
function end(token) {
    if (this.current.nodes && this.current.nodes.length) {
        this.current.raws.semicolon = this.semicolon;
    }
    this.semicolon = false;

    this.current.raws.after = (this.current.raws.after || '') + this.spaces;
    this.spaces = '';

    if (this.current.parent) {
        this.current.source.end = { line: token[2], column: token[3] };
        this.current = this.current.parent;
    } else {
        this.unexpectedClose(token);
    }
}
```
- example usage
```shell
...

case 'space':
case ';':
    this.spaces += token[1];
    break;

case '}':
    this.end(token);
    break;

case 'comment':
    this.comment(token);
    break;

case 'at-word':
...
```

#### <a name="apidoc.element.postcss.parser.prototype.endFile"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>endFile ()](#apidoc.element.postcss.parser.prototype.endFile)
- description and source-code
```javascript
function endFile() {
    if (this.current.parent) this.unclosedBlock();
    if (this.current.nodes && this.current.nodes.length) {
        this.current.raws.semicolon = this.semicolon;
    }
    this.current.raws.after = (this.current.raws.after || '') + this.spaces;
}
```
- example usage
```shell
...
            default:
                this.other();
                break;
        }

        this.pos += 1;
    }
    this.endFile();
};

Parser.prototype.comment = function comment(token) {
    var node = new _comment2.default();
    this.init(node, token[2], token[3]);
    node.source.end = { line: token[4], column: token[5] };
...
```

#### <a name="apidoc.element.postcss.parser.prototype.init"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>init (node, line, column)](#apidoc.element.postcss.parser.prototype.init)
- description and source-code
```javascript
function init(node, line, column) {
    this.current.push(node);

    node.source = { start: { line: line, column: column }, input: this.input };
    node.raws.before = this.spaces;
    this.spaces = '';
    if (node.type !== 'comment') this.semicolon = false;
}
```
- example usage
```shell
...

'''js
gulp.task('css', function () {
    var postcss    = require('gulp-postcss');
    var sourcemaps = require('gulp-sourcemaps');

    return gulp.src('src/**/*.css')
        .pipe( sourcemaps.init() )
        .pipe( postcss([ require('precss'), require('autoprefixer') ]) )
        .pipe( sourcemaps.write('.') )
        .pipe( gulp.dest('build/') );
});
'''

['gulp-sourcemaps']: https://github.com/floridoo/gulp-sourcemaps
...
```

#### <a name="apidoc.element.postcss.parser.prototype.loop"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>loop ()](#apidoc.element.postcss.parser.prototype.loop)
- description and source-code
```javascript
function loop() {
    var token = void 0;
    while (this.pos < this.tokens.length) {
        token = this.tokens[this.pos];

        switch (token[0]) {

            case 'space':
            case ';':
                this.spaces += token[1];
                break;

            case '}':
                this.end(token);
                break;

            case 'comment':
                this.comment(token);
                break;

            case 'at-word':
                this.atrule(token);
                break;

            case '{':
                this.emptyRule(token);
                break;

            default:
                this.other();
                break;
        }

        this.pos += 1;
    }
    this.endFile();
}
```
- example usage
```shell
...
}

var input = new _input2.default(css, opts);

var parser = new _parser2.default(input);
try {
    parser.tokenize();
    parser.loop();
} catch (e) {
    if (e.name === 'CssSyntaxError' && opts && opts.from) {
        if (/\.scss$/i.test(opts.from)) {
            e.message += '\nYou tried to parse SCSS with ' + 'the standard CSS parser; ' + 'try again with the postcss-scss parser
';
        } else if (/\.less$/i.test(opts.from)) {
            e.message += '\nYou tried to parse Less with ' + 'the standard CSS parser; ' + 'try again with the postcss-less parser
';
        }
...
```

#### <a name="apidoc.element.postcss.parser.prototype.other"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>other ()](#apidoc.element.postcss.parser.prototype.other)
- description and source-code
```javascript
function other() {
    var token = void 0;
    var end = false;
    var type = null;
    var colon = false;
    var bracket = null;
    var brackets = [];

    var start = this.pos;
    while (this.pos < this.tokens.length) {
        token = this.tokens[this.pos];
        type = token[0];

        if (type === '(' || type === '[') {
            if (!bracket) bracket = token;
            brackets.push(type === '(' ? ')' : ']');
        } else if (brackets.length === 0) {
            if (type === ';') {
                if (colon) {
                    this.decl(this.tokens.slice(start, this.pos + 1));
                    return;
                } else {
                    break;
                }
            } else if (type === '{') {
                this.rule(this.tokens.slice(start, this.pos + 1));
                return;
            } else if (type === '}') {
                this.pos -= 1;
                end = true;
                break;
            } else if (type === ':') {
                colon = true;
            }
        } else if (type === brackets[brackets.length - 1]) {
            brackets.pop();
            if (brackets.length === 0) bracket = null;
        }

        this.pos += 1;
    }
    if (this.pos === this.tokens.length) {
        this.pos -= 1;
        end = true;
    }

    if (brackets.length > 0) this.unclosedBracket(bracket);

    if (end && colon) {
        while (this.pos > start) {
            token = this.tokens[this.pos][0];
            if (token !== 'space' && token !== 'comment') break;
            this.pos -= 1;
        }
        this.decl(this.tokens.slice(start, this.pos + 1));
        return;
    }

    this.unknownWord(start);
}
```
- example usage
```shell
...
                break;

            case '{':
                this.emptyRule(token);
                break;

            default:
                this.other();
                break;
        }

        this.pos += 1;
    }
    this.endFile();
};
...
```

#### <a name="apidoc.element.postcss.parser.prototype.precheckMissedSemicolon"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>precheckMissedSemicolon (tokens)](#apidoc.element.postcss.parser.prototype.precheckMissedSemicolon)
- description and source-code
```javascript
function precheckMissedSemicolon(tokens) {
    // Hook for Safe Parser
    tokens;
}
```
- example usage
```shell
...
}

if (node.prop[0] === '_' || node.prop[0] === '*') {
    node.raws.before += node.prop[0];
    node.prop = node.prop.slice(1);
}
node.raws.between += this.spacesAndCommentsFromStart(tokens);
this.precheckMissedSemicolon(tokens);

for (var i = tokens.length - 1; i > 0; i--) {
    token = tokens[i];
    if (token[1] === '!important') {
        node.important = true;
        var string = this.stringFrom(tokens, i);
        string = this.spacesFromEnd(tokens) + string;
...
```

#### <a name="apidoc.element.postcss.parser.prototype.raw"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>raw (node, prop, tokens)](#apidoc.element.postcss.parser.prototype.raw)
- description and source-code
```javascript
function raw(node, prop, tokens) {
    var token = void 0,
        type = void 0;
    var length = tokens.length;
    var value = '';
    var clean = true;
    for (var i = 0; i < length; i += 1) {
        token = tokens[i];
        type = token[0];
        if (type === 'comment' || type === 'space' && i === length - 1) {
            clean = false;
        } else {
            value += token[1];
        }
    }
    if (!clean) {
        var raw = tokens.reduce(function (all, i) {
            return all + i[1];
        }, '');
        node.raws[prop] = { value: value, raw: raw };
    }
    node[prop] = value;
}
```
- example usage
```shell
...
 * @param {string} [defaultType] - name of default value, it can be missed
 *                                 if the value is the same as prop
 *
 * @example
 * const root = postcss.parse('a { background: white }');
 * root.nodes[0].append({ prop: 'color', value: 'black' });
 * root.nodes[0].nodes[1].raws.before   //=> undefined
 * root.nodes[0].nodes[1].raw('before') //=> ' '
 *
 * @return {string} code style value
 */


Node.prototype.raw = function raw(prop, defaultType) {
    var str = new _stringifier2.default();
...
```

#### <a name="apidoc.element.postcss.parser.prototype.rule"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>rule (tokens)](#apidoc.element.postcss.parser.prototype.rule)
- description and source-code
```javascript
function rule(tokens) {
    tokens.pop();

    var node = new _rule2.default();
    this.init(node, tokens[0][2], tokens[0][3]);

    node.raws.between = this.spacesAndCommentsFromEnd(tokens);
    this.raw(node, 'selector', tokens);
    this.current = node;
}
```
- example usage
```shell
...
     *
     * @param {stringifier|syntax} [stringifier] - a syntax to use
     *                                             in string generation
     *
     * @return {string} CSS string of this node
     *
     * @example
     * postcss.rule({ selector: 'a' }).toString() //=> "a {}"
     */


    Node.prototype.toString = function toString() {
var stringifier = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : _stringify2.default;

if (stringifier.stringify) stringifier = stringifier.stringify;
...
```

#### <a name="apidoc.element.postcss.parser.prototype.spacesAndCommentsFromEnd"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>spacesAndCommentsFromEnd (tokens)](#apidoc.element.postcss.parser.prototype.spacesAndCommentsFromEnd)
- description and source-code
```javascript
function spacesAndCommentsFromEnd(tokens) {
    var lastTokenType = void 0;
    var spaces = '';
    while (tokens.length) {
        lastTokenType = tokens[tokens.length - 1][0];
        if (lastTokenType !== 'space' && lastTokenType !== 'comment') break;
        spaces = tokens.pop()[1] + spaces;
    }
    return spaces;
}
```
- example usage
```shell
...

Parser.prototype.rule = function rule(tokens) {
    tokens.pop();

    var node = new _rule2.default();
    this.init(node, tokens[0][2], tokens[0][3]);

    node.raws.between = this.spacesAndCommentsFromEnd(tokens);
    this.raw(node, 'selector', tokens);
    this.current = node;
};

Parser.prototype.decl = function decl(tokens) {
    var node = new _declaration2.default();
    this.init(node);
...
```

#### <a name="apidoc.element.postcss.parser.prototype.spacesAndCommentsFromStart"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>spacesAndCommentsFromStart (tokens)](#apidoc.element.postcss.parser.prototype.spacesAndCommentsFromStart)
- description and source-code
```javascript
function spacesAndCommentsFromStart(tokens) {
    var next = void 0;
    var spaces = '';
    while (tokens.length) {
        next = tokens[0][0];
        if (next !== 'space' && next !== 'comment') break;
        spaces += tokens.shift()[1];
    }
    return spaces;
}
```
- example usage
```shell
...
    }
}

if (node.prop[0] === '_' || node.prop[0] === '*') {
    node.raws.before += node.prop[0];
    node.prop = node.prop.slice(1);
}
node.raws.between += this.spacesAndCommentsFromStart(tokens);
this.precheckMissedSemicolon(tokens);

for (var i = tokens.length - 1; i > 0; i--) {
    token = tokens[i];
    if (token[1] === '!important') {
        node.important = true;
        var string = this.stringFrom(tokens, i);
...
```

#### <a name="apidoc.element.postcss.parser.prototype.spacesFromEnd"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>spacesFromEnd (tokens)](#apidoc.element.postcss.parser.prototype.spacesFromEnd)
- description and source-code
```javascript
function spacesFromEnd(tokens) {
    var lastTokenType = void 0;
    var spaces = '';
    while (tokens.length) {
        lastTokenType = tokens[tokens.length - 1][0];
        if (lastTokenType !== 'space') break;
        spaces = tokens.pop()[1] + spaces;
    }
    return spaces;
}
```
- example usage
```shell
...
this.precheckMissedSemicolon(tokens);

for (var i = tokens.length - 1; i > 0; i--) {
    token = tokens[i];
    if (token[1] === '!important') {
        node.important = true;
        var string = this.stringFrom(tokens, i);
        string = this.spacesFromEnd(tokens) + string;
        if (string !== ' !important') node.raws.important = string;
        break;
    } else if (token[1] === 'important') {
        var cache = tokens.slice(0);
        var str = '';
        for (var j = i; j > 0; j--) {
            var _type = cache[j][0];
...
```

#### <a name="apidoc.element.postcss.parser.prototype.stringFrom"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>stringFrom (tokens, from)](#apidoc.element.postcss.parser.prototype.stringFrom)
- description and source-code
```javascript
function stringFrom(tokens, from) {
    var result = '';
    for (var i = from; i < tokens.length; i++) {
        result += tokens[i][1];
    }
    tokens.splice(from, tokens.length - from);
    return result;
}
```
- example usage
```shell
...
node.raws.between += this.spacesAndCommentsFromStart(tokens);
this.precheckMissedSemicolon(tokens);

for (var i = tokens.length - 1; i > 0; i--) {
    token = tokens[i];
    if (token[1] === '!important') {
        node.important = true;
        var string = this.stringFrom(tokens, i);
        string = this.spacesFromEnd(tokens) + string;
        if (string !== ' !important') node.raws.important = string;
        break;
    } else if (token[1] === 'important') {
        var cache = tokens.slice(0);
        var str = '';
        for (var j = i; j > 0; j--) {
...
```

#### <a name="apidoc.element.postcss.parser.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>tokenize ()](#apidoc.element.postcss.parser.prototype.tokenize)
- description and source-code
```javascript
function tokenize() {
    this.tokens = (0, _tokenize2.default)(this.input);
}
```
- example usage
```shell
...
    throw new Error('Option safe was removed. ' + 'Use parser: require("postcss-safe-parser")');
}

var input = new _input2.default(css, opts);

var parser = new _parser2.default(input);
try {
    parser.tokenize();
    parser.loop();
} catch (e) {
    if (e.name === 'CssSyntaxError' && opts && opts.from) {
        if (/\.scss$/i.test(opts.from)) {
            e.message += '\nYou tried to parse SCSS with ' + 'the standard CSS parser; ' + 'try again with the postcss-scss parser
';
        } else if (/\.less$/i.test(opts.from)) {
            e.message += '\nYou tried to parse Less with ' + 'the standard CSS parser; ' + 'try again with the postcss-less parser
';
...
```

#### <a name="apidoc.element.postcss.parser.prototype.unclosedBlock"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unclosedBlock ()](#apidoc.element.postcss.parser.prototype.unclosedBlock)
- description and source-code
```javascript
function unclosedBlock() {
    var pos = this.current.source.start;
    throw this.input.error('Unclosed block', pos.line, pos.column);
}
```
- example usage
```shell
...
        this.current = this.current.parent;
    } else {
        this.unexpectedClose(token);
    }
};

Parser.prototype.endFile = function endFile() {
    if (this.current.parent) this.unclosedBlock();
    if (this.current.nodes && this.current.nodes.length) {
        this.current.raws.semicolon = this.semicolon;
    }
    this.current.raws.after = (this.current.raws.after || '') + this.spaces;
};

// Helpers
...
```

#### <a name="apidoc.element.postcss.parser.prototype.unclosedBracket"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unclosedBracket (bracket)](#apidoc.element.postcss.parser.prototype.unclosedBracket)
- description and source-code
```javascript
function unclosedBracket(bracket) {
    throw this.input.error('Unclosed bracket', bracket[2], bracket[3]);
}
```
- example usage
```shell
...
    this.pos += 1;
}
if (this.pos === this.tokens.length) {
    this.pos -= 1;
    end = true;
}

if (brackets.length > 0) this.unclosedBracket(bracket);

if (end && colon) {
    while (this.pos > start) {
        token = this.tokens[this.pos][0];
        if (token !== 'space' && token !== 'comment') break;
        this.pos -= 1;
    }
...
```

#### <a name="apidoc.element.postcss.parser.prototype.unexpectedClose"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unexpectedClose (token)](#apidoc.element.postcss.parser.prototype.unexpectedClose)
- description and source-code
```javascript
function unexpectedClose(token) {
    throw this.input.error('Unexpected }', token[2], token[3]);
}
```
- example usage
```shell
...
    this.current.raws.after = (this.current.raws.after || '') + this.spaces;
    this.spaces = '';

    if (this.current.parent) {
        this.current.source.end = { line: token[2], column: token[3] };
        this.current = this.current.parent;
    } else {
        this.unexpectedClose(token);
    }
};

Parser.prototype.endFile = function endFile() {
    if (this.current.parent) this.unclosedBlock();
    if (this.current.nodes && this.current.nodes.length) {
        this.current.raws.semicolon = this.semicolon;
...
```

#### <a name="apidoc.element.postcss.parser.prototype.unknownWord"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unknownWord (start)](#apidoc.element.postcss.parser.prototype.unknownWord)
- description and source-code
```javascript
function unknownWord(start) {
    var token = this.tokens[start];
    throw this.input.error('Unknown word', token[2], token[3]);
}
```
- example usage
```shell
...
        if (token !== 'space' && token !== 'comment') break;
        this.pos -= 1;
    }
    this.decl(this.tokens.slice(start, this.pos + 1));
    return;
}

this.unknownWord(start);
    };

    Parser.prototype.rule = function rule(tokens) {
tokens.pop();

var node = new _rule2.default();
this.init(node, tokens[0][2], tokens[0][3]);
...
```

#### <a name="apidoc.element.postcss.parser.prototype.unnamedAtrule"></a>[function <span class="apidocSignatureSpan">postcss.parser.prototype.</span>unnamedAtrule (node, token)](#apidoc.element.postcss.parser.prototype.unnamedAtrule)
- description and source-code
```javascript
function unnamedAtrule(node, token) {
    throw this.input.error('At-rule without name', token[2], token[3]);
}
```
- example usage
```shell
...
if (node.value.indexOf(':') !== -1) this.checkMissedSemicolon(tokens);
    };

    Parser.prototype.atrule = function atrule(token) {
var node = new _atRule2.default();
node.name = token[1].slice(1);
if (node.name === '') {
    this.unnamedAtrule(node, token);
}
this.init(node, token[2], token[3]);

var last = false;
var open = false;
var params = [];
...
```



# <a name="apidoc.module.postcss.previous_map"></a>[module postcss.previous_map](#apidoc.module.postcss.previous_map)

#### <a name="apidoc.element.postcss.previous_map.previous_map"></a>[function <span class="apidocSignatureSpan">postcss.</span>previous_map (css, opts)](#apidoc.element.postcss.previous_map.previous_map)
- description and source-code
```javascript
function PreviousMap(css, opts) {
    _classCallCheck(this, PreviousMap);

    this.loadAnnotation(css);
<span class="apidocCodeCommentSpan">    /**
     * @member {boolean} - Was source map inlined by data-uri to input CSS.
     */
</span>    this.inline = this.startWith(this.annotation, 'data:');

    var prev = opts.map ? opts.map.prev : undefined;
    var text = this.loadMap(opts.from, prev);
    if (text) this.text = text;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.previous_map.prototype"></a>[module postcss.previous_map.prototype](#apidoc.module.postcss.previous_map.prototype)

#### <a name="apidoc.element.postcss.previous_map.prototype.consumer"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>consumer ()](#apidoc.element.postcss.previous_map.prototype.consumer)
- description and source-code
```javascript
function consumer() {
    if (!this.consumerCache) {
        this.consumerCache = new _sourceMap2.default.SourceMapConsumer(this.text);
    }
    return this.consumerCache;
}
```
- example usage
```shell
...
if (map.text) {
    /**
     * @member {PreviousMap} - The input source map passed from
     *                         a compilation step before PostCSS
     *                         (for example, from Sass compiler).
     *
     * @example
     * root.source.input.map.consumer().sources //=> ['a.sass']
     */
    this.map = map;
    var file = map.consumer().file;
    if (!this.file && file) this.file = this.mapResolve(file);
}

if (!this.file) {
...
```

#### <a name="apidoc.element.postcss.previous_map.prototype.decodeInline"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>decodeInline (text)](#apidoc.element.postcss.previous_map.prototype.decodeInline)
- description and source-code
```javascript
function decodeInline(text) {
    var utfd64 = 'data:application/json;charset=utf-8;base64,';
    var utf64 = 'data:application/json;charset=utf8;base64,';
    var b64 = 'data:application/json;base64,';
    var uri = 'data:application/json,';

    if (this.startWith(text, uri)) {
        return decodeURIComponent(text.substr(uri.length));
    } else if (this.startWith(text, b64)) {
        return _jsBase.Base64.decode(text.substr(b64.length));
    } else if (this.startWith(text, utf64)) {
        return _jsBase.Base64.decode(text.substr(utf64.length));
    } else if (this.startWith(text, utfd64)) {
        return _jsBase.Base64.decode(text.substr(utfd64.length));
    } else {
        var encoding = text.match(/data:application\/json;([^,]+),/)[1];
        throw new Error('Unsupported source map encoding ' + encoding);
    }
}
```
- example usage
```shell
...
    return prev.toString();
} else if (this.isMap(prev)) {
    return JSON.stringify(prev);
} else {
    throw new Error('Unsupported previous source map format: ' + prev.toString());
}
        } else if (this.inline) {
return this.decodeInline(this.annotation);
        } else if (this.annotation) {
var map = this.annotation;
if (file) map = _path2.default.join(_path2.default.dirname(file), map);

this.root = _path2.default.dirname(map);
if (_fs2.default.existsSync && _fs2.default.existsSync(map)) {
    return _fs2.default.readFileSync(map, 'utf-8').toString().trim();
...
```

#### <a name="apidoc.element.postcss.previous_map.prototype.isMap"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>isMap (map)](#apidoc.element.postcss.previous_map.prototype.isMap)
- description and source-code
```javascript
function isMap(map) {
    if ((typeof map === 'undefined' ? 'undefined' : _typeof(map)) !== 'object') return false;
    return typeof map.mappings === 'string' || typeof map._mappings === 'string';
}
```
- example usage
```shell
...
    }
});
    };

    MapGenerator.prototype.generate = function generate() {
this.clearAnnotation();

if (this.isMap()) {
    return this.generateMap();
} else {
    var result = '';
    this.stringify(this.root, function (i) {
        result += i;
    });
    return [result];
...
```

#### <a name="apidoc.element.postcss.previous_map.prototype.loadAnnotation"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>loadAnnotation (css)](#apidoc.element.postcss.previous_map.prototype.loadAnnotation)
- description and source-code
```javascript
function loadAnnotation(css) {
    var match = css.match(/\/\*\s*# sourceMappingURL=(.*)\s*\*\//);
    if (match) this.annotation = match[1].trim();
}
```
- example usage
```shell
...
    /**
     * @param {string}         css    - input CSS source
     * @param {processOptions} [opts] - {@link Processor#process} options
     */
    function PreviousMap(css, opts) {
_classCallCheck(this, PreviousMap);

this.loadAnnotation(css);
/**
 * @member {boolean} - Was source map inlined by data-uri to input CSS.
 */
this.inline = this.startWith(this.annotation, 'data:');

var prev = opts.map ? opts.map.prev : undefined;
var text = this.loadMap(opts.from, prev);
...
```

#### <a name="apidoc.element.postcss.previous_map.prototype.loadMap"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>loadMap (file, prev)](#apidoc.element.postcss.previous_map.prototype.loadMap)
- description and source-code
```javascript
function loadMap(file, prev) {
    if (prev === false) return false;

    if (prev) {
        if (typeof prev === 'string') {
            return prev;
        } else if (typeof prev === 'function') {
            var prevPath = prev(file);
            if (prevPath && _fs2.default.existsSync && _fs2.default.existsSync(prevPath)) {
                return _fs2.default.readFileSync(prevPath, 'utf-8').toString().trim();
            } else {
                throw new Error('Unable to load previous source map: ' + prevPath.toString());
            }
        } else if (prev instanceof _sourceMap2.default.SourceMapConsumer) {
            return _sourceMap2.default.SourceMapGenerator.fromSourceMap(prev).toString();
        } else if (prev instanceof _sourceMap2.default.SourceMapGenerator) {
            return prev.toString();
        } else if (this.isMap(prev)) {
            return JSON.stringify(prev);
        } else {
            throw new Error('Unsupported previous source map format: ' + prev.toString());
        }
    } else if (this.inline) {
        return this.decodeInline(this.annotation);
    } else if (this.annotation) {
        var map = this.annotation;
        if (file) map = _path2.default.join(_path2.default.dirname(file), map);

        this.root = _path2.default.dirname(map);
        if (_fs2.default.existsSync && _fs2.default.existsSync(map)) {
            return _fs2.default.readFileSync(map, 'utf-8').toString().trim();
        } else {
            return false;
        }
    }
}
```
- example usage
```shell
...
    this.loadAnnotation(css);
    /**
     * @member {boolean} - Was source map inlined by data-uri to input CSS.
     */
    this.inline = this.startWith(this.annotation, 'data:');

    var prev = opts.map ? opts.map.prev : undefined;
    var text = this.loadMap(opts.from, prev);
    if (text) this.text = text;
}

/**
 * Create a instance of 'SourceMapGenerator' class
 * from the 'source-map' library to work with source map information.
 *
...
```

#### <a name="apidoc.element.postcss.previous_map.prototype.startWith"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>startWith (string, start)](#apidoc.element.postcss.previous_map.prototype.startWith)
- description and source-code
```javascript
function startWith(string, start) {
    if (!string) return false;
    return string.substr(0, start.length) === start;
}
```
- example usage
```shell
...
function PreviousMap(css, opts) {
    _classCallCheck(this, PreviousMap);

    this.loadAnnotation(css);
    /**
     * @member {boolean} - Was source map inlined by data-uri to input CSS.
     */
    this.inline = this.startWith(this.annotation, 'data:');

    var prev = opts.map ? opts.map.prev : undefined;
    var text = this.loadMap(opts.from, prev);
    if (text) this.text = text;
}

/**
...
```

#### <a name="apidoc.element.postcss.previous_map.prototype.withContent"></a>[function <span class="apidocSignatureSpan">postcss.previous_map.prototype.</span>withContent ()](#apidoc.element.postcss.previous_map.prototype.withContent)
- description and source-code
```javascript
function withContent() {
    return !!(this.consumer().sourcesContent && this.consumer().sourcesContent.length > 0);
}
```
- example usage
```shell
...

MapGenerator.prototype.isSourcesContent = function isSourcesContent() {
    if (typeof this.mapOpts.sourcesContent !== 'undefined') {
        return this.mapOpts.sourcesContent;
    }
    if (this.previous().length) {
        return this.previous().some(function (i) {
            return i.withContent();
        });
    } else {
        return true;
    }
};

MapGenerator.prototype.clearAnnotation = function clearAnnotation() {
...
```



# <a name="apidoc.module.postcss.processor"></a>[module postcss.processor](#apidoc.module.postcss.processor)

#### <a name="apidoc.element.postcss.processor.processor"></a>[function <span class="apidocSignatureSpan">postcss.</span>processor ()](#apidoc.element.postcss.processor.processor)
- description and source-code
```javascript
function Processor() {
  var plugins = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : [];

  _classCallCheck(this, Processor);

<span class="apidocCodeCommentSpan">  /**
   * @member {string} - Current PostCSS version.
   *
   * @example
   * if ( result.processor.version.split('.')[0] !== '5' ) {
   *   throw new Error('This plugin works only with PostCSS 5');
   * }
   */
</span>  this.version = '5.2.16';
  /**
   * @member {pluginFunction[]} - Plugins added to this processor.
   *
   * @example
   * const processor = postcss([autoprefixer, precss]);
   * processor.plugins.length //=> 2
   */
  this.plugins = this.normalize(plugins);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.processor.prototype"></a>[module postcss.processor.prototype](#apidoc.module.postcss.processor.prototype)

#### <a name="apidoc.element.postcss.processor.prototype.normalize"></a>[function <span class="apidocSignatureSpan">postcss.processor.prototype.</span>normalize (plugins)](#apidoc.element.postcss.processor.prototype.normalize)
- description and source-code
```javascript
function normalize(plugins) {
  var normalized = [];
  for (var _iterator = plugins, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator[Symbol
.iterator]();;) {
    var _ref;

    if (_isArray) {
      if (_i >= _iterator.length) break;
      _ref = _iterator[_i++];
    } else {
      _i = _iterator.next();
      if (_i.done) break;
      _ref = _i.value;
    }

    var i = _ref;

    if (i.postcss) i = i.postcss;

    if ((typeof i === 'undefined' ? 'undefined' : _typeof(i)) === 'object' && Array.isArray(i.plugins)) {
      normalized = normalized.concat(i.plugins);
    } else if (typeof i === 'function') {
      normalized.push(i);
    } else if ((typeof i === 'undefined' ? 'undefined' : _typeof(i)) === 'object' && (i.parse || i.stringify)) {
      throw new Error('PostCSS syntaxes cannot be used as plugins. ' + 'Instead, please use one of the ' + 'syntax/parser/stringifier
 options as ' + 'outlined in your PostCSS ' + 'runner documentation.');
    } else {
      throw new Error(i + ' is not a PostCSS plugin');
    }
  }
  return normalized;
}
```
- example usage
```shell
...
_i = _iterator.next();
if (_i.done) break;
_ref = _i.value;
            }

            var child = _ref;

            var nodes = this.normalize(child, this.last);
            for (var _iterator2 = nodes, _isArray2 = Array.isArray(_iterator2), _i2 = 0, _iterator2 = _isArray2 ? _iterator2 : _iterator2
[Symbol.iterator]();;) {
var _ref2;

if (_isArray2) {
    if (_i2 >= _iterator2.length) break;
    _ref2 = _iterator2[_i2++];
} else {
...
```

#### <a name="apidoc.element.postcss.processor.prototype.process"></a>[function <span class="apidocSignatureSpan">postcss.processor.prototype.</span>process (css)](#apidoc.element.postcss.processor.prototype.process)
- description and source-code
```javascript
function process(css) {
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  return new _lazyResult2.default(this, css, opts);
}
```
- example usage
```shell
...
'''js
const postcss = require('postcss');
const precss = require('precss');
const autoprefixer = require('autoprefixer');

fs.readFile('src/app.css', (err, css) => {
    postcss([precss, autoprefixer])
        .process(css, { from: 'src/app.css', to: 'dest/app.css' })
        .then(result => {
            fs.writeFile('dest/app.css', result.css);
            if ( result.map ) fs.writeFile('dest/app.css.map', result.map);
        });
});
'''
...
```

#### <a name="apidoc.element.postcss.processor.prototype.use"></a>[function <span class="apidocSignatureSpan">postcss.processor.prototype.</span>use (plugin)](#apidoc.element.postcss.processor.prototype.use)
- description and source-code
```javascript
function use(plugin) {
  this.plugins = this.plugins.concat(this.normalize([plugin]));
  return this;
}
```
- example usage
```shell
...
 *
 * @param {Plugin|pluginFunction|Processor} plugin - PostCSS plugin
 *                                                   or {@link Processor}
 *                                                   with plugins
 *
 * @example
 * const processor = postcss()
 *   .use(autoprefixer)
 *   .use(precss);
 *
 * @return {Processes} current processor to make methods chain
 */


Processor.prototype.use = function use(plugin) {
...
```



# <a name="apidoc.module.postcss.result"></a>[module postcss.result](#apidoc.module.postcss.result)

#### <a name="apidoc.element.postcss.result.result"></a>[function <span class="apidocSignatureSpan">postcss.</span>result (processor, root, opts)](#apidoc.element.postcss.result.result)
- description and source-code
```javascript
function Result(processor, root, opts) {
  _classCallCheck(this, Result);

<span class="apidocCodeCommentSpan">  /**
   * @member {Processor} - The Processor instance used
   *                       for this transformation.
   *
   * @example
   * for ( let plugin of result.processor.plugins) {
   *   if ( plugin.postcssPlugin === 'postcss-bad' ) {
   *     throw 'postcss-good is incompatible with postcss-bad';
   *   }
   * });
   */
</span>  this.processor = processor;
  /**
   * @member {Message[]} - Contains messages from plugins
   *                       (e.g., warnings or custom messages).
   *                       Each message should have type
   *                       and plugin properties.
   *
   * @example
   * postcss.plugin('postcss-min-browser', () => {
   *   return (root, result) => {
   *     var browsers = detectMinBrowsersByCanIUse(root);
   *     result.messages.push({
   *       type:    'min-browser',
   *       plugin:  'postcss-min-browser',
   *       browsers: browsers
   *     });
   *   };
   * });
   */
  this.messages = [];
  /**
   * @member {Root} - Root node after all transformations.
   *
   * @example
   * root.toResult().root == root;
   */
  this.root = root;
  /**
   * @member {processOptions} - Options from the {@link Processor#process}
   *                            or {@link Root#toResult} call
   *                            that produced this Result instance.
   *
   * @example
   * root.toResult(opts).opts == opts;
   */
  this.opts = opts;
  /**
   * @member {string} - A CSS string representing of {@link Result#root}.
   *
   * @example
   * postcss.parse('a{}').toResult().css //=> "a{}"
   */
  this.css = undefined;
  /**
   * @member {SourceMapGenerator} - An instance of 'SourceMapGenerator'
   *                                class from the 'source-map' library,
   *                                representing changes
   *                                to the {@link Result#root} instance.
   *
   * @example
   * result.map.toJSON() //=> { version: 3, file: 'a.css', … }
   *
   * @example
   * if ( result.map ) {
   *   fs.writeFileSync(result.opts.to + '.map', result.map.toString());
   * }
   */
  this.map = undefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.result.prototype"></a>[module postcss.result.prototype](#apidoc.module.postcss.result.prototype)

#### <a name="apidoc.element.postcss.result.prototype.toString"></a>[function <span class="apidocSignatureSpan">postcss.result.prototype.</span>toString ()](#apidoc.element.postcss.result.prototype.toString)
- description and source-code
```javascript
function toString() {
  return this.css;
}
```
- example usage
```shell
...
    }).join('\n');
};

/**
 * Returns error position, message and source code of the broken part.
 *
 * @example
 * error.toString() //=> "CssSyntaxError: app.css:1:1: Unclosed block
 *                  //    > 1 | a {
 *                  //        | ^"
 *
 * @return {string} error position, message and source code
 */
...
```

#### <a name="apidoc.element.postcss.result.prototype.warn"></a>[function <span class="apidocSignatureSpan">postcss.result.prototype.</span>warn (text)](#apidoc.element.postcss.result.prototype.warn)
- description and source-code
```javascript
function warn(text) {
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  if (!opts.plugin) {
    if (this.lastPlugin && this.lastPlugin.postcssPlugin) {
      opts.plugin = this.lastPlugin.postcssPlugin;
    }
  }

  var warning = new _warning2.default(text, opts);
  this.messages.push(warning);

  return warning;
}
```
- example usage
```shell
...
 *
 * @return {Warning} created warning object
 *
 * @example
 * const plugin = postcss.plugin('postcss-deprecated', () => {
 *   return (root, result) => {
 *     root.walkDecls('bad', decl => {
 *       decl.warn(result, 'Deprecated property bad');
 *     });
 *   };
 * });
 */


Node.prototype.warn = function warn(result, text, opts) {
...
```

#### <a name="apidoc.element.postcss.result.prototype.warnings"></a>[function <span class="apidocSignatureSpan">postcss.result.prototype.</span>warnings ()](#apidoc.element.postcss.result.prototype.warnings)
- description and source-code
```javascript
function warnings() {
  return this.messages.filter(function (i) {
    return i.type === 'warning';
  });
}
```
- example usage
```shell
...
/**
 * Processes input CSS through synchronous plugins
 * and calls {@link Result#warnings()}.
 *
 * @return {Warning[]} warnings from plugins
 */
LazyResult.prototype.warnings = function warnings() {
    return this.sync().warnings();
};

/**
 * Alias for the {@link LazyResult#css} property.
 *
 * @example
 * lazy + '' === lazy.css;
...
```



# <a name="apidoc.module.postcss.root"></a>[module postcss.root](#apidoc.module.postcss.root)

#### <a name="apidoc.element.postcss.root.root"></a>[function <span class="apidocSignatureSpan">postcss.</span>root (defaults)](#apidoc.element.postcss.root.root)
- description and source-code
```javascript
function Root(defaults) {
    _classCallCheck(this, Root);

    var _this = _possibleConstructorReturn(this, _Container.call(this, defaults));

    _this.type = 'root';
    if (!_this.nodes) _this.nodes = [];
    return _this;
}
```
- example usage
```shell
...
 * It will also clean the 'between' property
 * if 'newParent' is in another {@link Root}.
 *
 * @param {Container} newParent - container node where the current node
 *                                will be moved
 *
 * @example
 * atrule.moveTo(atrule.root());
 *
 * @return {Node} current node to methods chain
 */


Node.prototype.moveTo = function moveTo(newParent) {
    this.cleanRaws(this.root() === newParent.root());
...
```



# <a name="apidoc.module.postcss.root.prototype"></a>[module postcss.root.prototype](#apidoc.module.postcss.root.prototype)

#### <a name="apidoc.element.postcss.root.prototype.normalize"></a>[function <span class="apidocSignatureSpan">postcss.root.prototype.</span>normalize (child, sample, type)](#apidoc.element.postcss.root.prototype.normalize)
- description and source-code
```javascript
function normalize(child, sample, type) {
    var nodes = _Container.prototype.normalize.call(this, child);

    if (sample) {
        if (type === 'prepend') {
            if (this.nodes.length > 1) {
                sample.raws.before = this.nodes[1].raws.before;
            } else {
                delete sample.raws.before;
            }
        } else if (this.first !== sample) {
            for (var _iterator = nodes, _isArray = Array.isArray(_iterator), _i = 0, _iterator = _isArray ? _iterator : _iterator
[Symbol.iterator]();;) {
                var _ref;

                if (_isArray) {
                    if (_i >= _iterator.length) break;
                    _ref = _iterator[_i++];
                } else {
                    _i = _iterator.next();
                    if (_i.done) break;
                    _ref = _i.value;
                }

                var node = _ref;

                node.raws.before = sample.raws.before;
            }
        }
    }

    return nodes;
}
```
- example usage
```shell
...
_i = _iterator.next();
if (_i.done) break;
_ref = _i.value;
            }

            var child = _ref;

            var nodes = this.normalize(child, this.last);
            for (var _iterator2 = nodes, _isArray2 = Array.isArray(_iterator2), _i2 = 0, _iterator2 = _isArray2 ? _iterator2 : _iterator2
[Symbol.iterator]();;) {
var _ref2;

if (_isArray2) {
    if (_i2 >= _iterator2.length) break;
    _ref2 = _iterator2[_i2++];
} else {
...
```

#### <a name="apidoc.element.postcss.root.prototype.prevMap"></a>[function <span class="apidocSignatureSpan">postcss.root.prototype.</span>prevMap ()](#apidoc.element.postcss.root.prototype.prevMap)
- description and source-code
```javascript
function prevMap() {
    (0, _warnOnce2.default)('Root#prevMap is deprecated. Use Root#source.input.map');
    return this.source.input.map;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.root.prototype.remove"></a>[function <span class="apidocSignatureSpan">postcss.root.prototype.</span>remove (child)](#apidoc.element.postcss.root.prototype.remove)
- description and source-code
```javascript
function remove(child) {
    (0, _warnOnce2.default)('Root#remove is deprecated. Use Root#removeChild');
    this.removeChild(child);
}
```
- example usage
```shell
...
*
* @example
* root.walkDecls(decl => {
*   checkPropertySupport(decl.prop);
* });
*
* root.walkDecls('border-radius', decl => {
*   decl.remove();
* });
*
* root.walkDecls(/^background/, decl => {
*   decl.value = takeFirstColorFromGradient(decl.value);
* });
*/
...
```

#### <a name="apidoc.element.postcss.root.prototype.removeChild"></a>[function <span class="apidocSignatureSpan">postcss.root.prototype.</span>removeChild (child)](#apidoc.element.postcss.root.prototype.removeChild)
- description and source-code
```javascript
function removeChild(child) {
    child = this.index(child);

    if (child === 0 && this.nodes.length > 1) {
        this.nodes[1].raws.before = this.nodes[child].raws.before;
    }

    return _Container.prototype.removeChild.call(this, child);
}
```
- example usage
```shell
...

    return this;
};

Container.prototype.remove = function remove(child) {
    if (typeof child !== 'undefined') {
        (0, _warnOnce2.default)('Container#remove is deprecated. ' + 'Use Container#removeChild');
        this.removeChild(child);
    } else {
        _Node.prototype.remove.call(this);
    }
    return this;
};

/**
...
```

#### <a name="apidoc.element.postcss.root.prototype.toResult"></a>[function <span class="apidocSignatureSpan">postcss.root.prototype.</span>toResult ()](#apidoc.element.postcss.root.prototype.toResult)
- description and source-code
```javascript
function toResult() {
    var opts = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

    var LazyResult = require('./lazy-result');
    var Processor = require('./processor');

    var lazy = new LazyResult(new Processor(), this, opts);
    return lazy.stringify();
}
```
- example usage
```shell
...
 *
 * @example
 * postcss([cssnext]).process(css).then(function (result) {
 *    console.log(result.css);
 * });
 *
 * @example
 * var result2 = postcss.parse(css).toResult();
 */
var Result = function () {

/**
 * @param {Processor} processor - processor used for this transformation.
 * @param {Root}      root      - Root node after all transformations.
 * @param {processOptions} opts - options from the {@link Processor#process}
...
```



# <a name="apidoc.module.postcss.stringifier"></a>[module postcss.stringifier](#apidoc.module.postcss.stringifier)

#### <a name="apidoc.element.postcss.stringifier.stringifier"></a>[function <span class="apidocSignatureSpan">postcss.</span>stringifier (builder)](#apidoc.element.postcss.stringifier.stringifier)
- description and source-code
```javascript
function Stringifier(builder) {
    _classCallCheck(this, Stringifier);

    this.builder = builder;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.stringifier.prototype"></a>[module postcss.stringifier.prototype](#apidoc.module.postcss.stringifier.prototype)

#### <a name="apidoc.element.postcss.stringifier.prototype.atrule"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>atrule (node, semicolon)](#apidoc.element.postcss.stringifier.prototype.atrule)
- description and source-code
```javascript
function atrule(node, semicolon) {
    var name = '@' + node.name;
    var params = node.params ? this.rawValue(node, 'params') : '';

    if (typeof node.raws.afterName !== 'undefined') {
        name += node.raws.afterName;
    } else if (params) {
        name += ' ';
    }

    if (node.nodes) {
        this.block(node, name + params);
    } else {
        var end = (node.raws.between || '') + (semicolon ? ';' : '');
        this.builder(name + params + end, node);
    }
}
```
- example usage
```shell
...
    break;

case 'comment':
    this.comment(token);
    break;

case 'at-word':
    this.atrule(token);
    break;

case '{':
    this.emptyRule(token);
    break;

default:
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.beforeAfter"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>beforeAfter (node, detect)](#apidoc.element.postcss.stringifier.prototype.beforeAfter)
- description and source-code
```javascript
function beforeAfter(node, detect) {
    var value = void 0;
    if (node.type === 'decl') {
        value = this.raw(node, null, 'beforeDecl');
    } else if (node.type === 'comment') {
        value = this.raw(node, null, 'beforeComment');
    } else if (detect === 'before') {
        value = this.raw(node, null, 'beforeRule');
    } else {
        value = this.raw(node, null, 'beforeClose');
    }

    var buf = node.parent;
    var depth = 0;
    while (buf && buf.type !== 'root') {
        depth += 1;
        buf = buf.parent;
    }

    if (value.indexOf('\n') !== -1) {
        var indent = this.raw(node, null, 'indent');
        if (indent.length) {
            for (var step = 0; step < depth; step++) {
                value += indent;
            }
        }
    }

    return value;
}
```
- example usage
```shell
...
var root = node.root();
if (!root.rawCache) root.rawCache = {};
if (typeof root.rawCache[detect] !== 'undefined') {
    return root.rawCache[detect];
}

if (detect === 'before' || detect === 'after') {
    return this.beforeAfter(node, detect);
} else {
    var method = 'raw' + capitalize(detect);
    if (this[method]) {
        value = this[method](root, node);
    } else {
        root.walk(function (i) {
            value = i.raws[own];
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.block"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>block (node, start)](#apidoc.element.postcss.stringifier.prototype.block)
- description and source-code
```javascript
function block(node, start) {
    var between = this.raw(node, 'between', 'beforeOpen');
    this.builder(start + between + '{', node, 'start');

    var after = void 0;
    if (node.nodes && node.nodes.length) {
        this.body(node);
        after = this.raw(node, 'after');
    } else {
        after = this.raw(node, 'after', 'emptyBody');
    }

    if (after) this.builder(after);
    this.builder('}', node, 'end');
}
```
- example usage
```shell
...
}

if (semicolon) string += ';';
this.builder(string, node);
    };

    Stringifier.prototype.rule = function rule(node) {
this.block(node, this.rawValue(node, 'selector'));
    };

    Stringifier.prototype.atrule = function atrule(node, semicolon) {
var name = '@' + node.name;
var params = node.params ? this.rawValue(node, 'params') : '';

if (typeof node.raws.afterName !== 'undefined') {
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.body"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>body (node)](#apidoc.element.postcss.stringifier.prototype.body)
- description and source-code
```javascript
function body(node) {
    var last = node.nodes.length - 1;
    while (last > 0) {
        if (node.nodes[last].type !== 'comment') break;
        last -= 1;
    }

    var semicolon = this.raw(node, 'semicolon');
    for (var i = 0; i < node.nodes.length; i++) {
        var child = node.nodes[i];
        var before = this.raw(child, 'before');
        if (before) this.builder(before);
        this.stringify(child, last !== i || semicolon);
    }
}
```
- example usage
```shell
...
}

Stringifier.prototype.stringify = function stringify(node, semicolon) {
    this[node.type](node, semicolon);
};

Stringifier.prototype.root = function root(node) {
    this.body(node);
    if (node.raws.after) this.builder(node.raws.after);
};

Stringifier.prototype.comment = function comment(node) {
    var left = this.raw(node, 'left', 'commentLeft');
    var right = this.raw(node, 'right', 'commentRight');
    this.builder('/*' + left + node.text + right + '*/', node);
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.comment"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>comment (node)](#apidoc.element.postcss.stringifier.prototype.comment)
- description and source-code
```javascript
function comment(node) {
    var left = this.raw(node, 'left', 'commentLeft');
    var right = this.raw(node, 'right', 'commentRight');
    this.builder('/*' + left + node.text + right + '*/', node);
}
```
- example usage
```shell
...
    break;

case '}':
    this.end(token);
    break;

case 'comment':
    this.comment(token);
    break;

case 'at-word':
    this.atrule(token);
    break;

case '{':
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.decl"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>decl (node, semicolon)](#apidoc.element.postcss.stringifier.prototype.decl)
- description and source-code
```javascript
function decl(node, semicolon) {
    var between = this.raw(node, 'between', 'colon');
    var string = node.prop + between + this.rawValue(node, 'value');

    if (node.important) {
        string += node.raws.important || ' !important';
    }

    if (semicolon) string += ';';
    this.builder(string, node);
}
```
- example usage
```shell
...
* Inserts new nodes to the end of the container.
*
* @param {...(Node|object|string|Node[])} children - new nodes
*
* @return {Node} this node for methods chain
*
* @example
* const decl1 = postcss.decl({ prop: 'color', value: 'black' });
* const decl2 = postcss.decl({ prop: 'background-color', value: 'white' });
* rule.append(decl1, decl2);
*
* root.append({ name: 'charset', params: '"UTF-8"' });  // at-rule
* root.append({ selector: 'a' });                       // rule
* rule.append({ prop: 'color', value: 'black' });       // declaration
* rule.append({ text: 'Comment' })                      // comment
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.raw"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>raw (node, own, detect)](#apidoc.element.postcss.stringifier.prototype.raw)
- description and source-code
```javascript
function raw(node, own, detect) {
    var value = void 0;
    if (!detect) detect = own;

    // Already had
    if (own) {
        value = node.raws[own];
        if (typeof value !== 'undefined') return value;
    }

    var parent = node.parent;

    // Hack for first rule in CSS
    if (detect === 'before') {
        if (!parent || parent.type === 'root' && parent.first === node) {
            return '';
        }
    }

    // Floating child without parent
    if (!parent) return defaultRaw[detect];

    // Detect style by other nodes
    var root = node.root();
    if (!root.rawCache) root.rawCache = {};
    if (typeof root.rawCache[detect] !== 'undefined') {
        return root.rawCache[detect];
    }

    if (detect === 'before' || detect === 'after') {
        return this.beforeAfter(node, detect);
    } else {
        var method = 'raw' + capitalize(detect);
        if (this[method]) {
            value = this[method](root, node);
        } else {
            root.walk(function (i) {
                value = i.raws[own];
                if (typeof value !== 'undefined') return false;
            });
        }
    }

    if (typeof value === 'undefined') value = defaultRaw[detect];

    root.rawCache[detect] = value;
    return value;
}
```
- example usage
```shell
...
 * @param {string} [defaultType] - name of default value, it can be missed
 *                                 if the value is the same as prop
 *
 * @example
 * const root = postcss.parse('a { background: white }');
 * root.nodes[0].append({ prop: 'color', value: 'black' });
 * root.nodes[0].nodes[1].raws.before   //=> undefined
 * root.nodes[0].nodes[1].raw('before') //=> ' '
 *
 * @return {string} code style value
 */


Node.prototype.raw = function raw(prop, defaultType) {
    var str = new _stringifier2.default();
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawBeforeClose"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeClose (root)](#apidoc.element.postcss.stringifier.prototype.rawBeforeClose)
- description and source-code
```javascript
function rawBeforeClose(root) {
    var value = void 0;
    root.walk(function (i) {
        if (i.nodes && i.nodes.length > 0) {
            if (typeof i.raws.after !== 'undefined') {
                value = i.raws.after;
                if (value.indexOf('\n') !== -1) {
                    value = value.replace(/[^\n]+$/, '');
                }
                return false;
            }
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawBeforeComment"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeComment (root, node)](#apidoc.element.postcss.stringifier.prototype.rawBeforeComment)
- description and source-code
```javascript
function rawBeforeComment(root, node) {
    var value = void 0;
    root.walkComments(function (i) {
        if (typeof i.raws.before !== 'undefined') {
            value = i.raws.before;
            if (value.indexOf('\n') !== -1) {
                value = value.replace(/[^\n]+$/, '');
            }
            return false;
        }
    });
    if (typeof value === 'undefined') {
        value = this.raw(node, null, 'beforeDecl');
    }
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawBeforeDecl"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeDecl (root, node)](#apidoc.element.postcss.stringifier.prototype.rawBeforeDecl)
- description and source-code
```javascript
function rawBeforeDecl(root, node) {
    var value = void 0;
    root.walkDecls(function (i) {
        if (typeof i.raws.before !== 'undefined') {
            value = i.raws.before;
            if (value.indexOf('\n') !== -1) {
                value = value.replace(/[^\n]+$/, '');
            }
            return false;
        }
    });
    if (typeof value === 'undefined') {
        value = this.raw(node, null, 'beforeRule');
    }
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawBeforeOpen"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeOpen (root)](#apidoc.element.postcss.stringifier.prototype.rawBeforeOpen)
- description and source-code
```javascript
function rawBeforeOpen(root) {
    var value = void 0;
    root.walk(function (i) {
        if (i.type !== 'decl') {
            value = i.raws.between;
            if (typeof value !== 'undefined') return false;
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawBeforeRule"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawBeforeRule (root)](#apidoc.element.postcss.stringifier.prototype.rawBeforeRule)
- description and source-code
```javascript
function rawBeforeRule(root) {
    var value = void 0;
    root.walk(function (i) {
        if (i.nodes && (i.parent !== root || root.first !== i)) {
            if (typeof i.raws.before !== 'undefined') {
                value = i.raws.before;
                if (value.indexOf('\n') !== -1) {
                    value = value.replace(/[^\n]+$/, '');
                }
                return false;
            }
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawColon"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawColon (root)](#apidoc.element.postcss.stringifier.prototype.rawColon)
- description and source-code
```javascript
function rawColon(root) {
    var value = void 0;
    root.walkDecls(function (i) {
        if (typeof i.raws.between !== 'undefined') {
            value = i.raws.between.replace(/[^\s:]/g, '');
            return false;
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawEmptyBody"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawEmptyBody (root)](#apidoc.element.postcss.stringifier.prototype.rawEmptyBody)
- description and source-code
```javascript
function rawEmptyBody(root) {
    var value = void 0;
    root.walk(function (i) {
        if (i.nodes && i.nodes.length === 0) {
            value = i.raws.after;
            if (typeof value !== 'undefined') return false;
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawIndent"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawIndent (root)](#apidoc.element.postcss.stringifier.prototype.rawIndent)
- description and source-code
```javascript
function rawIndent(root) {
    if (root.raws.indent) return root.raws.indent;
    var value = void 0;
    root.walk(function (i) {
        var p = i.parent;
        if (p && p !== root && p.parent && p.parent === root) {
            if (typeof i.raws.before !== 'undefined') {
                var parts = i.raws.before.split('\n');
                value = parts[parts.length - 1];
                value = value.replace(/[^\s]/g, '');
                return false;
            }
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawSemicolon"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawSemicolon (root)](#apidoc.element.postcss.stringifier.prototype.rawSemicolon)
- description and source-code
```javascript
function rawSemicolon(root) {
    var value = void 0;
    root.walk(function (i) {
        if (i.nodes && i.nodes.length && i.last.type === 'decl') {
            value = i.raws.semicolon;
            if (typeof value !== 'undefined') return false;
        }
    });
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rawValue"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rawValue (node, prop)](#apidoc.element.postcss.stringifier.prototype.rawValue)
- description and source-code
```javascript
function rawValue(node, prop) {
    var value = node[prop];
    var raw = node.raws[prop];
    if (raw && raw.value === value) {
        return raw.raw;
    } else {
        return value;
    }
}
```
- example usage
```shell
...
var left = this.raw(node, 'left', 'commentLeft');
var right = this.raw(node, 'right', 'commentRight');
this.builder('/*' + left + node.text + right + '*/', node);
    };

    Stringifier.prototype.decl = function decl(node, semicolon) {
var between = this.raw(node, 'between', 'colon');
var string = node.prop + between + this.rawValue(node, 'value');

if (node.important) {
    string += node.raws.important || ' !important';
}

if (semicolon) string += ';';
this.builder(string, node);
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.root"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>root (node)](#apidoc.element.postcss.stringifier.prototype.root)
- description and source-code
```javascript
function root(node) {
    this.body(node);
    if (node.raws.after) this.builder(node.raws.after);
}
```
- example usage
```shell
...
 * It will also clean the 'between' property
 * if 'newParent' is in another {@link Root}.
 *
 * @param {Container} newParent - container node where the current node
 *                                will be moved
 *
 * @example
 * atrule.moveTo(atrule.root());
 *
 * @return {Node} current node to methods chain
 */


Node.prototype.moveTo = function moveTo(newParent) {
    this.cleanRaws(this.root() === newParent.root());
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.rule"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>rule (node)](#apidoc.element.postcss.stringifier.prototype.rule)
- description and source-code
```javascript
function rule(node) {
    this.block(node, this.rawValue(node, 'selector'));
}
```
- example usage
```shell
...
     *
     * @param {stringifier|syntax} [stringifier] - a syntax to use
     *                                             in string generation
     *
     * @return {string} CSS string of this node
     *
     * @example
     * postcss.rule({ selector: 'a' }).toString() //=> "a {}"
     */


    Node.prototype.toString = function toString() {
var stringifier = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : _stringify2.default;

if (stringifier.stringify) stringifier = stringifier.stringify;
...
```

#### <a name="apidoc.element.postcss.stringifier.prototype.stringify"></a>[function <span class="apidocSignatureSpan">postcss.stringifier.prototype.</span>stringify (node, semicolon)](#apidoc.element.postcss.stringifier.prototype.stringify)
- description and source-code
```javascript
function stringify(node, semicolon) {
    this[node.type](node, semicolon);
}
```
- example usage
```shell
...
var _this2 = this;

if (this.processed) {
    return new Promise(function (resolve, reject) {
        if (_this2.error) {
            reject(_this2.error);
        } else {
            resolve(_this2.stringify());
        }
    });
}
if (this.processing) {
    return this.processing;
}
...
```



# <a name="apidoc.module.postcss.vendor"></a>[module postcss.vendor](#apidoc.module.postcss.vendor)

#### <a name="apidoc.element.postcss.vendor.prefix"></a>[function <span class="apidocSignatureSpan">postcss.vendor.</span>prefix (prop)](#apidoc.element.postcss.vendor.prefix)
- description and source-code
```javascript
function prefix(prop) {
    var match = prop.match(/^(-\w+-)/);
    if (match) {
        return match[0];
    } else {
        return '';
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.postcss.vendor.unprefixed"></a>[function <span class="apidocSignatureSpan">postcss.vendor.</span>unprefixed (prop)](#apidoc.element.postcss.vendor.unprefixed)
- description and source-code
```javascript
function unprefixed(prop) {
    return prop.replace(/^-\w+-/, '');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.warning"></a>[module postcss.warning](#apidoc.module.postcss.warning)

#### <a name="apidoc.element.postcss.warning.warning"></a>[function <span class="apidocSignatureSpan">postcss.</span>warning (text)](#apidoc.element.postcss.warning.warning)
- description and source-code
```javascript
function Warning(text) {
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  _classCallCheck(this, Warning);

<span class="apidocCodeCommentSpan">  /**
   * @member {string} - Type to filter warnings from
   *                    {@link Result#messages}. Always equal
   *                    to '"warning"'.
   *
   * @example
   * const nonWarning = result.messages.filter(i => i.type !== 'warning')
   */
</span>  this.type = 'warning';
  /**
   * @member {string} - The warning message.
   *
   * @example
   * warning.text //=> 'Try to avoid !important'
   */
  this.text = text;

  if (opts.node && opts.node.source) {
    var pos = opts.node.positionBy(opts);
    /**
     * @member {number} - Line in the input file
     *                    with this warning’s source
     *
     * @example
     * warning.line //=> 5
     */
    this.line = pos.line;
    /**
     * @member {number} - Column in the input file
     *                    with this warning’s source.
     *
     * @example
     * warning.column //=> 6
     */
    this.column = pos.column;
  }

  for (var opt in opts) {
    this[opt] = opts[opt];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss.warning.prototype"></a>[module postcss.warning.prototype](#apidoc.module.postcss.warning.prototype)

#### <a name="apidoc.element.postcss.warning.prototype.toString"></a>[function <span class="apidocSignatureSpan">postcss.warning.prototype.</span>toString ()](#apidoc.element.postcss.warning.prototype.toString)
- description and source-code
```javascript
function toString() {
  if (this.node) {
    return this.node.error(this.text, {
      plugin: this.plugin,
      index: this.index,
      word: this.word
    }).message;
  } else if (this.plugin) {
    return this.plugin + ': ' + this.text;
  } else {
    return this.text;
  }
}
```
- example usage
```shell
...
    }).join('\n');
};

/**
 * Returns error position, message and source code of the broken part.
 *
 * @example
 * error.toString() //=> "CssSyntaxError: app.css:1:1: Unclosed block
 *                  //    > 1 | a {
 *                  //        | ^"
 *
 * @return {string} error position, message and source code
 */
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
