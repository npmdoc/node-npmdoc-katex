# api documentation for  [katex (v0.7.1)](https://github.com/Khan/KaTeX#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-katex.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-katex) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-katex.svg)](https://travis-ci.org/npmdoc/node-npmdoc-katex)
#### Fast math typesetting for the web.

[![NPM](https://nodei.co/npm/katex.png?downloads=true)](https://www.npmjs.com/package/katex)

[![apidoc](https://npmdoc.github.io/node-npmdoc-katex/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-katex_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-katex/build/apidoc.html)

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
            "name": "gagern",
            "email": "Martin.vGagern@gmx.net"
        },
        {
            "name": "kevinbarabash",
            "email": "kevinb7@gmail.com"
        },
        {
            "name": "khanacademy",
            "email": "opensource+npm@khanacademy.org"
        },
        {
            "name": "spicyj",
            "email": "ben@benalpert.com"
        },
        {
            "name": "xymostech",
            "email": "xymostech@gmail.com"
        }
    ],
    "name": "katex",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module katex](#apidoc.module.katex)
1.  [function <span class="apidocSignatureSpan">katex.</span>Lexer (input)](#apidoc.element.katex.Lexer)
1.  [function <span class="apidocSignatureSpan">katex.</span>MacroExpander (input, macros)](#apidoc.element.katex.MacroExpander)
1.  [function <span class="apidocSignatureSpan">katex.</span>Options (data)](#apidoc.element.katex.Options)
1.  [function <span class="apidocSignatureSpan">katex.</span>ParseError (message, token)](#apidoc.element.katex.ParseError)
1.  [function <span class="apidocSignatureSpan">katex.</span>Parser (input, settings)](#apidoc.element.katex.Parser)
1.  [function <span class="apidocSignatureSpan">katex.</span>__parse (expression, options)](#apidoc.element.katex.__parse)
1.  [function <span class="apidocSignatureSpan">katex.</span>render (expression, baseNode, options)](#apidoc.element.katex.render)
1.  [function <span class="apidocSignatureSpan">katex.</span>renderToString (expression, options)](#apidoc.element.katex.renderToString)
1.  object <span class="apidocSignatureSpan">katex.</span>Lexer.prototype
1.  object <span class="apidocSignatureSpan">katex.</span>MacroExpander.prototype
1.  object <span class="apidocSignatureSpan">katex.</span>Options.prototype
1.  object <span class="apidocSignatureSpan">katex.</span>Parser.prototype
1.  object <span class="apidocSignatureSpan">katex.</span>buildCommon
1.  object <span class="apidocSignatureSpan">katex.</span>delimiter
1.  object <span class="apidocSignatureSpan">katex.</span>domTree
1.  object <span class="apidocSignatureSpan">katex.</span>fontMetrics
1.  object <span class="apidocSignatureSpan">katex.</span>mathMLTree
1.  object <span class="apidocSignatureSpan">katex.</span>parseData
1.  object <span class="apidocSignatureSpan">katex.</span>utils

#### [module katex.Lexer](#apidoc.module.katex.Lexer)
1.  [function <span class="apidocSignatureSpan">katex.</span>Lexer (input)](#apidoc.element.katex.Lexer.Lexer)

#### [module katex.Lexer.prototype](#apidoc.module.katex.Lexer.prototype)
1.  [function <span class="apidocSignatureSpan">katex.Lexer.prototype.</span>lex ()](#apidoc.element.katex.Lexer.prototype.lex)

#### [module katex.MacroExpander](#apidoc.module.katex.MacroExpander)
1.  [function <span class="apidocSignatureSpan">katex.</span>MacroExpander (input, macros)](#apidoc.element.katex.MacroExpander.MacroExpander)

#### [module katex.MacroExpander.prototype](#apidoc.module.katex.MacroExpander.prototype)
1.  [function <span class="apidocSignatureSpan">katex.MacroExpander.prototype.</span>get (ignoreSpace)](#apidoc.element.katex.MacroExpander.prototype.get)
1.  [function <span class="apidocSignatureSpan">katex.MacroExpander.prototype.</span>nextToken ()](#apidoc.element.katex.MacroExpander.prototype.nextToken)
1.  [function <span class="apidocSignatureSpan">katex.MacroExpander.prototype.</span>unget (token)](#apidoc.element.katex.MacroExpander.prototype.unget)

#### [module katex.Options](#apidoc.module.katex.Options)
1.  [function <span class="apidocSignatureSpan">katex.</span>Options (data)](#apidoc.element.katex.Options.Options)

#### [module katex.Options.prototype](#apidoc.module.katex.Options.prototype)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>extend (extension)](#apidoc.element.katex.Options.prototype.extend)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>getColor ()](#apidoc.element.katex.Options.prototype.getColor)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>reset ()](#apidoc.element.katex.Options.prototype.reset)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withColor (color)](#apidoc.element.katex.Options.prototype.withColor)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withFont (font)](#apidoc.element.katex.Options.prototype.withFont)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withPhantom ()](#apidoc.element.katex.Options.prototype.withPhantom)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withSize (size)](#apidoc.element.katex.Options.prototype.withSize)
1.  [function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withStyle (style)](#apidoc.element.katex.Options.prototype.withStyle)

#### [module katex.Parser](#apidoc.module.katex.Parser)
1.  [function <span class="apidocSignatureSpan">katex.</span>Parser (input, settings)](#apidoc.element.katex.Parser.Parser)

#### [module katex.Parser.prototype](#apidoc.module.katex.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>ParseNode (type, value, mode, firstToken, lastToken)](#apidoc.element.katex.Parser.prototype.ParseNode)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>callFunction (name, args, positions, token)](#apidoc.element.katex.Parser.prototype.callFunction)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>consume ()](#apidoc.element.katex.Parser.prototype.consume)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>expect (text, consume)](#apidoc.element.katex.Parser.prototype.expect)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>formLigatures (group)](#apidoc.element.katex.Parser.prototype.formLigatures)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>handleInfixNodes (body)](#apidoc.element.katex.Parser.prototype.handleInfixNodes)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>handleSupSubscript (name)](#apidoc.element.katex.Parser.prototype.handleSupSubscript)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>handleUnsupportedCmd ()](#apidoc.element.katex.Parser.prototype.handleUnsupportedCmd)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parse ()](#apidoc.element.katex.Parser.prototype.parse)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseArguments (func, funcData)](#apidoc.element.katex.Parser.prototype.parseArguments)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseAtom ()](#apidoc.element.katex.Parser.prototype.parseAtom)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseColorGroup (optional)](#apidoc.element.katex.Parser.prototype.parseColorGroup)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseExpression (breakOnInfix, breakOnTokenText)](#apidoc.element.katex.Parser.prototype.parseExpression)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseFunction (baseGroup)](#apidoc.element.katex.Parser.prototype.parseFunction)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseGroup (optional)](#apidoc.element.katex.Parser.prototype.parseGroup)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseGroupOfType (innerMode, optional)](#apidoc.element.katex.Parser.prototype.parseGroupOfType)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseImplicitGroup ()](#apidoc.element.katex.Parser.prototype.parseImplicitGroup)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseInput ()](#apidoc.element.katex.Parser.prototype.parseInput)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseRegexGroup (regex, modeName)](#apidoc.element.katex.Parser.prototype.parseRegexGroup)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseSizeGroup (optional)](#apidoc.element.katex.Parser.prototype.parseSizeGroup)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseStringGroup (modeName, optional)](#apidoc.element.katex.Parser.prototype.parseStringGroup)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseSymbol ()](#apidoc.element.katex.Parser.prototype.parseSymbol)
1.  [function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>switchMode (newMode)](#apidoc.element.katex.Parser.prototype.switchMode)

#### [module katex.buildCommon](#apidoc.module.katex.buildCommon)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeFragment (children)](#apidoc.element.katex.buildCommon.makeFragment)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeOrd (group, options, type)](#apidoc.element.katex.buildCommon.makeOrd)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeSpan (classes, children, options)](#apidoc.element.katex.buildCommon.makeSpan)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeSymbol (value, fontFamily, mode, options, classes)](#apidoc.element.katex.buildCommon.makeSymbol)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeVList (children, positionType, positionData, options)](#apidoc.element.katex.buildCommon.makeVList)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>mathsym (value, mode, options, classes)](#apidoc.element.katex.buildCommon.mathsym)
1.  [function <span class="apidocSignatureSpan">katex.buildCommon.</span>prependChildren (span, children)](#apidoc.element.katex.buildCommon.prependChildren)
1.  object <span class="apidocSignatureSpan">katex.buildCommon.</span>fontMap
1.  object <span class="apidocSignatureSpan">katex.buildCommon.</span>sizingMultiplier
1.  object <span class="apidocSignatureSpan">katex.buildCommon.</span>spacingFunctions

#### [module katex.delimiter](#apidoc.module.katex.delimiter)
1.  [function <span class="apidocSignatureSpan">katex.delimiter.</span>customSizedDelim (delim, height, center, options, mode, classes)](#apidoc.element.katex.delimiter.customSizedDelim)
1.  [function <span class="apidocSignatureSpan">katex.delimiter.</span>leftRightDelim (delim, height, depth, options, mode, classes)](#apidoc.element.katex.delimiter.leftRightDelim)
1.  [function <span class="apidocSignatureSpan">katex.delimiter.</span>sizedDelim (delim, size, options, mode, classes)](#apidoc.element.katex.delimiter.sizedDelim)

#### [module katex.domTree](#apidoc.module.katex.domTree)
1.  [function <span class="apidocSignatureSpan">katex.domTree.</span>documentFragment (children)](#apidoc.element.katex.domTree.documentFragment)
1.  [function <span class="apidocSignatureSpan">katex.domTree.</span>span (classes, children, options)](#apidoc.element.katex.domTree.span)
1.  [function <span class="apidocSignatureSpan">katex.domTree.</span>symbolNode (value, height, depth, italic, skew, classes, style)](#apidoc.element.katex.domTree.symbolNode)

#### [module katex.fontMetrics](#apidoc.module.katex.fontMetrics)
1.  [function <span class="apidocSignatureSpan">katex.fontMetrics.</span>getCharacterMetrics (character, style)](#apidoc.element.katex.fontMetrics.getCharacterMetrics)
1.  object <span class="apidocSignatureSpan">katex.fontMetrics.</span>metrics
1.  object <span class="apidocSignatureSpan">katex.fontMetrics.</span>sigmas

#### [module katex.mathMLTree](#apidoc.module.katex.mathMLTree)
1.  [function <span class="apidocSignatureSpan">katex.mathMLTree.</span>MathNode (type, children)](#apidoc.element.katex.mathMLTree.MathNode)
1.  [function <span class="apidocSignatureSpan">katex.mathMLTree.</span>TextNode (text)](#apidoc.element.katex.mathMLTree.TextNode)

#### [module katex.parseData](#apidoc.module.katex.parseData)
1.  [function <span class="apidocSignatureSpan">katex.parseData.</span>ParseNode (type, value, mode, firstToken, lastToken)](#apidoc.element.katex.parseData.ParseNode)

#### [module katex.utils](#apidoc.module.katex.utils)
1.  [function <span class="apidocSignatureSpan">katex.utils.</span>clearNode (node)](#apidoc.element.katex.utils.clearNode)
1.  [function <span class="apidocSignatureSpan">katex.utils.</span>contains (list, elem)](#apidoc.element.katex.utils.contains)
1.  [function <span class="apidocSignatureSpan">katex.utils.</span>deflt (setting, defaultIfUndefined)](#apidoc.element.katex.utils.deflt)
1.  [function <span class="apidocSignatureSpan">katex.utils.</span>escape (text)](#apidoc.element.katex.utils.escape)
1.  [function <span class="apidocSignatureSpan">katex.utils.</span>hyphenate (str)](#apidoc.element.katex.utils.hyphenate)
1.  [function <span class="apidocSignatureSpan">katex.utils.</span>indexOf (list, elem)](#apidoc.element.katex.utils.indexOf)



# <a name="apidoc.module.katex"></a>[module katex](#apidoc.module.katex)

#### <a name="apidoc.element.katex.Lexer"></a>[function <span class="apidocSignatureSpan">katex.</span>Lexer (input)](#apidoc.element.katex.Lexer)
- description and source-code
```javascript
function Lexer(input) {
    this.input = input;
    this.pos = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.MacroExpander"></a>[function <span class="apidocSignatureSpan">katex.</span>MacroExpander (input, macros)](#apidoc.element.katex.MacroExpander)
- description and source-code
```javascript
function MacroExpander(input, macros) {
    this.lexer = new Lexer(input);
    this.macros = macros;
    this.stack = []; // contains tokens in REVERSE order
    this.discardedWhiteSpace = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.Options"></a>[function <span class="apidocSignatureSpan">katex.</span>Options (data)](#apidoc.element.katex.Options)
- description and source-code
```javascript
function Options(data) {
    this.style = data.style;
    this.color = data.color;
    this.size = data.size;
    this.phantom = data.phantom;
    this.font = data.font;

    if (data.parentStyle === undefined) {
        this.parentStyle = data.style;
    } else {
        this.parentStyle = data.parentStyle;
    }

    if (data.parentSize === undefined) {
        this.parentSize = data.size;
    } else {
        this.parentSize = data.parentSize;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.ParseError"></a>[function <span class="apidocSignatureSpan">katex.</span>ParseError (message, token)](#apidoc.element.katex.ParseError)
- description and source-code
```javascript
function ParseError(message, token) {
    var error = "KaTeX parse error: " + message;
    var start;
    var end;

    if (token && token.lexer && token.start <= token.end) {
        // If we have the input and a position, make the error a bit fancier

        // Get the input
        var input = token.lexer.input;

        // Prepend some information
        start = token.start;
        end = token.end;
        if (start === input.length) {
            error += " at end of input: ";
        } else {
            error += " at position " + (start + 1) + ": ";
        }

        // Underline token in question using combining underscores
        var underlined = input.slice(start, end).replace(/[^]/g, "$&\u0332");

        // Extract some context from the input and add it to the error
        var left;
        if (start > 15) {
            left = "…" + input.slice(start - 15, start);
        } else {
            left = input.slice(0, start);
        }
        var right;
        if (end + 15 < input.length) {
            right = input.slice(end, end + 15) + "…";
        } else {
            right = input.slice(end);
        }
        error += left + underlined + right;
    }

    // Some hackery to make ParseError a prototype of Error
    // See http://stackoverflow.com/a/8460753
    var self = new Error(error);
    self.name = "ParseError";
    self.__proto__ = ParseError.prototype;

    self.position = start;
    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.Parser"></a>[function <span class="apidocSignatureSpan">katex.</span>Parser (input, settings)](#apidoc.element.katex.Parser)
- description and source-code
```javascript
function Parser(input, settings) {
    // Create a new macro expander (gullet) and (indirectly via that) also a
    // new lexer (mouth) for this parser (stomach, in the language of TeX)
    this.gullet = new MacroExpander(input, settings.macros);
    // Store the settings for use in parsing
    this.settings = settings;
    // Count leftright depth (for \middle errors)
    this.leftrightDepth = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.__parse"></a>[function <span class="apidocSignatureSpan">katex.</span>__parse (expression, options)](#apidoc.element.katex.__parse)
- description and source-code
```javascript
__parse = function (expression, options) {
    var settings = new Settings(options);
    return parseTree(expression, settings);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.render"></a>[function <span class="apidocSignatureSpan">katex.</span>render (expression, baseNode, options)](#apidoc.element.katex.render)
- description and source-code
```javascript
render = function (expression, baseNode, options) {
    utils.clearNode(baseNode);

    var settings = new Settings(options);

    var tree = parseTree(expression, settings);
    var node = buildTree(tree, expression, settings).toNode();

    baseNode.appendChild(node);
}
```
- example usage
```shell
...
'''

#### In-browser rendering

Call 'katex.render' with a TeX expression and a DOM element to render into:

'''js
katex.render("c = \\pm\\sqrt{a^2 + b^2}", element);
'''

If KaTeX can't parse the expression, it throws a 'katex.ParseError' error.

#### Server side rendering or rendering to a string

To generate HTML on the server or to generate an HTML string of the rendered math, you can use 'katex.renderToString':
...
```

#### <a name="apidoc.element.katex.renderToString"></a>[function <span class="apidocSignatureSpan">katex.</span>renderToString (expression, options)](#apidoc.element.katex.renderToString)
- description and source-code
```javascript
renderToString = function (expression, options) {
    var settings = new Settings(options);

    var tree = parseTree(expression, settings);
    return buildTree(tree, expression, settings).toMarkup();
}
```
- example usage
```shell
...
If KaTeX can't parse the expression, it throws a 'katex.ParseError' error.

#### Server side rendering or rendering to a string

To generate HTML on the server or to generate an HTML string of the rendered math, you can use 'katex.renderToString':

'''js
var html = katex.renderToString("c = \\pm\\sqrt{a^2 + b^2}");
// '<span class="katex">...</span>'
'''

Make sure to include the CSS and font files, but there is no need to include the JavaScript. Like 'render', 'renderToString' throws
 if it can't parse the expression.

#### Rendering options
...
```



# <a name="apidoc.module.katex.Lexer"></a>[module katex.Lexer](#apidoc.module.katex.Lexer)

#### <a name="apidoc.element.katex.Lexer.Lexer"></a>[function <span class="apidocSignatureSpan">katex.</span>Lexer (input)](#apidoc.element.katex.Lexer.Lexer)
- description and source-code
```javascript
function Lexer(input) {
    this.input = input;
    this.pos = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.katex.Lexer.prototype"></a>[module katex.Lexer.prototype](#apidoc.module.katex.Lexer.prototype)

#### <a name="apidoc.element.katex.Lexer.prototype.lex"></a>[function <span class="apidocSignatureSpan">katex.Lexer.prototype.</span>lex ()](#apidoc.element.katex.Lexer.prototype.lex)
- description and source-code
```javascript
lex = function () {
    var input = this.input;
    var pos = this.pos;
    if (pos === input.length) {
        return new Token("EOF", pos, pos, this);
    }
    var match = matchAt(tokenRegex, input, pos);
    if (match === null) {
        throw new ParseError(
            "Unexpected character: '" + input[pos] + "'",
            new Token(input[pos], pos, pos + 1, this));
    }
    var text = match[2] || " ";
    var start = this.pos;
    this.pos += match[0].length;
    var end = this.pos;
    return new Token(text, start, end, this);
}
```
- example usage
```shell
...

/**
 * Recursively expand first token, then return first non-expandable token.
 */
MacroExpander.prototype.nextToken = function() {
for (;;) {
    if (this.stack.length === 0) {
        this.stack.push(this.lexer.lex());
    }
    var topToken = this.stack.pop();
    var name = topToken.text;
    if (!(name.charAt(0) === "\\" && this.macros.hasOwnProperty(name))) {
        return topToken;
    }
    var expansion = this.macros[name];
...
```



# <a name="apidoc.module.katex.MacroExpander"></a>[module katex.MacroExpander](#apidoc.module.katex.MacroExpander)

#### <a name="apidoc.element.katex.MacroExpander.MacroExpander"></a>[function <span class="apidocSignatureSpan">katex.</span>MacroExpander (input, macros)](#apidoc.element.katex.MacroExpander.MacroExpander)
- description and source-code
```javascript
function MacroExpander(input, macros) {
    this.lexer = new Lexer(input);
    this.macros = macros;
    this.stack = []; // contains tokens in REVERSE order
    this.discardedWhiteSpace = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.katex.MacroExpander.prototype"></a>[module katex.MacroExpander.prototype](#apidoc.module.katex.MacroExpander.prototype)

#### <a name="apidoc.element.katex.MacroExpander.prototype.get"></a>[function <span class="apidocSignatureSpan">katex.MacroExpander.prototype.</span>get (ignoreSpace)](#apidoc.element.katex.MacroExpander.prototype.get)
- description and source-code
```javascript
get = function (ignoreSpace) {
    this.discardedWhiteSpace = [];
    var token = this.nextToken();
    if (ignoreSpace) {
        while (token.text === " ") {
            this.discardedWhiteSpace.push(token);
            token = this.nextToken();
        }
    }
    return token;
}
```
- example usage
```shell
...
};

/**
 * Considers the current look ahead token as consumed,
 * and fetches the one after that as the new look ahead.
 */
Parser.prototype.consume = function() {
    this.nextToken = this.gullet.get(this.mode === "math");
};

Parser.prototype.switchMode = function(newMode) {
    this.gullet.unget(this.nextToken);
    this.mode = newMode;
    this.consume();
};
...
```

#### <a name="apidoc.element.katex.MacroExpander.prototype.nextToken"></a>[function <span class="apidocSignatureSpan">katex.MacroExpander.prototype.</span>nextToken ()](#apidoc.element.katex.MacroExpander.prototype.nextToken)
- description and source-code
```javascript
nextToken = function () {
    for (;;) {
        if (this.stack.length === 0) {
            this.stack.push(this.lexer.lex());
        }
        var topToken = this.stack.pop();
        var name = topToken.text;
        if (!(name.charAt(0) === "\\" && this.macros.hasOwnProperty(name))) {
            return topToken;
        }
        var expansion = this.macros[name];
        if (typeof expansion === "string") {
            var bodyLexer = new Lexer(expansion);
            expansion = [];
            var tok = bodyLexer.lex();
            while (tok.text !== "EOF") {
                expansion.push(tok);
                tok = bodyLexer.lex();
            }
            expansion.reverse(); // to fit in with stack using push and pop
            this.macros[name] = expansion;
        }
        this.stack = this.stack.concat(expansion);
    }
}
```
- example usage
```shell
...
    }
    this.stack = this.stack.concat(expansion);
}
};

MacroExpander.prototype.get = function(ignoreSpace) {
this.discardedWhiteSpace = [];
var token = this.nextToken();
if (ignoreSpace) {
    while (token.text === " ") {
        this.discardedWhiteSpace.push(token);
        token = this.nextToken();
    }
}
return token;
...
```

#### <a name="apidoc.element.katex.MacroExpander.prototype.unget"></a>[function <span class="apidocSignatureSpan">katex.MacroExpander.prototype.</span>unget (token)](#apidoc.element.katex.MacroExpander.prototype.unget)
- description and source-code
```javascript
unget = function (token) {
    this.stack.push(token);
    while (this.discardedWhiteSpace.length !== 0) {
        this.stack.push(this.discardedWhiteSpace.pop());
    }
}
```
- example usage
```shell
...
* and fetches the one after that as the new look ahead.
*/
Parser.prototype.consume = function() {
   this.nextToken = this.gullet.get(this.mode === "math");
};

Parser.prototype.switchMode = function(newMode) {
   this.gullet.unget(this.nextToken);
   this.mode = newMode;
   this.consume();
};

/**
* Main parsing function, which parses an entire input.
*
...
```



# <a name="apidoc.module.katex.Options"></a>[module katex.Options](#apidoc.module.katex.Options)

#### <a name="apidoc.element.katex.Options.Options"></a>[function <span class="apidocSignatureSpan">katex.</span>Options (data)](#apidoc.element.katex.Options.Options)
- description and source-code
```javascript
function Options(data) {
    this.style = data.style;
    this.color = data.color;
    this.size = data.size;
    this.phantom = data.phantom;
    this.font = data.font;

    if (data.parentStyle === undefined) {
        this.parentStyle = data.style;
    } else {
        this.parentStyle = data.parentStyle;
    }

    if (data.parentSize === undefined) {
        this.parentSize = data.size;
    } else {
        this.parentSize = data.parentSize;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.katex.Options.prototype"></a>[module katex.Options.prototype](#apidoc.module.katex.Options.prototype)

#### <a name="apidoc.element.katex.Options.prototype.extend"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>extend (extension)](#apidoc.element.katex.Options.prototype.extend)
- description and source-code
```javascript
extend = function (extension) {
    var data = {
        style: this.style,
        size: this.size,
        color: this.color,
        parentStyle: this.style,
        parentSize: this.size,
        phantom: this.phantom,
        font: this.font
    };

    for (var key in extension) {
        if (extension.hasOwnProperty(key)) {
            data[key] = extension[key];
        }
    }

    return new Options(data);
}
```
- example usage
```shell
...
   return new Options(data);
};

/**
* Create a new options object with the given style.
*/
Options.prototype.withStyle = function(style) {
   return this.extend({
       style: style
   });
};

/**
* Create a new options object with the given size.
*/
...
```

#### <a name="apidoc.element.katex.Options.prototype.getColor"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>getColor ()](#apidoc.element.katex.Options.prototype.getColor)
- description and source-code
```javascript
getColor = function () {
    if (this.phantom) {
        return "transparent";
    } else {
        return colorMap[this.color] || this.color;
    }
}
```
- example usage
```shell
...
        symbolNode = new domTree.symbolNode(value, 0, 0, 0, 0, classes);
    }

    if (options) {
        if (options.style.isTight()) {
            symbolNode.classes.push("mtight");
        }
        if (options.getColor()) {
            symbolNode.style.color = options.getColor();
        }
    }

    return symbolNode;
};
...
```

#### <a name="apidoc.element.katex.Options.prototype.reset"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>reset ()](#apidoc.element.katex.Options.prototype.reset)
- description and source-code
```javascript
reset = function () {
    return this.extend({});
}
```
- example usage
```shell
...
       baseElem.type === "close" ||
       baseElem.type === "punct";
};

var makeNullDelimiter = function(options, classes) {
   return makeSpan(classes.concat([
       "sizing", "reset-" + options.size, "size5",
       options.style.reset(), Style.TEXT.cls(),
       "nulldelimiter"]));
};

/**
* This is a map of group types to the function used to handle that type.
* Simpler types come at the beginning, while complicated types come afterwards.
*/
...
```

#### <a name="apidoc.element.katex.Options.prototype.withColor"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withColor (color)](#apidoc.element.katex.Options.prototype.withColor)
- description and source-code
```javascript
withColor = function (color) {
    return this.extend({
        color: color
    });
}
```
- example usage
```shell
...
return makeSpan(["mord", "text", newOptions.style.cls()],
    inner, newOptions);
};

groupTypes.color = function(group, options) {
var elements = buildExpression(
    group.value.value,
    options.withColor(group.value.color),
    false
);

// \color isn't supposed to affect the type of the elements it contains.
// To accomplish this, we wrap the results in a fragment, so the inner
// elements will be able to directly interact with their neighbors. For
// example, '\color{red}{2 +} 3' has the same spacing as '2 + 3'
...
```

#### <a name="apidoc.element.katex.Options.prototype.withFont"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withFont (font)](#apidoc.element.katex.Options.prototype.withFont)
- description and source-code
```javascript
withFont = function (font) {
    return this.extend({
        font: font || this.font
    });
}
```
- example usage
```shell
...
    ["mord", options.style.cls()],
    buildExpression(group.value, options.reset(), true),
    options
);
};

groupTypes.text = function(group, options) {
var newOptions = options.withFont(group.value.style);
var inner = buildExpression(group.value.body, newOptions, true);
for (var i = 0; i < inner.length - 1; i++) {
    if (inner[i].tryCombine(inner[i + 1])) {
        inner.splice(i + 1, 1);
        i--;
    }
}
...
```

#### <a name="apidoc.element.katex.Options.prototype.withPhantom"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withPhantom ()](#apidoc.element.katex.Options.prototype.withPhantom)
- description and source-code
```javascript
withPhantom = function () {
    return this.extend({
        phantom: true
    });
}
```
- example usage
```shell
...
        return accentWrap;
    }
};

groupTypes.phantom = function(group, options) {
    var elements = buildExpression(
        group.value.value,
        options.withPhantom(),
        false
    );

    // \phantom isn't supposed to affect the elements it contains.
    // See "color" for more details.
    return new buildCommon.makeFragment(elements);
};
...
```

#### <a name="apidoc.element.katex.Options.prototype.withSize"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withSize (size)](#apidoc.element.katex.Options.prototype.withSize)
- description and source-code
```javascript
withSize = function (size) {
    return this.extend({
        size: size
    });
}
```
- example usage
```shell
...
};

groupTypes.sizing = function(group, options) {
// Handle sizing operators like \Huge. Real TeX doesn't actually allow
// these functions inside of math expressions, so we do some special
// handling.
var inner = buildExpression(group.value.value,
        options.withSize(group.value.size), false);

// Compute the correct maxFontSize.
var style = options.style;
var fontSize = buildCommon.sizingMultiplier[group.value.size];
fontSize = fontSize * style.sizeMultiplier;

// Add size-resetting classes to the inner list and set maxFontSize
...
```

#### <a name="apidoc.element.katex.Options.prototype.withStyle"></a>[function <span class="apidocSignatureSpan">katex.Options.prototype.</span>withStyle (style)](#apidoc.element.katex.Options.prototype.withStyle)
- description and source-code
```javascript
withStyle = function (style) {
    return this.extend({
        style: style
    });
}
```
- example usage
```shell
...
var sup;
var sub;

var style = options.style;
var newOptions;

if (group.value.sup) {
    newOptions = options.withStyle(style.sup());
    sup = buildGroup(group.value.sup, newOptions);
    supmid = makeSpan([style.reset(), style.sup().cls()],
        [sup], newOptions);
}

if (group.value.sub) {
    newOptions = options.withStyle(style.sub());
...
```



# <a name="apidoc.module.katex.Parser"></a>[module katex.Parser](#apidoc.module.katex.Parser)

#### <a name="apidoc.element.katex.Parser.Parser"></a>[function <span class="apidocSignatureSpan">katex.</span>Parser (input, settings)](#apidoc.element.katex.Parser.Parser)
- description and source-code
```javascript
function Parser(input, settings) {
    // Create a new macro expander (gullet) and (indirectly via that) also a
    // new lexer (mouth) for this parser (stomach, in the language of TeX)
    this.gullet = new MacroExpander(input, settings.macros);
    // Store the settings for use in parsing
    this.settings = settings;
    // Count leftright depth (for \middle errors)
    this.leftrightDepth = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.katex.Parser.prototype"></a>[module katex.Parser.prototype](#apidoc.module.katex.Parser.prototype)

#### <a name="apidoc.element.katex.Parser.prototype.ParseNode"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>ParseNode (type, value, mode, firstToken, lastToken)](#apidoc.element.katex.Parser.prototype.ParseNode)
- description and source-code
```javascript
function ParseNode(type, value, mode, firstToken, lastToken) {
    this.type = type;
    this.value = value;
    this.mode = mode;
    if (firstToken && (!lastToken || lastToken.lexer === firstToken.lexer)) {
        this.lexer = firstToken.lexer;
        this.start = firstToken.start;
        this.end = (lastToken || firstToken).end;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.Parser.prototype.callFunction"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>callFunction (name, args, positions, token)](#apidoc.element.katex.Parser.prototype.callFunction)
- description and source-code
```javascript
callFunction = function (name, args, positions, token) {
    var context = {
        funcName: name,
        parser: this,
        positions: positions,
        token: token
    };
    return functions[name].handler(context, args);
}
```
- example usage
```shell
...

        if (denomBody.length === 1 && denomBody[0].type === "ordgroup") {
            denomNode = denomBody[0];
        } else {
            denomNode = new ParseNode("ordgroup", denomBody, this.mode);
        }

        var value = this.callFunction(
            funcName, [numerNode, denomNode], null);
        return [new ParseNode(value.type, value, this.mode)];
    } else {
        return body;
    }
};
...
```

#### <a name="apidoc.element.katex.Parser.prototype.consume"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>consume ()](#apidoc.element.katex.Parser.prototype.consume)
- description and source-code
```javascript
consume = function () {
    this.nextToken = this.gullet.get(this.mode === "math");
}
```
- example usage
```shell
...
   if (this.nextToken.text !== text) {
       throw new ParseError(
           "Expected '" + text + "', got '" + this.nextToken.text + "'",
           this.nextToken
       );
   }
   if (consume !== false) {
       this.consume();
   }
};

/**
* Considers the current look ahead token as consumed,
* and fetches the one after that as the new look ahead.
*/
...
```

#### <a name="apidoc.element.katex.Parser.prototype.expect"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>expect (text, consume)](#apidoc.element.katex.Parser.prototype.expect)
- description and source-code
```javascript
expect = function (text, consume) {
    if (this.nextToken.text !== text) {
        throw new ParseError(
            "Expected '" + text + "', got '" + this.nextToken.text + "'",
            this.nextToken
        );
    }
    if (consume !== false) {
        this.consume();
    }
}
```
- example usage
```shell
...
/**
* Parses an entire input tree.
*/
Parser.prototype.parseInput = function() {
   // Parse an expression
   var expression = this.parseExpression(false);
   // If we succeeded, make sure there's an EOF at the end
   this.expect("EOF", false);
   return expression;
};

var endOfExpression = ["}", "\\end", "\\right", "&", "\\\\", "\\cr"];

/**
* Parses an "expression", which is a list of atoms.
...
```

#### <a name="apidoc.element.katex.Parser.prototype.formLigatures"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>formLigatures (group)](#apidoc.element.katex.Parser.prototype.formLigatures)
- description and source-code
```javascript
formLigatures = function (group) {
    var i;
    var n = group.length - 1;
    for (i = 0; i < n; ++i) {
        var a = group[i];
        var v = a.value;
        if (v === "-" && group[i + 1].value === "-") {
            if (i + 1 < n && group[i + 2].value === "-") {
                group.splice(i, 3, new ParseNode(
                    "textord", "---", "text", a, group[i + 2]));
                n -= 2;
            } else {
                group.splice(i, 2, new ParseNode(
                    "textord", "--", "text", a, group[i + 1]));
                n -= 1;
            }
        }
        if ((v === "'" || v === "'") && group[i + 1].value === v) {
            group.splice(i, 2, new ParseNode(
                "textord", v + v, "text", a, group[i + 1]));
            n -= 1;
        }
    }
}
```
- example usage
```shell
...
    // If we get a brace, parse an expression
    this.consume();
    var expression = this.parseExpression(false, optional ? "]" : null);
    var lastToken = this.nextToken;
    // Make sure we get a close brace
    this.expect(optional ? "]" : "}");
    if (this.mode === "text") {
        this.formLigatures(expression);
    }
    return new ParseFuncOrArgument(
        new ParseNode("ordgroup", expression, this.mode,
                      firstToken, lastToken),
        false);
} else {
    // Otherwise, just return a nucleus, or nothing for an optional group
...
```

#### <a name="apidoc.element.katex.Parser.prototype.handleInfixNodes"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>handleInfixNodes (body)](#apidoc.element.katex.Parser.prototype.handleInfixNodes)
- description and source-code
```javascript
handleInfixNodes = function (body) {
    var overIndex = -1;
    var funcName;

    for (var i = 0; i < body.length; i++) {
        var node = body[i];
        if (node.type === "infix") {
            if (overIndex !== -1) {
                throw new ParseError(
                    "only one infix operator per group",
                    node.value.token);
            }
            overIndex = i;
            funcName = node.value.replaceWith;
        }
    }

    if (overIndex !== -1) {
        var numerNode;
        var denomNode;

        var numerBody = body.slice(0, overIndex);
        var denomBody = body.slice(overIndex + 1);

        if (numerBody.length === 1 && numerBody[0].type === "ordgroup") {
            numerNode = numerBody[0];
        } else {
            numerNode = new ParseNode("ordgroup", numerBody, this.mode);
        }

        if (denomBody.length === 1 && denomBody[0].type === "ordgroup") {
            denomNode = denomBody[0];
        } else {
            denomNode = new ParseNode("ordgroup", denomBody, this.mode);
        }

        var value = this.callFunction(
            funcName, [numerNode, denomNode], null);
        return [new ParseNode(value.type, value, this.mode)];
    } else {
        return body;
    }
}
```
- example usage
```shell
...
               continue;
           }

           break;
       }
       body.push(atom);
   }
   return this.handleInfixNodes(body);
};

/**
* Rewrites infix operators such as \over with corresponding commands such
* as \frac.
*
* There can only be one infix operator per group.  If there's more than one
...
```

#### <a name="apidoc.element.katex.Parser.prototype.handleSupSubscript"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>handleSupSubscript (name)](#apidoc.element.katex.Parser.prototype.handleSupSubscript)
- description and source-code
```javascript
handleSupSubscript = function (name) {
    var symbolToken = this.nextToken;
    var symbol = symbolToken.text;
    this.consume();
    var group = this.parseGroup();

    if (!group) {
        if (!this.settings.throwOnError && this.nextToken.text[0] === "\\") {
            return this.handleUnsupportedCmd();
        } else {
            throw new ParseError(
                "Expected group after '" + symbol + "'",
                symbolToken
            );
        }
    } else if (group.isFunction) {
        // ^ and _ have a greediness, so handle interactions with functions'
        // greediness
        var funcGreediness = functions[group.result].greediness;
        if (funcGreediness > SUPSUB_GREEDINESS) {
            return this.parseFunction(group);
        } else {
            throw new ParseError(
                "Got function '" + group.result + "' with no arguments " +
                    "as " + name, symbolToken);
        }
    } else {
        return group.result;
    }
}
```
- example usage
```shell
...
    }
    this.consume();
} else if (lex.text === "^") {
    // We got a superscript start
    if (superscript) {
        throw new ParseError("Double superscript", lex);
    }
    superscript = this.handleSupSubscript("superscript");
} else if (lex.text === "_") {
    // We got a subscript start
    if (subscript) {
        throw new ParseError("Double subscript", lex);
    }
    subscript = this.handleSupSubscript("subscript");
} else if (lex.text === "'") {
...
```

#### <a name="apidoc.element.katex.Parser.prototype.handleUnsupportedCmd"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>handleUnsupportedCmd ()](#apidoc.element.katex.Parser.prototype.handleUnsupportedCmd)
- description and source-code
```javascript
handleUnsupportedCmd = function () {
    var text = this.nextToken.text;
    var textordArray = [];

    for (var i = 0; i < text.length; i++) {
        textordArray.push(new ParseNode("textord", text[i], "text"));
    }

    var textNode = new ParseNode(
        "text",
        {
            body: textordArray,
            type: "text"
        },
        this.mode);

    var colorNode = new ParseNode(
        "color",
        {
            color: this.settings.errorColor,
            value: [textNode],
            type: "color"
        },
        this.mode);

    this.consume();
    return colorNode;
}
```
- example usage
```shell
...
}
if (breakOnInfix && functions[lex.text] && functions[lex.text].infix) {
    break;
}
var atom = this.parseAtom();
if (!atom) {
    if (!this.settings.throwOnError && lex.text[0] === "\\") {
        var errorNode = this.handleUnsupportedCmd();
        body.push(errorNode);
        continue;
    }

    break;
}
body.push(atom);
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parse ()](#apidoc.element.katex.Parser.prototype.parse)
- description and source-code
```javascript
parse = function () {
    // Try to parse the input
    this.mode = "math";
    this.consume();
    var parse = this.parseInput();
    return parse;
}
```
- example usage
```shell
...
/**
 * Take an entire parse tree, and build it into an appropriate set of HTML
 * nodes.
 */
var buildHTML = function(tree, options) {
// buildExpression is destructive, so we need to make a clone
// of the incoming tree so that it isn't accidentally changed
tree = JSON.parse(JSON.stringify(tree));

// Build the expression contained in the tree
var expression = buildExpression(tree, options, true);
var body = makeSpan(["base", options.style.cls()], expression, options);

// Add struts, which ensure that the top of the HTML element falls at the
// height of the expression, and the bottom of the HTML element falls at the
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseArguments"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseArguments (func, funcData)](#apidoc.element.katex.Parser.prototype.parseArguments)
- description and source-code
```javascript
parseArguments = function (func, funcData) {
    var totalArgs = funcData.numArgs + funcData.numOptionalArgs;
    if (totalArgs === 0) {
        return [[this.pos]];
    }

    var baseGreediness = funcData.greediness;
    var positions = [this.pos];
    var args = [];

    for (var i = 0; i < totalArgs; i++) {
        var nextToken = this.nextToken;
        var argType = funcData.argTypes && funcData.argTypes[i];
        var arg;
        if (i < funcData.numOptionalArgs) {
            if (argType) {
                arg = this.parseGroupOfType(argType, true);
            } else {
                arg = this.parseGroup(true);
            }
            if (!arg) {
                args.push(null);
                positions.push(this.pos);
                continue;
            }
        } else {
            if (argType) {
                arg = this.parseGroupOfType(argType);
            } else {
                arg = this.parseGroup();
            }
            if (!arg) {
                if (!this.settings.throwOnError &&
                    this.nextToken.text[0] === "\\") {
                    arg = new ParseFuncOrArgument(
                        this.handleUnsupportedCmd(this.nextToken.text),
                        false);
                } else {
                    throw new ParseError(
                        "Expected group after '" + func + "'", nextToken);
                }
            }
        }
        var argNode;
        if (arg.isFunction) {
            var argGreediness =
                functions[arg.result].greediness;
            if (argGreediness > baseGreediness) {
                argNode = this.parseFunction(arg);
            } else {
                throw new ParseError(
                    "Got function '" + arg.result + "' as " +
                    "argument to '" + func + "'", nextToken);
            }
        } else {
            argNode = arg.result;
        }
        args.push(argNode);
        positions.push(this.pos);
    }

    args.push(positions);

    return args;
}
```
- example usage
```shell
...
if (!environments.hasOwnProperty(envName)) {
    throw new ParseError(
        "No such environment: " + envName, begin.value.nameGroup);
}
// Build the environment object. Arguments and other information will
// be made available to the begin and end methods using properties.
var env = environments[envName];
var args = this.parseArguments("\\begin{" + envName + "}", env);
var context = {
    mode: this.mode,
    envName: envName,
    parser: this,
    positions: args.pop()
};
var result = env.handler(context, args);
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseAtom"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseAtom ()](#apidoc.element.katex.Parser.prototype.parseAtom)
- description and source-code
```javascript
parseAtom = function () {
    // The body of an atom is an implicit group, so that things like
    // \left(x\right)^2 work correctly.
    var base = this.parseImplicitGroup();

    // In text mode, we don't have superscripts or subscripts
    if (this.mode === "text") {
        return base;
    }

    // Note that base may be empty (i.e. null) at this point.

    var superscript;
    var subscript;
    while (true) {
        // Lex the first token
        var lex = this.nextToken;

        if (lex.text === "\\limits" || lex.text === "\\nolimits") {
            // We got a limit control
            if (!base || base.type !== "op") {
                throw new ParseError(
                    "Limit controls must follow a math operator",
                    lex);
            } else {
                var limits = lex.text === "\\limits";
                base.value.limits = limits;
                base.value.alwaysHandleSupSub = true;
            }
            this.consume();
        } else if (lex.text === "^") {
            // We got a superscript start
            if (superscript) {
                throw new ParseError("Double superscript", lex);
            }
            superscript = this.handleSupSubscript("superscript");
        } else if (lex.text === "_") {
            // We got a subscript start
            if (subscript) {
                throw new ParseError("Double subscript", lex);
            }
            subscript = this.handleSupSubscript("subscript");
        } else if (lex.text === "'") {
            // We got a prime
            var prime = new ParseNode("textord", "\\prime", this.mode);

            // Many primes can be grouped together, so we handle this here
            var primes = [prime];
            this.consume();
            // Keep lexing tokens until we get something that's not a prime
            while (this.nextToken.text === "'") {
                // For each one, add another prime to the list
                primes.push(prime);
                this.consume();
            }
            // Put them into an ordgroup as the superscript
            superscript = new ParseNode("ordgroup", primes, this.mode);
        } else {
            // If it wasn't ^, _, or ', stop parsing super/subscripts
            break;
        }
    }

    if (superscript || subscript) {
        // If we got either a superscript or subscript, create a supsub
        return new ParseNode("supsub", {
            base: base,
            sup: superscript,
            sub: subscript
        }, this.mode);
    } else {
        // Otherwise return the original body
        return base;
    }
}
```
- example usage
```shell
...
}
if (breakOnTokenText && lex.text === breakOnTokenText) {
    break;
}
if (breakOnInfix && functions[lex.text] && functions[lex.text].infix) {
    break;
}
var atom = this.parseAtom();
if (!atom) {
    if (!this.settings.throwOnError && lex.text[0] === "\\") {
        var errorNode = this.handleUnsupportedCmd();
        body.push(errorNode);
        continue;
    }
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseColorGroup"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseColorGroup (optional)](#apidoc.element.katex.Parser.prototype.parseColorGroup)
- description and source-code
```javascript
parseColorGroup = function (optional) {
    var res = this.parseStringGroup("color", optional);
    if (!res) {
        return null;
    }
    var match = (/^(#[a-z0-9]+|[a-z]+)$/i).exec(res.text);
    if (!match) {
        throw new ParseError("Invalid color: '" + res.text + "'", res);
    }
    return new ParseFuncOrArgument(
        new ParseNode("color", match[0], this.mode),
        false);
}
```
- example usage
```shell
...
var outerMode = this.mode;
// Handle 'original' argTypes
if (innerMode === "original") {
    innerMode = outerMode;
}

if (innerMode === "color") {
    return this.parseColorGroup(optional);
}
if (innerMode === "size") {
    return this.parseSizeGroup(optional);
}

this.switchMode(innerMode);
if (innerMode === "text") {
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseExpression"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseExpression (breakOnInfix, breakOnTokenText)](#apidoc.element.katex.Parser.prototype.parseExpression)
- description and source-code
```javascript
parseExpression = function (breakOnInfix, breakOnTokenText) {
    var body = [];
    // Keep adding atoms to the body until we can't parse any more atoms (either
    // we reached the end, a }, or a \right)
    while (true) {
        var lex = this.nextToken;
        if (endOfExpression.indexOf(lex.text) !== -1) {
            break;
        }
        if (breakOnTokenText && lex.text === breakOnTokenText) {
            break;
        }
        if (breakOnInfix && functions[lex.text] && functions[lex.text].infix) {
            break;
        }
        var atom = this.parseAtom();
        if (!atom) {
            if (!this.settings.throwOnError && lex.text[0] === "\\") {
                var errorNode = this.handleUnsupportedCmd();
                body.push(errorNode);
                continue;
            }

            break;
        }
        body.push(atom);
    }
    return this.handleInfixNodes(body);
}
```
- example usage
```shell
...
};

/**
 * Parses an entire input tree.
 */
Parser.prototype.parseInput = function() {
    // Parse an expression
    var expression = this.parseExpression(false);
    // If we succeeded, make sure there's an EOF at the end
    this.expect("EOF", false);
    return expression;
};

var endOfExpression = ["}", "\\end", "\\right", "&", "\\\\", "\\cr"];
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseFunction"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseFunction (baseGroup)](#apidoc.element.katex.Parser.prototype.parseFunction)
- description and source-code
```javascript
parseFunction = function (baseGroup) {
    if (!baseGroup) {
        baseGroup = this.parseGroup();
    }

    if (baseGroup) {
        if (baseGroup.isFunction) {
            var func = baseGroup.result;
            var funcData = functions[func];
            if (this.mode === "text" && !funcData.allowedInText) {
                throw new ParseError(
                    "Can't use function '" + func + "' in text mode",
                    baseGroup.token);
            }

            var args = this.parseArguments(func, funcData);
            var token = baseGroup.token;
            var result = this.callFunction(func, args, args.pop(), token);
            return new ParseNode(result.type, result, this.mode);
        } else {
            return baseGroup.result;
        }
    } else {
        return null;
    }
}
```
- example usage
```shell
...
        );
    }
} else if (group.isFunction) {
    // ^ and _ have a greediness, so handle interactions with functions'
    // greediness
    var funcGreediness = functions[group.result].greediness;
    if (funcGreediness > SUPSUB_GREEDINESS) {
        return this.parseFunction(group);
    } else {
        throw new ParseError(
            "Got function '" + group.result + "' with no arguments " +
                "as " + name, symbolToken);
    }
} else {
    return group.result;
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseGroup"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseGroup (optional)](#apidoc.element.katex.Parser.prototype.parseGroup)
- description and source-code
```javascript
parseGroup = function (optional) {
    var firstToken = this.nextToken;
    // Try to parse an open brace
    if (this.nextToken.text === (optional ? "[" : "{")) {
        // If we get a brace, parse an expression
        this.consume();
        var expression = this.parseExpression(false, optional ? "]" : null);
        var lastToken = this.nextToken;
        // Make sure we get a close brace
        this.expect(optional ? "]" : "}");
        if (this.mode === "text") {
            this.formLigatures(expression);
        }
        return new ParseFuncOrArgument(
            new ParseNode("ordgroup", expression, this.mode,
                          firstToken, lastToken),
            false);
    } else {
        // Otherwise, just return a nucleus, or nothing for an optional group
        return optional ? null : this.parseSymbol();
    }
}
```
- example usage
```shell
...
/**
 * Handle a subscript or superscript with nice errors.
 */
Parser.prototype.handleSupSubscript = function(name) {
var symbolToken = this.nextToken;
var symbol = symbolToken.text;
this.consume();
var group = this.parseGroup();

if (!group) {
    if (!this.settings.throwOnError && this.nextToken.text[0] === "\\") {
        return this.handleUnsupportedCmd();
    } else {
        throw new ParseError(
            "Expected group after '" + symbol + "'",
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseGroupOfType"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseGroupOfType (innerMode, optional)](#apidoc.element.katex.Parser.prototype.parseGroupOfType)
- description and source-code
```javascript
parseGroupOfType = function (innerMode, optional) {
    var outerMode = this.mode;
    // Handle 'original' argTypes
    if (innerMode === "original") {
        innerMode = outerMode;
    }

    if (innerMode === "color") {
        return this.parseColorGroup(optional);
    }
    if (innerMode === "size") {
        return this.parseSizeGroup(optional);
    }

    this.switchMode(innerMode);
    if (innerMode === "text") {
        // text mode is special because it should ignore the whitespace before
        // it
        while (this.nextToken.text === " ") {
            this.consume();
        }
    }
    // By the time we get here, innerMode is one of "text" or "math".
    // We switch the mode of the parser, recurse, then restore the old mode.
    var res = this.parseGroup(optional);
    this.switchMode(outerMode);
    return res;
}
```
- example usage
```shell
...

    for (var i = 0; i < totalArgs; i++) {
var nextToken = this.nextToken;
var argType = funcData.argTypes && funcData.argTypes[i];
var arg;
if (i < funcData.numOptionalArgs) {
    if (argType) {
        arg = this.parseGroupOfType(argType, true);
    } else {
        arg = this.parseGroup(true);
    }
    if (!arg) {
        args.push(null);
        positions.push(this.pos);
        continue;
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseImplicitGroup"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseImplicitGroup ()](#apidoc.element.katex.Parser.prototype.parseImplicitGroup)
- description and source-code
```javascript
parseImplicitGroup = function () {
    var start = this.parseSymbol();

    if (start == null) {
        // If we didn't get anything we handle, fall back to parseFunction
        return this.parseFunction();
    }

    var func = start.result;
    var body;

    if (func === "\\left") {
        // If we see a left:
        // Parse the entire left function (including the delimiter)
        var left = this.parseFunction(start);
        // Parse out the implicit body
        ++this.leftrightDepth;
        body = this.parseExpression(false);
        --this.leftrightDepth;
        // Check the next token
        this.expect("\\right", false);
        var right = this.parseFunction();
        return new ParseNode("leftright", {
            body: body,
            left: left.value.value,
            right: right.value.value
        }, this.mode);
    } else if (func === "\\begin") {
        // begin...end is similar to left...right
        var begin = this.parseFunction(start);
        var envName = begin.value.name;
        if (!environments.hasOwnProperty(envName)) {
            throw new ParseError(
                "No such environment: " + envName, begin.value.nameGroup);
        }
        // Build the environment object. Arguments and other information will
        // be made available to the begin and end methods using properties.
        var env = environments[envName];
        var args = this.parseArguments("\\begin{" + envName + "}", env);
        var context = {
            mode: this.mode,
            envName: envName,
            parser: this,
            positions: args.pop()
        };
        var result = env.handler(context, args);
        this.expect("\\end", false);
        var endNameToken = this.nextToken;
        var end = this.parseFunction();
        if (end.value.name !== envName) {
            throw new ParseError(
                "Mismatch: \\begin{" + envName + "} matched " +
                "by \\end{" + end.value.name + "}",
                endNameToken);
        }
        result.position = end.position;
        return result;
    } else if (utils.contains(sizeFuncs, func)) {
        // If we see a sizing function, parse out the implict body
        body = this.parseExpression(false);
        return new ParseNode("sizing", {
            // Figure out what size to use based on the list of functions above
            size: "size" + (utils.indexOf(sizeFuncs, func) + 1),
            value: body
        }, this.mode);
    } else if (utils.contains(styleFuncs, func)) {
        // If we see a styling function, parse out the implict body
        body = this.parseExpression(true);
        return new ParseNode("styling", {
            // Figure out what style to use by pulling out the style from
            // the function name
            style: func.slice(1, func.length - 5),
            value: body
        }, this.mode);
    } else {
        // Defer to parseFunction if it's not a function we handle
        return this.parseFunction(start);
    }
}
```
- example usage
```shell
...
 * Parses a group with optional super/subscripts.
 *
 * @return {?ParseNode}
 */
Parser.prototype.parseAtom = function() {
// The body of an atom is an implicit group, so that things like
// \left(x\right)^2 work correctly.
var base = this.parseImplicitGroup();

// In text mode, we don't have superscripts or subscripts
if (this.mode === "text") {
    return base;
}

// Note that base may be empty (i.e. null) at this point.
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseInput"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseInput ()](#apidoc.element.katex.Parser.prototype.parseInput)
- description and source-code
```javascript
parseInput = function () {
    // Parse an expression
    var expression = this.parseExpression(false);
    // If we succeeded, make sure there's an EOF at the end
    this.expect("EOF", false);
    return expression;
}
```
- example usage
```shell
...
 *
 * @return {?Array.<ParseNode>}
 */
Parser.prototype.parse = function() {
    // Try to parse the input
    this.mode = "math";
    this.consume();
    var parse = this.parseInput();
    return parse;
};

/**
 * Parses an entire input tree.
 */
Parser.prototype.parseInput = function() {
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseRegexGroup"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseRegexGroup (regex, modeName)](#apidoc.element.katex.Parser.prototype.parseRegexGroup)
- description and source-code
```javascript
parseRegexGroup = function (regex, modeName) {
    var outerMode = this.mode;
    this.mode = "text";
    var firstToken = this.nextToken;
    var lastToken = firstToken;
    var str = "";
    while (this.nextToken.text !== "EOF"
           && regex.test(str + this.nextToken.text)) {
        lastToken = this.nextToken;
        str += lastToken.text;
        this.consume();
    }
    if (str === "") {
        throw new ParseError(
            "Invalid " + modeName + ": '" + firstToken.text + "'",
            firstToken);
    }
    this.mode = outerMode;
    return firstToken.range(lastToken, str);
}
```
- example usage
```shell
...

/**
 * Parses a size specification, consisting of magnitude and unit.
 */
Parser.prototype.parseSizeGroup = function(optional) {
var res;
if (!optional && this.nextToken.text !== "{") {
    res = this.parseRegexGroup(
        /^[-+]? *(?:$|\d+|\d+\.\d*|\.\d*) *[a-z]{0,2}$/, "size");
} else {
    res = this.parseStringGroup("size", optional);
}
if (!res) {
    return null;
}
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseSizeGroup"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseSizeGroup (optional)](#apidoc.element.katex.Parser.prototype.parseSizeGroup)
- description and source-code
```javascript
parseSizeGroup = function (optional) {
    var res;
    if (!optional && this.nextToken.text !== "{") {
        res = this.parseRegexGroup(
            /^[-+]? *(?:$|\d+|\d+\.\d*|\.\d*) *[a-z]{0,2}$/, "size");
    } else {
        res = this.parseStringGroup("size", optional);
    }
    if (!res) {
        return null;
    }
    var match = (/([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/).exec(res.text);
    if (!match) {
        throw new ParseError("Invalid size: '" + res.text + "'", res);
    }
    var data = {
        number: +(match[1] + match[2]), // sign + magnitude, cast to number
        unit: match[3]
    };
    if (data.unit !== "em" && data.unit !== "ex" && data.unit !== "mu") {
        throw new ParseError("Invalid unit: '" + data.unit + "'", res);
    }
    return new ParseFuncOrArgument(
        new ParseNode("color", data, this.mode),
        false);
}
```
- example usage
```shell
...
    innerMode = outerMode;
}

if (innerMode === "color") {
    return this.parseColorGroup(optional);
}
if (innerMode === "size") {
    return this.parseSizeGroup(optional);
}

this.switchMode(innerMode);
if (innerMode === "text") {
    // text mode is special because it should ignore the whitespace before
    // it
    while (this.nextToken.text === " ") {
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseStringGroup"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseStringGroup (modeName, optional)](#apidoc.element.katex.Parser.prototype.parseStringGroup)
- description and source-code
```javascript
parseStringGroup = function (modeName, optional) {
    if (optional && this.nextToken.text !== "[") {
        return null;
    }
    var outerMode = this.mode;
    this.mode = "text";
    this.expect(optional ? "[" : "{");
    var str = "";
    var firstToken = this.nextToken;
    var lastToken = firstToken;
    while (this.nextToken.text !== (optional ? "]" : "}")) {
        if (this.nextToken.text === "EOF") {
            throw new ParseError(
                "Unexpected end of input in " + modeName,
                firstToken.range(this.nextToken, str));
        }
        lastToken = this.nextToken;
        str += lastToken.text;
        this.consume();
    }
    this.mode = outerMode;
    this.expect(optional ? "]" : "}");
    return firstToken.range(lastToken, str);
}
```
- example usage
```shell
...
return firstToken.range(lastToken, str);
};

/**
 * Parses a color description.
 */
Parser.prototype.parseColorGroup = function(optional) {
var res = this.parseStringGroup("color", optional);
if (!res) {
    return null;
}
var match = (/^(#[a-z0-9]+|[a-z]+)$/i).exec(res.text);
if (!match) {
    throw new ParseError("Invalid color: '" + res.text + "'", res);
}
...
```

#### <a name="apidoc.element.katex.Parser.prototype.parseSymbol"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>parseSymbol ()](#apidoc.element.katex.Parser.prototype.parseSymbol)
- description and source-code
```javascript
parseSymbol = function () {
    var nucleus = this.nextToken;

    if (functions[nucleus.text]) {
        this.consume();
        // If there exists a function with this name, we return the function and
        // say that it is a function.
        return new ParseFuncOrArgument(
            nucleus.text,
            true, nucleus);
    } else if (symbols[this.mode][nucleus.text]) {
        this.consume();
        // Otherwise if this is a no-argument function, find the type it
        // corresponds to in the symbols map
        return new ParseFuncOrArgument(
            new ParseNode(symbols[this.mode][nucleus.text].group,
                          nucleus.text, this.mode, nucleus),
            false, nucleus);
    } else if (this.mode === "text" && cjkRegex.test(nucleus.text)) {
        this.consume();
        return new ParseFuncOrArgument(
            new ParseNode("textord", nucleus.text, this.mode, nucleus),
            false, nucleus);
    } else {
        return null;
    }
}
```
- example usage
```shell
...
 * implicit grouping after it until the end of the group. E.g.
 *   small text {\Large large text} small text again
 * It is also used for \left and \right to get the correct grouping.
 *
 * @return {?ParseNode}
 */
Parser.prototype.parseImplicitGroup = function() {
var start = this.parseSymbol();

if (start == null) {
    // If we didn't get anything we handle, fall back to parseFunction
    return this.parseFunction();
}

var func = start.result;
...
```

#### <a name="apidoc.element.katex.Parser.prototype.switchMode"></a>[function <span class="apidocSignatureSpan">katex.Parser.prototype.</span>switchMode (newMode)](#apidoc.element.katex.Parser.prototype.switchMode)
- description and source-code
```javascript
switchMode = function (newMode) {
    this.gullet.unget(this.nextToken);
    this.mode = newMode;
    this.consume();
}
```
- example usage
```shell
...
if (innerMode === "color") {
    return this.parseColorGroup(optional);
}
if (innerMode === "size") {
    return this.parseSizeGroup(optional);
}

this.switchMode(innerMode);
if (innerMode === "text") {
    // text mode is special because it should ignore the whitespace before
    // it
    while (this.nextToken.text === " ") {
        this.consume();
    }
}
...
```



# <a name="apidoc.module.katex.buildCommon"></a>[module katex.buildCommon](#apidoc.module.katex.buildCommon)

#### <a name="apidoc.element.katex.buildCommon.makeFragment"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeFragment (children)](#apidoc.element.katex.buildCommon.makeFragment)
- description and source-code
```javascript
makeFragment = function (children) {
    var fragment = new domTree.documentFragment(children);

    sizeElementFromChildren(fragment);

    return fragment;
}
```
- example usage
```shell
...
    false
);

// \color isn't supposed to affect the type of the elements it contains.
// To accomplish this, we wrap the results in a fragment, so the inner
// elements will be able to directly interact with their neighbors. For
// example, '\color{red}{2 +} 3' has the same spacing as '2 + 3'
return new buildCommon.makeFragment(elements);
};

groupTypes.supsub = function(group, options) {
// Superscript and subscripts are handled in the TeXbook on page
// 445-446, rules 18(a-f).

// Here is where we defer to the inner group if it should handle
...
```

#### <a name="apidoc.element.katex.buildCommon.makeOrd"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeOrd (group, options, type)](#apidoc.element.katex.buildCommon.makeOrd)
- description and source-code
```javascript
makeOrd = function (group, options, type) {
    var mode = group.mode;
    var value = group.value;
    if (symbols[mode][value] && symbols[mode][value].replace) {
        value = symbols[mode][value].replace;
    }

    var classes = ["mord"];

    var font = options.font;
    if (font) {
        if (font === "mathit" || utils.contains(mainitLetters, value)) {
            return mathit(value, mode, options, classes);
        } else {
            var fontName = fontMap[font].fontName;
            if (fontMetrics.getCharacterMetrics(value, fontName)) {
                return makeSymbol(
                    value, fontName, mode, options, classes.concat([font]));
            } else {
                return mathDefault(value, mode, options, classes, type);
            }
        }
    } else {
        return mathDefault(value, mode, options, classes, type);
    }
}
```
- example usage
```shell
...
/**
 * This is a map of group types to the function used to handle that type.
 * Simpler types come at the beginning, while complicated types come afterwards.
 */
var groupTypes = {};

groupTypes.mathord = function(group, options) {
    return buildCommon.makeOrd(group, options, "mathord");
};

groupTypes.textord = function(group, options) {
    return buildCommon.makeOrd(group, options, "textord");
};

groupTypes.bin = function(group, options) {
...
```

#### <a name="apidoc.element.katex.buildCommon.makeSpan"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeSpan (classes, children, options)](#apidoc.element.katex.buildCommon.makeSpan)
- description and source-code
```javascript
makeSpan = function (classes, children, options) {
    var span = new domTree.span(classes, children, options);

    sizeElementFromChildren(span);

    return span;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.katex.buildCommon.makeSymbol"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeSymbol (value, fontFamily, mode, options, classes)](#apidoc.element.katex.buildCommon.makeSymbol)
- description and source-code
```javascript
makeSymbol = function (value, fontFamily, mode, options, classes) {
    // Replace the value with its replaced value from symbol.js
    if (symbols[mode][value] && symbols[mode][value].replace) {
        value = symbols[mode][value].replace;
    }

    var metrics = fontMetrics.getCharacterMetrics(value, fontFamily);

    var symbolNode;
    if (metrics) {
        var italic = metrics.italic;
        if (mode === "text") {
            italic = 0;
        }
        symbolNode = new domTree.symbolNode(
            value, metrics.height, metrics.depth, italic, metrics.skew,
            classes);
    } else {
        // TODO(emily): Figure out a good way to only print this in development
        typeof console !== "undefined" && console.warn(
            "No character metrics for '" + value + "' in style '" +
                fontFamily + "'");
        symbolNode = new domTree.symbolNode(value, 0, 0, 0, 0, classes);
    }

    if (options) {
        if (options.style.isTight()) {
            symbolNode.classes.push("mtight");
        }
        if (options.getColor()) {
            symbolNode.style.color = options.getColor();
        }
    }

    return symbolNode;
}
```
- example usage
```shell
...

    var base;
    var baseShift = 0;
    var slant = 0;
    if (group.value.symbol) {
// If this is a symbol, create the symbol.
var fontName = large ? "Size2-Regular" : "Size1-Regular";
base = buildCommon.makeSymbol(
    group.value.body, fontName, "math", options,
    ["mop", "op-symbol", large ? "large-op" : "small-op"]);

// Shift the symbol so its center lies on the axis (rule 13). It
// appears that our fonts have the centers of the symbols already
// almost on the axis, so these numbers are very small. Note we
// don't actually apply this here, but instead it is used either in
...
```

#### <a name="apidoc.element.katex.buildCommon.makeVList"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>makeVList (children, positionType, positionData, options)](#apidoc.element.katex.buildCommon.makeVList)
- description and source-code
```javascript
makeVList = function (children, positionType, positionData, options) {
    var depth;
    var currPos;
    var i;
    if (positionType === "individualShift") {
        var oldChildren = children;
        children = [oldChildren[0]];

        // Add in kerns to the list of children to get each element to be
        // shifted to the correct specified shift
        depth = -oldChildren[0].shift - oldChildren[0].elem.depth;
        currPos = depth;
        for (i = 1; i < oldChildren.length; i++) {
            var diff = -oldChildren[i].shift - currPos -
                oldChildren[i].elem.depth;
            var size = diff -
                (oldChildren[i - 1].elem.height +
                 oldChildren[i - 1].elem.depth);

            currPos = currPos + diff;

            children.push({type: "kern", size: size});
            children.push(oldChildren[i]);
        }
    } else if (positionType === "top") {
        // We always start at the bottom, so calculate the bottom by adding up
        // all the sizes
        var bottom = positionData;
        for (i = 0; i < children.length; i++) {
            if (children[i].type === "kern") {
                bottom -= children[i].size;
            } else {
                bottom -= children[i].elem.height + children[i].elem.depth;
            }
        }
        depth = bottom;
    } else if (positionType === "bottom") {
        depth = -positionData;
    } else if (positionType === "shift") {
        depth = -children[0].elem.depth - positionData;
    } else if (positionType === "firstBaseline") {
        depth = -children[0].elem.depth;
    } else {
        depth = 0;
    }

    // Make the fontSizer
    var maxFontSize = 0;
    for (i = 0; i < children.length; i++) {
        if (children[i].type === "elem") {
            maxFontSize = Math.max(maxFontSize, children[i].elem.maxFontSize);
        }
    }
    var fontSizer = makeFontSizer(options, maxFontSize);

    // Create a new list of actual children at the correct offsets
    var realChildren = [];
    currPos = depth;
    for (i = 0; i < children.length; i++) {
        if (children[i].type === "kern") {
            currPos += children[i].size;
        } else {
            var child = children[i].elem;

            var shift = -child.depth - currPos;
            currPos += child.height + child.depth;

            var childWrap = makeSpan([], [fontSizer, child]);
            childWrap.height -= shift;
            childWrap.depth += shift;
            childWrap.style.top = shift + "em";

            realChildren.push(childWrap);
        }
    }

    // Add in an element at the end with no offset to fix the calculation of
    // baselines in some browsers (namely IE, sometimes safari)
    var baselineFix = makeSpan(
        ["baseline-fix"], [fontSizer, new domTree.symbolNode("\u200b")]);
    realChildren.push(baselineFix);

    var vlist = makeSpan(["vlist"], realChildren);
    // Fix the final height and depth, in case there were kerns at the ends
    // since the makeSpan calculation won't take that in to account.
    vlist.height = Math.max(currPos, vlist.height);
    vlist.depth = Math.max(-depth, vlist.depth);
    return vlist;
}
```
- example usage
```shell
...
    var supsub;
    if (!group.value.sup) {
// Rule 18b
subShift = Math.max(
    subShift, style.metrics.sub1,
    sub.height - 0.8 * style.metrics.xHeight);

supsub = buildCommon.makeVList([
    {type: "elem", elem: submid}
], "shift", subShift, options);

supsub.children[0].style.marginRight = scriptspace;

// Subscripts shouldn't be shifted by the base's italic correction.
// Account for that by shifting the subscript back the appropriate
...
```

#### <a name="apidoc.element.katex.buildCommon.mathsym"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>mathsym (value, mode, options, classes)](#apidoc.element.katex.buildCommon.mathsym)
- description and source-code
```javascript
mathsym = function (value, mode, options, classes) {
    // Decide what font to render the symbol in by its entry in the symbols
    // table.
    // Have a special case for when the value = \ because the \ is used as a
    // textord in unsupported command errors but cannot be parsed as a regular
    // text ordinal and is therefore not present as a symbol in the symbols
    // table for text
    if (value === "\\" || symbols[mode][value].font === "main") {
        return makeSymbol(value, "Main-Regular", mode, options, classes);
    } else {
        return makeSymbol(
            value, "AMS-Regular", mode, options, classes.concat(["amsrm"]));
    }
}
```
- example usage
```shell
...
};

groupTypes.textord = function(group, options) {
    return buildCommon.makeOrd(group, options, "textord");
};

groupTypes.bin = function(group, options) {
    return buildCommon.mathsym(
        group.value, group.mode, options, ["mbin"]);
};

groupTypes.rel = function(group, options) {
    return buildCommon.mathsym(
        group.value, group.mode, options, ["mrel"]);
};
...
```

#### <a name="apidoc.element.katex.buildCommon.prependChildren"></a>[function <span class="apidocSignatureSpan">katex.buildCommon.</span>prependChildren (span, children)](#apidoc.element.katex.buildCommon.prependChildren)
- description and source-code
```javascript
prependChildren = function (span, children) {
    span.children = children.concat(span.children);

    sizeElementFromChildren(span);
}
```
- example usage
```shell
...
        spaces.push(groups[i]);
        groups.splice(i, 1);
        i--;
    } else if (spaces) {
        if (groups[i] instanceof domTree.symbolNode) {
            groups[i] = makeSpan([].concat(groups[i].classes), [groups[i]]);
        }
        buildCommon.prependChildren(groups[i], spaces);
        spaces = null;
    }
}
if (spaces) {
    Array.prototype.push.apply(groups, spaces);
}
...
```



# <a name="apidoc.module.katex.delimiter"></a>[module katex.delimiter](#apidoc.module.katex.delimiter)

#### <a name="apidoc.element.katex.delimiter.customSizedDelim"></a>[function <span class="apidocSignatureSpan">katex.delimiter.</span>customSizedDelim (delim, height, center, options, mode, classes)](#apidoc.element.katex.delimiter.customSizedDelim)
- description and source-code
```javascript
customSizedDelim = function (delim, height, center, options, mode, classes) {
    if (delim === "<" || delim === "\\lt") {
        delim = "\\langle";
    } else if (delim === ">" || delim === "\\gt") {
        delim = "\\rangle";
    }

    // Decide what sequence to use
    var sequence;
    if (utils.contains(stackNeverDelimiters, delim)) {
        sequence = stackNeverDelimiterSequence;
    } else if (utils.contains(stackLargeDelimiters, delim)) {
        sequence = stackLargeDelimiterSequence;
    } else {
        sequence = stackAlwaysDelimiterSequence;
    }

    // Look through the sequence
    var delimType = traverseSequence(delim, height, sequence, options);

    // Depending on the sequence element we decided on, call the appropriate
    // function.
    if (delimType.type === "small") {
        return makeSmallDelim(delim, delimType.style, center, options, mode,
                              classes);
    } else if (delimType.type === "large") {
        return makeLargeDelim(delim, delimType.size, center, options, mode,
                              classes);
    } else if (delimType.type === "stack") {
        return makeStackedDelim(delim, height, center, options, mode, classes);
    }
}
```
- example usage
```shell
...
}

var leftDelim;
var rightDelim;
if (group.value.leftDelim == null) {
    leftDelim = makeNullDelimiter(options, ["mopen"]);
} else {
    leftDelim = delimiter.customSizedDelim(
        group.value.leftDelim, delimSize, true,
        options.withStyle(style), group.mode, ["mopen"]);
}
if (group.value.rightDelim == null) {
    rightDelim = makeNullDelimiter(options, ["mclose"]);
} else {
    rightDelim = delimiter.customSizedDelim(
...
```

#### <a name="apidoc.element.katex.delimiter.leftRightDelim"></a>[function <span class="apidocSignatureSpan">katex.delimiter.</span>leftRightDelim (delim, height, depth, options, mode, classes)](#apidoc.element.katex.delimiter.leftRightDelim)
- description and source-code
```javascript
leftRightDelim = function (delim, height, depth, options, mode, classes) {
    // We always center \left/\right delimiters, so the axis is always shifted
    var axisHeight =
        options.style.metrics.axisHeight * options.style.sizeMultiplier;

    // Taken from TeX source, tex.web, function make_left_right
    var delimiterFactor = 901;
    var delimiterExtend = 5.0 / fontMetrics.metrics.ptPerEm;

    var maxDistFromAxis = Math.max(
        height - axisHeight, depth + axisHeight);

    var totalHeight = Math.max(
        // In real TeX, calculations are done using integral values which are
        // 65536 per pt, or 655360 per em. So, the division here truncates in
        // TeX but doesn't here, producing different results. If we wanted to
        // exactly match TeX's calculation, we could do
        //   Math.floor(655360 * maxDistFromAxis / 500) *
        //    delimiterFactor / 655360
        // (To see the difference, compare
        //    x^{x^{\left(\rule{0.1em}{0.68em}\right)}}
        // in TeX and KaTeX)
        maxDistFromAxis / 500 * delimiterFactor,
        2 * maxDistFromAxis - delimiterExtend);

    // Finally, we defer to 'makeCustomSizedDelim' with our calculated total
    // height
    return makeCustomSizedDelim(delim, totalHeight, true, options, mode,
                                classes);
}
```
- example usage
```shell
...
var leftDelim;
if (group.value.left === ".") {
    // Empty delimiters in \left and \right make null delimiter spaces.
    leftDelim = makeNullDelimiter(options, ["mopen"]);
} else {
    // Otherwise, use leftRightDelim to generate the correct sized
    // delimiter.
    leftDelim = delimiter.leftRightDelim(
        group.value.left, innerHeight, innerDepth, options,
        group.mode, ["mopen"]);
}
// Add it to the beginning of the expression
inner.unshift(leftDelim);

// Handle middle delimiters
...
```

#### <a name="apidoc.element.katex.delimiter.sizedDelim"></a>[function <span class="apidocSignatureSpan">katex.delimiter.</span>sizedDelim (delim, size, options, mode, classes)](#apidoc.element.katex.delimiter.sizedDelim)
- description and source-code
```javascript
sizedDelim = function (delim, size, options, mode, classes) {
    // < and > turn into \langle and \rangle in delimiters
    if (delim === "<" || delim === "\\lt") {
        delim = "\\langle";
    } else if (delim === ">" || delim === "\\gt") {
        delim = "\\rangle";
    }

    // Sized delimiters are never centered.
    if (utils.contains(stackLargeDelimiters, delim) ||
        utils.contains(stackNeverDelimiters, delim)) {
        return makeLargeDelim(delim, size, false, options, mode, classes);
    } else if (utils.contains(stackAlwaysDelimiters, delim)) {
        return makeStackedDelim(
            delim, sizeToMaxHeight[size], false, options, mode, classes);
    } else {
        throw new ParseError("Illegal delimiter: '" + delim + "'");
    }
}
```
- example usage
```shell
...
if (delim === ".") {
    // Empty delimiters still count as elements, even though they don't
    // show anything.
    return makeSpan([group.value.mclass]);
}

// Use delimiter.sizedDelim to generate the delimiter.
return delimiter.sizedDelim(
        delim, group.value.size, options, group.mode,
        [group.value.mclass]);
};

groupTypes.leftright = function(group, options) {
// Build the inner expression
var inner = buildExpression(group.value.body, options.reset(), true);
...
```



# <a name="apidoc.module.katex.domTree"></a>[module katex.domTree](#apidoc.module.katex.domTree)

#### <a name="apidoc.element.katex.domTree.documentFragment"></a>[function <span class="apidocSignatureSpan">katex.domTree.</span>documentFragment (children)](#apidoc.element.katex.domTree.documentFragment)
- description and source-code
```javascript
function documentFragment(children) {
    this.children = children || [];
    this.height = 0;
    this.depth = 0;
    this.maxFontSize = 0;
}
```
- example usage
```shell
...
    sizeElementFromChildren(span);
};

/**
 * Makes a document fragment with the given list of children.
 */
var makeFragment = function(children) {
    var fragment = new domTree.documentFragment(children);

    sizeElementFromChildren(fragment);

    return fragment;
};

/**
...
```

#### <a name="apidoc.element.katex.domTree.span"></a>[function <span class="apidocSignatureSpan">katex.domTree.</span>span (classes, children, options)](#apidoc.element.katex.domTree.span)
- description and source-code
```javascript
function span(classes, children, options) {
    this.classes = classes || [];
    this.children = children || [];
    this.height = 0;
    this.depth = 0;
    this.maxFontSize = 0;
    this.style = {};
    this.attributes = {};
    if (options) {
        if (options.style.isTight()) {
            this.classes.push("mtight");
        }
        if (options.getColor()) {
            this.style.color = options.getColor();
        }
    }
}
```
- example usage
```shell
...
 *
 * TODO: Ensure that 'options' is always provided (currently some call sites
 * don't pass it).
 * TODO: add a separate argument for math class (e.g. 'mop', 'mbin'), which
 * should if present come first in 'classes'.
 */
var makeSpan = function(classes, children, options) {
    var span = new domTree.span(classes, children, options);

    sizeElementFromChildren(span);

    return span;
};

/**
...
```

#### <a name="apidoc.element.katex.domTree.symbolNode"></a>[function <span class="apidocSignatureSpan">katex.domTree.</span>symbolNode (value, height, depth, italic, skew, classes, style)](#apidoc.element.katex.domTree.symbolNode)
- description and source-code
```javascript
function symbolNode(value, height, depth, italic, skew, classes, style) {
    this.value = value || "";
    this.height = height || 0;
    this.depth = depth || 0;
    this.italic = italic || 0;
    this.skew = skew || 0;
    this.classes = classes || [];
    this.style = style || {};
    this.maxFontSize = 0;

    // Mark CJK characters with specific classes so that we can specify which
    // fonts to use.  This allows us to render these characters with a serif
    // font in situations where the browser would either default to a sans serif
    // or render a placeholder character.
    if (unicodeRegexes.cjkRegex.test(value)) {
        // I couldn't find any fonts that contained Hangul as well as all of
        // the other characters we wanted to test there for it gets its own
        // CSS class.
        if (unicodeRegexes.hangulRegex.test(value)) {
            this.classes.push('hangul_fallback');
        } else {
            this.classes.push('cjk_fallback');
        }
    }

    if (/[îïíì]/.test(this.value)) {    // add ī when we add Extended Latin
        this.value = iCombinations[this.value];
    }
}
```
- example usage
```shell
...

var symbolNode;
if (metrics) {
    var italic = metrics.italic;
    if (mode === "text") {
        italic = 0;
    }
    symbolNode = new domTree.symbolNode(
        value, metrics.height, metrics.depth, italic, metrics.skew,
        classes);
} else {
    // TODO(emily): Figure out a good way to only print this in development
    typeof console !== "undefined" && console.warn(
        "No character metrics for '" + value + "' in style '" +
            fontFamily + "'");
...
```



# <a name="apidoc.module.katex.fontMetrics"></a>[module katex.fontMetrics](#apidoc.module.katex.fontMetrics)

#### <a name="apidoc.element.katex.fontMetrics.getCharacterMetrics"></a>[function <span class="apidocSignatureSpan">katex.fontMetrics.</span>getCharacterMetrics (character, style)](#apidoc.element.katex.fontMetrics.getCharacterMetrics)
- description and source-code
```javascript
getCharacterMetrics = function (character, style) {
    var ch = character.charCodeAt(0);
    if (character[0] in extraCharacterMap) {
        ch = extraCharacterMap[character[0]].charCodeAt(0);
    } else if (cjkRegex.test(character[0])) {
        ch = 'M'.charCodeAt(0);
    }
    var metrics = metricMap[style][ch];
    if (metrics) {
        return {
            depth: metrics[0],
            height: metrics[1],
            italic: metrics[2],
            skew: metrics[3],
            width: metrics[4]
        };
    }
}
```
- example usage
```shell
...
 */
var makeSymbol = function(value, fontFamily, mode, options, classes) {
// Replace the value with its replaced value from symbol.js
if (symbols[mode][value] && symbols[mode][value].replace) {
    value = symbols[mode][value].replace;
}

var metrics = fontMetrics.getCharacterMetrics(value, fontFamily);

var symbolNode;
if (metrics) {
    var italic = metrics.italic;
    if (mode === "text") {
        italic = 0;
    }
...
```



# <a name="apidoc.module.katex.mathMLTree"></a>[module katex.mathMLTree](#apidoc.module.katex.mathMLTree)

#### <a name="apidoc.element.katex.mathMLTree.MathNode"></a>[function <span class="apidocSignatureSpan">katex.mathMLTree.</span>MathNode (type, children)](#apidoc.element.katex.mathMLTree.MathNode)
- description and source-code
```javascript
function MathNode(type, children) {
    this.type = type;
    this.attributes = {};
    this.children = children || [];
}
```
- example usage
```shell
...
/**
 * Functions for handling the different types of groups found in the parse
 * tree. Each function should take a parse group and return a MathML node.
 */
var groupTypes = {};

groupTypes.mathord = function(group, options) {
var node = new mathMLTree.MathNode(
    "mi",
    [makeText(group.value, group.mode)]);

var variant = getVariant(group, options);
if (variant) {
    node.setAttribute("mathvariant", variant);
}
...
```

#### <a name="apidoc.element.katex.mathMLTree.TextNode"></a>[function <span class="apidocSignatureSpan">katex.mathMLTree.</span>TextNode (text)](#apidoc.element.katex.mathMLTree.TextNode)
- description and source-code
```javascript
function TextNode(text) {
    this.text = text;
}
```
- example usage
```shell
...
 * optional replacement from symbols.js.
 */
var makeText = function(text, mode) {
if (symbols[mode][text] && symbols[mode][text].replace) {
    text = symbols[mode][text].replace;
}

return new mathMLTree.TextNode(text);
};

/**
 * Returns the math variant as a string or null if none is required.
 */
var getVariant = function(group, options) {
var font = options.font;
...
```



# <a name="apidoc.module.katex.parseData"></a>[module katex.parseData](#apidoc.module.katex.parseData)

#### <a name="apidoc.element.katex.parseData.ParseNode"></a>[function <span class="apidocSignatureSpan">katex.parseData.</span>ParseNode (type, value, mode, firstToken, lastToken)](#apidoc.element.katex.parseData.ParseNode)
- description and source-code
```javascript
function ParseNode(type, value, mode, firstToken, lastToken) {
    this.type = type;
    this.value = value;
    this.mode = mode;
    if (firstToken && (!lastToken || lastToken.lexer === firstToken.lexer)) {
        this.lexer = firstToken.lexer;
        this.start = firstToken.start;
        this.end = (lastToken || firstToken).end;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.katex.utils"></a>[module katex.utils](#apidoc.module.katex.utils)

#### <a name="apidoc.element.katex.utils.clearNode"></a>[function <span class="apidocSignatureSpan">katex.utils.</span>clearNode (node)](#apidoc.element.katex.utils.clearNode)
- description and source-code
```javascript
function clearNode(node) {
    setTextContent(node, "");
}
```
- example usage
```shell
...
var utils = require("./src/utils");

/**
 * Parse and build an expression, and place that expression in the DOM node
 * given.
 */
var render = function(expression, baseNode, options) {
utils.clearNode(baseNode);

var settings = new Settings(options);

var tree = parseTree(expression, settings);
var node = buildTree(tree, expression, settings).toNode();

baseNode.appendChild(node);
...
```

#### <a name="apidoc.element.katex.utils.contains"></a>[function <span class="apidocSignatureSpan">katex.utils.</span>contains (list, elem)](#apidoc.element.katex.utils.contains)
- description and source-code
```javascript
contains = function (list, elem) {
    return indexOf(list, elem) !== -1;
}
```
- example usage
```shell
...
        throw new ParseError(
            "Mismatch: \\begin{" + envName + "} matched " +
            "by \\end{" + end.value.name + "}",
            endNameToken);
    }
    result.position = end.position;
    return result;
} else if (utils.contains(sizeFuncs, func)) {
    // If we see a sizing function, parse out the implict body
    body = this.parseExpression(false);
    return new ParseNode("sizing", {
        // Figure out what size to use based on the list of functions above
        size: "size" + (utils.indexOf(sizeFuncs, func) + 1),
        value: body
    }, this.mode);
...
```

#### <a name="apidoc.element.katex.utils.deflt"></a>[function <span class="apidocSignatureSpan">katex.utils.</span>deflt (setting, defaultIfUndefined)](#apidoc.element.katex.utils.deflt)
- description and source-code
```javascript
deflt = function (setting, defaultIfUndefined) {
    return setting === undefined ? defaultIfUndefined : setting;
}
```
- example usage
```shell
...
var pt = 1 / fontMetrics.metrics.ptPerEm;
var arraycolsep = 5 * pt; // \arraycolsep in article.cls

// Vertical spacing
var baselineskip = 12 * pt; // see size10.clo
// Default \arraystretch from lttab.dtx
// TODO(gagern): may get redefined once we have user-defined macros
var arraystretch = utils.deflt(group.value.arraystretch, 1);
var arrayskip = arraystretch * baselineskip;
var arstrutHeight = 0.7 * arrayskip; // \strutbox in ltfsstrc.dtx and
var arstrutDepth = 0.3 * arrayskip;  // \@arstrutbox in lttab.dtx

var totalHeight = 0;
for (r = 0; r < group.value.body.length; ++r) {
    var inrow = group.value.body[r];
...
```

#### <a name="apidoc.element.katex.utils.escape"></a>[function <span class="apidocSignatureSpan">katex.utils.</span>escape (text)](#apidoc.element.katex.utils.escape)
- description and source-code
```javascript
function escape(text) {
    return ("" + text).replace(ESCAPE_REGEX, escaper);
}
```
- example usage
```shell
...
 */
span.prototype.toMarkup = function() {
var markup = "<span";

// Add the class
if (this.classes.length) {
    markup += " class=\"";
    markup += utils.escape(createClass(this.classes));
    markup += "\"";
}

var styles = "";

// Add the styles, after hyphenation
for (var style in this.style) {
...
```

#### <a name="apidoc.element.katex.utils.hyphenate"></a>[function <span class="apidocSignatureSpan">katex.utils.</span>hyphenate (str)](#apidoc.element.katex.utils.hyphenate)
- description and source-code
```javascript
hyphenate = function (str) {
    return str.replace(uppercase, "-$1").toLowerCase();
}
```
- example usage
```shell
...
}

var styles = "";

// Add the styles, after hyphenation
for (var style in this.style) {
    if (this.style.hasOwnProperty(style)) {
        styles += utils.hyphenate(style) + ":" + this.style[style] + ";";
    }
}

if (styles) {
    markup += " style=\"" + utils.escape(styles) + "\"";
}
...
```

#### <a name="apidoc.element.katex.utils.indexOf"></a>[function <span class="apidocSignatureSpan">katex.utils.</span>indexOf (list, elem)](#apidoc.element.katex.utils.indexOf)
- description and source-code
```javascript
indexOf = function (list, elem) {
    if (list == null) {
        return -1;
    }
    if (nativeIndexOf && list.indexOf === nativeIndexOf) {
        return list.indexOf(elem);
    }
    var i = 0;
    var l = list.length;
    for (; i < l; i++) {
        if (list[i] === elem) {
            return i;
        }
    }
    return -1;
}
```
- example usage
```shell
...
 */
Parser.prototype.parseExpression = function(breakOnInfix, breakOnTokenText) {
var body = [];
// Keep adding atoms to the body until we can't parse any more atoms (either
// we reached the end, a }, or a \right)
while (true) {
    var lex = this.nextToken;
    if (endOfExpression.indexOf(lex.text) !== -1) {
        break;
    }
    if (breakOnTokenText && lex.text === breakOnTokenText) {
        break;
    }
    if (breakOnInfix && functions[lex.text] && functions[lex.text].infix) {
        break;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
