# npmdoc-katex

#### api documentation for  [katex (v0.7.1)](https://github.com/Khan/KaTeX#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-katex.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-katex) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-katex.svg)](https://travis-ci.org/npmdoc/node-npmdoc-katex)

#### Fast math typesetting for the web.

[![NPM](https://nodei.co/npm/katex.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/katex)

- [https://npmdoc.github.io/node-npmdoc-katex/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-katex/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-katex/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-katex/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-katex/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-katex/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "katex": "cli.js"
    },
    "bugs": {
        "url": "https://github.com/Khan/KaTeX/issues"
    },
    "dependencies": {
        "match-at": "^0.1.0"
    },
    "description": "Fast math typesetting for the web.",
    "devDependencies": {
        "browserify": "^10.2.4",
        "clean-css": "~2.2.15",
        "eslint": "^1.10.3",
        "express": "~3.3.3",
        "glob": "^5.0.15",
        "jasmine": "^2.3.2",
        "jasmine-core": "^2.3.4",
        "js-yaml": "^3.3.1",
        "jspngopt": "^0.1.0",
        "less": "~2.7.1",
        "nomnom": "^1.8.1",
        "pako": "0.2.7",
        "selenium-webdriver": "^2.46.1",
        "sri-toolbox": "^0.2.0",
        "uglify-js": "~2.4.15"
    },
    "directories": {},
    "dist": {
        "shasum": "06bb5298efad05e1e7228035ba8e1591f3061b8f",
        "tarball": "https://registry.npmjs.org/katex/-/katex-0.7.1.tgz"
    },
    "files": [
        "katex.js",
        "cli.js",
        "src/",
        "dist/"
    ],
    "gitHead": "216832464034c13ec812a10f2143464b21a978c1",
    "homepage": "https://github.com/Khan/KaTeX#readme",
    "license": "MIT",
    "main": "katex.js",
    "maintainers": [
        {
            "name": "gagern"
        },
        {
            "name": "kevinbarabash"
        },
        {
            "name": "khanacademy"
        },
        {
            "name": "spicyj"
        },
        {
            "name": "xymostech"
        }
    ],
    "name": "katex",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/Khan/KaTeX.git"
    },
    "scripts": {
        "prepublish": "make NIS= dist",
        "start": "node server.js",
        "test": "make lint test"
    },
    "version": "0.7.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
