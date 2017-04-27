# npmdoc-tape

#### basic api documentation for  [tape (v4.6.3)](https://github.com/substack/tape)  [![npm package](https://img.shields.io/npm/v/npmdoc-tape.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tape) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tape.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tape)

#### tap-producing test harness for node and browsers

[![NPM](https://nodei.co/npm/tape.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/tape)

- [https://npmdoc.github.io/node-npmdoc-tape/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-tape/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tape/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tape/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tape/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tape/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Halliday",
        "url": "http://substack.net"
    },
    "bin": {
        "tape": "./bin/tape"
    },
    "bugs": {
        "url": "https://github.com/substack/tape/issues"
    },
    "dependencies": {
        "deep-equal": "~1.0.1",
        "defined": "~1.0.0",
        "for-each": "~0.3.2",
        "function-bind": "~1.1.0",
        "glob": "~7.1.1",
        "has": "~1.0.1",
        "inherits": "~2.0.3",
        "minimist": "~1.2.0",
        "object-inspect": "~1.2.1",
        "resolve": "~1.1.7",
        "resumer": "~0.0.0",
        "string.prototype.trim": "~1.1.2",
        "through": "~2.3.8"
    },
    "description": "tap-producing test harness for node and browsers",
    "devDependencies": {
        "concat-stream": "~1.5.2",
        "falafel": "~2.0.0",
        "js-yaml": "~3.7.0",
        "tap": "~7.1.1",
        "tap-parser": "~3.0.4"
    },
    "directories": {
        "example": "example",
        "test": "test"
    },
    "dist": {
        "shasum": "637e77581e9ab2ce17577e9bd4ce4f575806d8b6",
        "tarball": "https://registry.npmjs.org/tape/-/tape-4.6.3.tgz"
    },
    "gitHead": "72213e119fb9c52e7620fdc58908b1227dd1c9f8",
    "homepage": "https://github.com/substack/tape",
    "keywords": [
        "tap",
        "test",
        "harness",
        "assert",
        "browser"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "substack"
        },
        {
            "name": "raynos"
        },
        {
            "name": "domenic"
        },
        {
            "name": "ljharb"
        }
    ],
    "name": "tape",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/substack/tape.git"
    },
    "scripts": {
        "test": "tap test/*.js"
    },
    "testling": {
        "files": "test/browser/*.js",
        "browsers": [
            "ie/6..latest",
            "chrome/20..latest",
            "firefox/10..latest",
            "safari/latest",
            "opera/11.0..latest",
            "iphone/6",
            "ipad/6"
        ]
    },
    "version": "4.6.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
