# api documentation for  [tape (v4.6.3)](https://github.com/substack/tape)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tape.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tape)
#### tap-producing test harness for node and browsers

[![NPM](https://nodei.co/npm/tape.png?downloads=true)](https://www.npmjs.com/package/tape)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tape/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-tape_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tape/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-tape/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "James Halliday",
        "email": "mail@substack.net",
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
            "name": "substack",
            "email": "substack@gmail.com"
        },
        {
            "name": "raynos",
            "email": "raynos2@gmail.com"
        },
        {
            "name": "domenic",
            "email": "d@domenic.me"
        },
        {
            "name": "ljharb",
            "email": "ljharb@gmail.com"
        }
    ],
    "name": "tape",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tape](#apidoc.module.tape)
1.  [function <span class="apidocSignatureSpan">tape.</span>Test (name_, opts_, cb_)](#apidoc.element.tape.Test)
1.  [function <span class="apidocSignatureSpan">tape.</span>createHarness (conf_)](#apidoc.element.tape.createHarness)
1.  [function <span class="apidocSignatureSpan">tape.</span>createStream (opts)](#apidoc.element.tape.createStream)
1.  [function <span class="apidocSignatureSpan">tape.</span>getHarness (opts)](#apidoc.element.tape.getHarness)
1.  [function <span class="apidocSignatureSpan">tape.</span>onFinish ()](#apidoc.element.tape.onFinish)
1.  [function <span class="apidocSignatureSpan">tape.</span>only ()](#apidoc.element.tape.only)
1.  [function <span class="apidocSignatureSpan">tape.</span>results ()](#apidoc.element.tape.results)
1.  [function <span class="apidocSignatureSpan">tape.</span>skip (name_, _opts, _cb)](#apidoc.element.tape.skip)
1.  [function <span class="apidocSignatureSpan">tape.</span>test ()](#apidoc.element.tape.test)
1.  object <span class="apidocSignatureSpan">tape.</span>Test.prototype
1.  object <span class="apidocSignatureSpan">tape.</span>results.prototype

#### [module tape.Test](#apidoc.module.tape.Test)
1.  [function <span class="apidocSignatureSpan">tape.</span>Test (name_, opts_, cb_)](#apidoc.element.tape.Test.Test)
1.  [function <span class="apidocSignatureSpan">tape.Test.</span>skip (name_, _opts, _cb)](#apidoc.element.tape.Test.skip)
1.  [function <span class="apidocSignatureSpan">tape.Test.</span>super_ ()](#apidoc.element.tape.Test.super_)

#### [module tape.Test.prototype](#apidoc.module.tape.Test.prototype)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_assert (ok, opts)](#apidoc.element.tape.Test.prototype._assert)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_end (err)](#apidoc.element.tape.Test.prototype._end)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_exit ()](#apidoc.element.tape.Test.prototype._exit)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_pendingAsserts ()](#apidoc.element.tape.Test.prototype._pendingAsserts)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>assert (value, msg, extra)](#apidoc.element.tape.Test.prototype.assert)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>comment (msg)](#apidoc.element.tape.Test.prototype.comment)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>deepEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.deepEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>deepEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.deepEquals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>deepLooseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.deepLooseEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>doesNotEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.doesNotEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>doesNotThrow (fn, expected, msg, extra)](#apidoc.element.tape.Test.prototype.doesNotThrow)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>end (err)](#apidoc.element.tape.Test.prototype.end)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>equal (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.equal)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>equals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.equals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>error (err, msg, extra)](#apidoc.element.tape.Test.prototype.error)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>fail (msg, extra)](#apidoc.element.tape.Test.prototype.fail)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>false (value, msg, extra)](#apidoc.element.tape.Test.prototype.false)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>ifErr (err, msg, extra)](#apidoc.element.tape.Test.prototype.ifErr)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>ifError (err, msg, extra)](#apidoc.element.tape.Test.prototype.ifError)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>iferror (err, msg, extra)](#apidoc.element.tape.Test.prototype.iferror)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>is (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.is)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isEquivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isEquivalent)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isInequal (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isInequal)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isInequivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isInequivalent)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNot (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNot)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotDeepEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotDeepEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotDeeply (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotDeeply)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotEquivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotEquivalent)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>looseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.looseEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>looseEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.looseEquals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>not (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.not)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notDeepEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notDeepEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notDeepLooseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notDeepLooseEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notDeeply (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notDeeply)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notEquals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notEquivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notEquivalent)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notLooseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notLooseEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notLooseEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notLooseEquals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notOk (value, msg, extra)](#apidoc.element.tape.Test.prototype.notOk)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notSame (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notSame)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notStrictEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notStrictEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notStrictEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notStrictEquals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notok (value, msg, extra)](#apidoc.element.tape.Test.prototype.notok)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>ok (value, msg, extra)](#apidoc.element.tape.Test.prototype.ok)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>pass (msg, extra)](#apidoc.element.tape.Test.prototype.pass)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>plan (n)](#apidoc.element.tape.Test.prototype.plan)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>run ()](#apidoc.element.tape.Test.prototype.run)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>same (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.same)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>skip (msg, extra)](#apidoc.element.tape.Test.prototype.skip)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>strictEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.strictEqual)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>strictEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.strictEquals)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>test (name, opts, cb)](#apidoc.element.tape.Test.prototype.test)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>throws (fn, expected, msg, extra)](#apidoc.element.tape.Test.prototype.throws)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>timeoutAfter (ms)](#apidoc.element.tape.Test.prototype.timeoutAfter)
1.  [function <span class="apidocSignatureSpan">tape.Test.prototype.</span>true (value, msg, extra)](#apidoc.element.tape.Test.prototype.true)

#### [module tape.results](#apidoc.module.tape.results)
1.  [function <span class="apidocSignatureSpan">tape.</span>results ()](#apidoc.element.tape.results.results)
1.  [function <span class="apidocSignatureSpan">tape.results.</span>super_ ()](#apidoc.element.tape.results.super_)

#### [module tape.results.prototype](#apidoc.module.tape.results.prototype)
1.  [function <span class="apidocSignatureSpan">tape.results.prototype.</span>_watch (t)](#apidoc.element.tape.results.prototype._watch)
1.  [function <span class="apidocSignatureSpan">tape.results.prototype.</span>close ()](#apidoc.element.tape.results.prototype.close)
1.  [function <span class="apidocSignatureSpan">tape.results.prototype.</span>createStream (opts)](#apidoc.element.tape.results.prototype.createStream)
1.  [function <span class="apidocSignatureSpan">tape.results.prototype.</span>only (t)](#apidoc.element.tape.results.prototype.only)
1.  [function <span class="apidocSignatureSpan">tape.results.prototype.</span>push (t)](#apidoc.element.tape.results.prototype.push)



# <a name="apidoc.module.tape"></a>[module tape](#apidoc.module.tape)

#### <a name="apidoc.element.tape.Test"></a>[function <span class="apidocSignatureSpan">tape.</span>Test (name_, opts_, cb_)](#apidoc.element.tape.Test)
- description and source-code
```javascript
function Test(name_, opts_, cb_) {
    if (! (this instanceof Test)) {
        return new Test(name_, opts_, cb_);
    }

    var args = getTestArgs(name_, opts_, cb_);

    this.readable = true;
    this.name = args.name || '(anonymous)';
    this.assertCount = 0;
    this.pendingCount = 0;
    this._skip = args.opts.skip || false;
    this._timeout = args.opts.timeout;
    this._objectPrintDepth = args.opts.objectPrintDepth || 5;
    this._plan = undefined;
    this._cb = args.cb;
    this._progeny = [];
    this._ok = true;

    for (var prop in this) {
        this[prop] = (function bind(self, val) {
            if (typeof val === 'function') {
                return function bound() {
                    return val.apply(self, arguments);
                };
            }
            else return val;
        })(this, this[prop]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.createHarness"></a>[function <span class="apidocSignatureSpan">tape.</span>createHarness (conf_)](#apidoc.element.tape.createHarness)
- description and source-code
```javascript
function createHarness(conf_) {
    if (!conf_) conf_ = {};
    var results = createResult();
    if (conf_.autoclose !== false) {
        results.once('done', function () { results.close() });
    }

    var test = function (name, conf, cb) {
        var t = new Test(name, conf, cb);
        test._tests.push(t);

        (function inspectCode (st) {
            st.on('test', function sub (st_) {
                inspectCode(st_);
            });
            st.on('result', function (r) {
                if (!r.ok && typeof r !== 'string') test._exitCode = 1
            });
        })(t);

        results.push(t);
        return t;
    };
    test._results = results;

    test._tests = [];

    test.createStream = function (opts) {
        return results.createStream(opts);
    };

    test.onFinish = function (cb) {
        results.on('done', cb);
    };

    var only = false;
    test.only = function () {
        if (only) throw new Error('there can only be one only test');
        only = true;
        var t = test.apply(null, arguments);
        results.only(t);
        return t;
    };
    test._exitCode = 0;

    test.close = function () { results.close() };

    return test;
}
```
- example usage
```shell
...

You may pass the same options that ['test()'](#testname-opts-cb) accepts.

## t.comment(message)

Print a message without breaking the tap output. (Useful when using e.g. 'tap-colorize' where output is buffered & 'console.log'
will print in incorrect order vis-a-vis tap output.)

## var htest = test.createHarness()

Create a new test harness instance, which is a function like 'test()', but with
a new pending stack and test state.

By default the TAP output goes to 'console.log()'. You can pipe the output to
someplace else if you 'htest.createStream().pipe()' to a destination stream on
the first tick.
...
```

#### <a name="apidoc.element.tape.createStream"></a>[function <span class="apidocSignatureSpan">tape.</span>createStream (opts)](#apidoc.element.tape.createStream)
- description and source-code
```javascript
createStream = function (opts) {
    if (!opts) opts = {};
    if (!harness) {
        var output = through();
        getHarness({ stream: output, objectMode: opts.objectMode });
        return output;
    }
    return harness.createStream(opts);
}
```
- example usage
```shell
...
lazyLoad.createStream = function (opts) {
    if (!opts) opts = {};
    if (!harness) {
        var output = through();
        getHarness({ stream: output, objectMode: opts.objectMode });
        return output;
    }
    return harness.createStream(opts);
};

lazyLoad.onFinish = function () {
    return getHarness().onFinish.apply(this, arguments);
};

lazyLoad.getHarness = getHarness
...
```

#### <a name="apidoc.element.tape.getHarness"></a>[function <span class="apidocSignatureSpan">tape.</span>getHarness (opts)](#apidoc.element.tape.getHarness)
- description and source-code
```javascript
function getHarness(opts) {
    if (!opts) opts = {};
    opts.autoclose = !canEmitExit;
    if (!harness) harness = createExitHarness(opts);
    return harness;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.onFinish"></a>[function <span class="apidocSignatureSpan">tape.</span>onFinish ()](#apidoc.element.tape.onFinish)
- description and source-code
```javascript
onFinish = function () {
    return getHarness().onFinish.apply(this, arguments);
}
```
- example usage
```shell
...
If you forget to 't.plan()' out how many assertions you are going to run and you
don't call 't.end()' explicitly, your test will hang.

## test.skip(name, cb)

Generate a new test that will be skipped over.

## test.onFinish(fn)

The onFinish hook will get invoked when ALL tape tests have finished
right before tape is about to print the test summary.

## t.plan(n)

Declare that 'n' assertions should be run. 't.end()' will be called
...
```

#### <a name="apidoc.element.tape.only"></a>[function <span class="apidocSignatureSpan">tape.</span>only ()](#apidoc.element.tape.only)
- description and source-code
```javascript
only = function () {
    return getHarness().only.apply(this, arguments);
}
```
- example usage
```shell
...
};

var only = false;
test.only = function () {
    if (only) throw new Error('there can only be one only test');
    only = true;
    var t = test.apply(null, arguments);
    results.only(t);
    return t;
};
test._exitCode = 0;

test.close = function () { results.close() };

return test;
...
```

#### <a name="apidoc.element.tape.results"></a>[function <span class="apidocSignatureSpan">tape.</span>results ()](#apidoc.element.tape.results)
- description and source-code
```javascript
function Results() {
    if (!(this instanceof Results)) return new Results;
    this.count = 0;
    this.fail = 0;
    this.pass = 0;
    this._stream = through();
    this.tests = [];
    this._only = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.skip"></a>[function <span class="apidocSignatureSpan">tape.</span>skip (name_, _opts, _cb)](#apidoc.element.tape.skip)
- description and source-code
```javascript
skip = function (name_, _opts, _cb) {
    var args = getTestArgs.apply(null, arguments);
    args.opts.skip = true;
    return Test(args.name, args.opts, args.cb);
}
```
- example usage
```shell
...
  See test.timeoutAfter.
- opts.objectPrintDepth = 5. Configure max depth of expected / actual object
  printing.

If you forget to 't.plan()' out how many assertions you are going to run and you
don't call 't.end()' explicitly, your test will hang.

## test.skip(name, cb)

Generate a new test that will be skipped over.

## test.onFinish(fn)

The onFinish hook will get invoked when ALL tape tests have finished
right before tape is about to print the test summary.
...
```

#### <a name="apidoc.element.tape.test"></a>[function <span class="apidocSignatureSpan">tape.</span>test ()](#apidoc.element.tape.test)
- description and source-code
```javascript
test = function () {
    return getHarness().apply(this, arguments);
}
```
- example usage
```shell
...

Assert that the function call 'fn()' throws an exception. 'expected', if present, must be a 'RegExp' or 'Function'. The 'RegExp'
matches the string representation of the exception, as generated by 'err.toString()'. The 'Function' is the exception thrown (e.
g. 'Error'). 'msg' is an optional description of the assertion.

## t.doesNotThrow(fn, expected, msg)

Assert that the function call 'fn()' does not throw an exception. 'msg' is an optional description of the assertion.

## t.test(name, [opts], cb)

Create a subtest with a new test handle 'st' from 'cb(st)' inside the current
test 't'. 'cb(st)' will only fire when 't' finishes. Additional tests queued up
after 't' will not be run until all subtests finish.

You may pass the same options that ['test()'](#testname-opts-cb) accepts.
...
```



# <a name="apidoc.module.tape.Test"></a>[module tape.Test](#apidoc.module.tape.Test)

#### <a name="apidoc.element.tape.Test.Test"></a>[function <span class="apidocSignatureSpan">tape.</span>Test (name_, opts_, cb_)](#apidoc.element.tape.Test.Test)
- description and source-code
```javascript
function Test(name_, opts_, cb_) {
    if (! (this instanceof Test)) {
        return new Test(name_, opts_, cb_);
    }

    var args = getTestArgs(name_, opts_, cb_);

    this.readable = true;
    this.name = args.name || '(anonymous)';
    this.assertCount = 0;
    this.pendingCount = 0;
    this._skip = args.opts.skip || false;
    this._timeout = args.opts.timeout;
    this._objectPrintDepth = args.opts.objectPrintDepth || 5;
    this._plan = undefined;
    this._cb = args.cb;
    this._progeny = [];
    this._ok = true;

    for (var prop in this) {
        this[prop] = (function bind(self, val) {
            if (typeof val === 'function') {
                return function bound() {
                    return val.apply(self, arguments);
                };
            }
            else return val;
        })(this, this[prop]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.Test.skip"></a>[function <span class="apidocSignatureSpan">tape.Test.</span>skip (name_, _opts, _cb)](#apidoc.element.tape.Test.skip)
- description and source-code
```javascript
skip = function (name_, _opts, _cb) {
    var args = getTestArgs.apply(null, arguments);
    args.opts.skip = true;
    return Test(args.name, args.opts, args.cb);
}
```
- example usage
```shell
...
  See test.timeoutAfter.
- opts.objectPrintDepth = 5. Configure max depth of expected / actual object
  printing.

If you forget to 't.plan()' out how many assertions you are going to run and you
don't call 't.end()' explicitly, your test will hang.

## test.skip(name, cb)

Generate a new test that will be skipped over.

## test.onFinish(fn)

The onFinish hook will get invoked when ALL tape tests have finished
right before tape is about to print the test summary.
...
```

#### <a name="apidoc.element.tape.Test.super_"></a>[function <span class="apidocSignatureSpan">tape.Test.</span>super_ ()](#apidoc.element.tape.Test.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tape.Test.prototype"></a>[module tape.Test.prototype](#apidoc.module.tape.Test.prototype)

#### <a name="apidoc.element.tape.Test.prototype._assert"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_assert (ok, opts)](#apidoc.element.tape.Test.prototype._assert)
- description and source-code
```javascript
function assert(ok, opts) {
    var self = this;
    var extra = opts.extra || {};

    var res = {
        id : self.assertCount ++,
        ok : Boolean(ok),
        skip : defined(extra.skip, opts.skip),
        name : defined(extra.message, opts.message, '(unnamed assert)'),
        operator : defined(extra.operator, opts.operator),
        objectPrintDepth : self._objectPrintDepth
    };
    if (has(opts, 'actual') || has(extra, 'actual')) {
        res.actual = defined(extra.actual, opts.actual);
    }
    if (has(opts, 'expected') || has(extra, 'expected')) {
        res.expected = defined(extra.expected, opts.expected);
    }
    this._ok = Boolean(this._ok && ok);

    if (!ok) {
        res.error = defined(extra.error, opts.error, new Error(res.name));
    }

    if (!ok) {
        var e = new Error('exception');
        var err = (e.stack || '').split('\n');
        var dir = path.dirname(__dirname) + path.sep;

        for (var i = 0; i < err.length; i++) {
            var m = /^[^\s]*\s*\bat\s+(.+)/.exec(err[i]);
            if (!m) {
                continue;
            }

            var s = m[1].split(/\s+/);
            var filem = /((?:\/|[A-Z]:\\)[^:\s]+:(\d+)(?::(\d+))?)/.exec(s[1]);
            if (!filem) {
                filem = /((?:\/|[A-Z]:\\)[^:\s]+:(\d+)(?::(\d+))?)/.exec(s[2]);

                if (!filem) {
                    filem = /((?:\/|[A-Z]:\\)[^:\s]+:(\d+)(?::(\d+))?)/.exec(s[3]);

                    if (!filem) {
                        continue;
                    }
                }
            }

            if (filem[1].slice(0, dir.length) === dir) {
                continue;
            }

            res.functionName = s[0];
            res.file = filem[1];
            res.line = Number(filem[2]);
            if (filem[3]) res.column = filem[3];

            res.at = m[1];
            break;
        }
    }

    self.emit('result', res);

    var pendingAsserts = self._pendingAsserts();
    if (!pendingAsserts) {
        if (extra.exiting) {
            self._end();
        } else {
            nextTick(function () {
                self._end();
            });
        }
    }

    if (!self._planError && pendingAsserts < 0) {
        self._planError = true;
        self.fail('plan != count', {
            expected : self._plan,
            actual : self._plan - pendingAsserts
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.Test.prototype._end"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_end (err)](#apidoc.element.tape.Test.prototype._end)
- description and source-code
```javascript
_end = function (err) {
    var self = this;
    if (this._progeny.length) {
        var t = this._progeny.shift();
        t.on('end', function () { self._end() });
        t.run();
        return;
    }

    if (!this.ended) this.emit('end');
    var pendingAsserts = this._pendingAsserts();
    if (!this._planError && this._plan !== undefined && pendingAsserts) {
        this._planError = true;
        this.fail('plan != count', {
            expected : this._plan,
            actual : this.assertCount
        });
    }
    this.ended = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.Test.prototype._exit"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_exit ()](#apidoc.element.tape.Test.prototype._exit)
- description and source-code
```javascript
_exit = function () {
    if (this._plan !== undefined &&
        !this._planError && this.assertCount !== this._plan) {
        this._planError = true;
        this.fail('plan != count', {
            expected : this._plan,
            actual : this.assertCount,
            exiting : true
        });
    }
    else if (!this.ended) {
        this.fail('test exited without ending', {
            exiting: true
        });
    }
}
```
- example usage
```shell
...
    }

    if (!ended) {
        var only = harness._results._only;
        for (var i = 0; i < harness._tests.length; i++) {
            var t = harness._tests[i];
            if (only && t !== only) continue;
            t._exit();
        }
    }
    harness.close();
    process.exit(code || harness._exitCode);
});

return harness;
...
```

#### <a name="apidoc.element.tape.Test.prototype._pendingAsserts"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>_pendingAsserts ()](#apidoc.element.tape.Test.prototype._pendingAsserts)
- description and source-code
```javascript
_pendingAsserts = function () {
    if (this._plan === undefined) {
        return 1;
    }
    else {
        return this._plan - (this._progeny.length + this.assertCount);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.Test.prototype.assert"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>assert (value, msg, extra)](#apidoc.element.tape.Test.prototype.assert)
- description and source-code
```javascript
assert = function (value, msg, extra) {
    this._assert(value, {
        message : defined(msg, 'should be truthy'),
        operator : 'ok',
        expected : true,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
...

Generate an assertion that will be skipped over.

## t.ok(value, msg)

Assert that 'value' is truthy with an optional description of the assertion 'msg'.

Aliases: 't.true()', 't.assert()'

## t.notOk(value, msg)

Assert that 'value' is falsy with an optional description of the assertion 'msg'.

Aliases: 't.false()', 't.notok()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.comment"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>comment (msg)](#apidoc.element.tape.Test.prototype.comment)
- description and source-code
```javascript
comment = function (msg) {
    var that = this;
    forEach(trim(msg).split('\n'), function (aMsg) {
        that.emit('result', trim(aMsg).replace(/^#\s*/, ''));
    });
}
```
- example usage
```shell
...

Create a subtest with a new test handle 'st' from 'cb(st)' inside the current
test 't'. 'cb(st)' will only fire when 't' finishes. Additional tests queued up
after 't' will not be run until all subtests finish.

You may pass the same options that ['test()'](#testname-opts-cb) accepts.

## t.comment(message)

Print a message without breaking the tap output. (Useful when using e.g. 'tap-colorize' where output is buffered & 'console.log'
will print in incorrect order vis-a-vis tap output.)

## var htest = test.createHarness()

Create a new test harness instance, which is a function like 'test()', but with
a new pending stack and test state.
...
```

#### <a name="apidoc.element.tape.Test.prototype.deepEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>deepEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.deepEqual)
- description and source-code
```javascript
deepEqual = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.deepEquals()', 't.isEquivalent()', 't.same()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.deepEquals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>deepEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.deepEquals)
- description and source-code
```javascript
deepEquals = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.deepEquals()', 't.isEquivalent()', 't.same()'

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.deepLooseEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>deepLooseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.deepLooseEqual)
- description and source-code
```javascript
deepLooseEqual = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.looseEqual()', 't.looseEquals()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.doesNotEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>doesNotEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.doesNotEqual)
- description and source-code
```javascript
doesNotEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.doesNotThrow"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>doesNotThrow (fn, expected, msg, extra)](#apidoc.element.tape.Test.prototype.doesNotThrow)
- description and source-code
```javascript
doesNotThrow = function (fn, expected, msg, extra) {
    if (typeof expected === 'string') {
        msg = expected;
        expected = undefined;
    }
    var caught = undefined;
    try {
        fn();
    }
    catch (err) {
        caught = { error : err };
    }
    this._assert(!caught, {
        message : defined(msg, 'should not throw'),
        operator : 'throws',
        actual : caught && caught.error,
        expected : expected,
        error : caught && caught.error,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.notLooseEqual()', 't.notLooseEquals()'

## t.throws(fn, expected, msg)

Assert that the function call 'fn()' throws an exception. 'expected', if present, must be a 'RegExp' or 'Function'. The 'RegExp'
matches the string representation of the exception, as generated by 'err.toString()'. The 'Function' is the exception thrown (e.
g. 'Error'). 'msg' is an optional description of the assertion.

## t.doesNotThrow(fn, expected, msg)

Assert that the function call 'fn()' does not throw an exception. 'msg' is an optional description of the assertion.

## t.test(name, [opts], cb)

Create a subtest with a new test handle 'st' from 'cb(st)' inside the current
test 't'. 'cb(st)' will only fire when 't' finishes. Additional tests queued up
...
```

#### <a name="apidoc.element.tape.Test.prototype.end"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>end (err)](#apidoc.element.tape.Test.prototype.end)
- description and source-code
```javascript
end = function (err) {
    var self = this;
    if (arguments.length >= 1 && !!err) {
        this.ifError(err);
    }

    if (this.calledEnd) {
        this.fail('.end() called twice');
    }
    this.calledEnd = true;
    this._end();
}
```
- example usage
```shell
...
- opts.skip = true/false. See test.skip.
- opts.timeout = 500. Set a timeout for the test, after which it will fail.
  See test.timeoutAfter.
- opts.objectPrintDepth = 5. Configure max depth of expected / actual object
  printing.

If you forget to 't.plan()' out how many assertions you are going to run and you
don't call 't.end()' explicitly, your test will hang.

## test.skip(name, cb)

Generate a new test that will be skipped over.

## test.onFinish(fn)
...
```

#### <a name="apidoc.element.tape.Test.prototype.equal"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>equal (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.equal)
- description and source-code
```javascript
equal = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

''' js
var test = require('tape');

test('timing test', function (t) {
    t.plan(2);

    t.equal(typeof Date.now, 'function');
    var start = Date.now();

    setTimeout(function () {
        t.equal(Date.now() - start, 100);
    }, 100);
});
'''
...
```

#### <a name="apidoc.element.tape.Test.prototype.equals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>equals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.equals)
- description and source-code
```javascript
equals = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
...
```

#### <a name="apidoc.element.tape.Test.prototype.error"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>error (err, msg, extra)](#apidoc.element.tape.Test.prototype.error)
- description and source-code
```javascript
error = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.notOk(value, msg)

Assert that 'value' is falsy with an optional description of the assertion 'msg'.

Aliases: 't.false()', 't.notok()'

## t.error(err, msg)

Assert that 'err' is falsy. If 'err' is non-falsy, use its 'err.message' as the
description message.

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)
...
```

#### <a name="apidoc.element.tape.Test.prototype.fail"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>fail (msg, extra)](#apidoc.element.tape.Test.prototype.fail)
- description and source-code
```javascript
fail = function (msg, extra) {
    this._assert(false, {
        message : msg,
        operator : 'fail',
        extra : extra
    });
}
```
- example usage
```shell
...
the 'n'th, or after 't.end()' is called, they will generate errors.

## t.end(err)

Declare the end of a test explicitly. If 'err' is passed in 't.end' will assert
that it is falsey.

## t.fail(msg)

Generate a failing assertion with a message 'msg'.

## t.pass(msg)

Generate a passing assertion with a message 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.false"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>false (value, msg, extra)](#apidoc.element.tape.Test.prototype.false)
- description and source-code
```javascript
false = function (value, msg, extra) {
    this._assert(!value, {
        message : defined(msg, 'should be falsy'),
        operator : 'notOk',
        expected : false,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.true()', 't.assert()'

## t.notOk(value, msg)

Assert that 'value' is falsy with an optional description of the assertion 'msg'.

Aliases: 't.false()', 't.notok()'

## t.error(err, msg)

Assert that 'err' is falsy. If 'err' is non-falsy, use its 'err.message' as the
description message.

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.ifErr"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>ifErr (err, msg, extra)](#apidoc.element.tape.Test.prototype.ifErr)
- description and source-code
```javascript
ifErr = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.false()', 't.notok()'

## t.error(err, msg)

Assert that 'err' is falsy. If 'err' is non-falsy, use its 'err.message' as the
description message.

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.ifError"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>ifError (err, msg, extra)](#apidoc.element.tape.Test.prototype.ifError)
- description and source-code
```javascript
ifError = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.false()', 't.notok()'

## t.error(err, msg)

Assert that 'err' is falsy. If 'err' is non-falsy, use its 'err.message' as the
description message.

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.iferror"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>iferror (err, msg, extra)](#apidoc.element.tape.Test.prototype.iferror)
- description and source-code
```javascript
iferror = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.false()', 't.notok()'

## t.error(err, msg)

Assert that 'err' is falsy. If 'err' is non-falsy, use its 'err.message' as the
description message.

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.is"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>is (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.is)
- description and source-code
```javascript
is = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
...
```

#### <a name="apidoc.element.tape.Test.prototype.isEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isEqual)
- description and source-code
```javascript
isEqual = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
...
```

#### <a name="apidoc.element.tape.Test.prototype.isEquivalent"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isEquivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isEquivalent)
- description and source-code
```javascript
isEquivalent = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.deepEquals()', 't.isEquivalent()', 't.same()'

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isInequal"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isInequal (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isInequal)
- description and source-code
```javascript
isInequal = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isInequivalent"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isInequivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isInequivalent)
- description and source-code
```javascript
isInequivalent = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isNot"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNot (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNot)
- description and source-code
```javascript
isNot = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isNotDeepEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotDeepEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotDeepEqual)
- description and source-code
```javascript
isNotDeepEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isNotDeeply"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotDeeply (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotDeeply)
- description and source-code
```javascript
isNotDeeply = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isNotEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotEqual)
- description and source-code
```javascript
isNotEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.isNotEquivalent"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>isNotEquivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.isNotEquivalent)
- description and source-code
```javascript
isNotEquivalent = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.looseEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>looseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.looseEqual)
- description and source-code
```javascript
looseEqual = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.looseEqual()', 't.looseEquals()'

## t.notDeepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.looseEquals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>looseEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.looseEquals)
- description and source-code
```javascript
looseEquals = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.looseEqual()', 't.looseEquals()'

## t.notDeepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.not"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>not (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.not)
- description and source-code
```javascript
not = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.notDeepEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notDeepEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notDeepEqual)
- description and source-code
```javascript
notDeepEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.deepEquals()', 't.isEquivalent()', 't.same()'

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
...
```

#### <a name="apidoc.element.tape.Test.prototype.notDeepLooseEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notDeepLooseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notDeepLooseEqual)
- description and source-code
```javascript
notDeepLooseEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'notDeepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.looseEqual()', 't.looseEquals()'

## t.notDeepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notLooseEqual()', 't.notLooseEquals()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.notDeeply"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notDeeply (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notDeeply)
- description and source-code
```javascript
notDeeply = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notEqual)
- description and source-code
```javascript
notEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notEquals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notEquals)
- description and source-code
```javascript
notEquals = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.notEquivalent"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notEquivalent (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notEquivalent)
- description and source-code
```javascript
notEquivalent = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notLooseEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notLooseEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notLooseEqual)
- description and source-code
```javascript
notLooseEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'notDeepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.notDeepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notLooseEqual()', 't.notLooseEquals()'

## t.throws(fn, expected, msg)

Assert that the function call 'fn()' throws an exception. 'expected', if present, must be a 'RegExp' or 'Function'. The 'RegExp'
matches the string representation of the exception, as generated by 'err.toString()'. The 'Function' is the exception thrown (e.
g. 'Error'). 'msg' is an optional description of the assertion.

## t.doesNotThrow(fn, expected, msg)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notLooseEquals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notLooseEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notLooseEquals)
- description and source-code
```javascript
notLooseEquals = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'notDeepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.notDeepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notLooseEqual()', 't.notLooseEquals()'

## t.throws(fn, expected, msg)

Assert that the function call 'fn()' throws an exception. 'expected', if present, must be a 'RegExp' or 'Function'. The 'RegExp'
matches the string representation of the exception, as generated by 'err.toString()'. The 'Function' is the exception thrown (e.
g. 'Error'). 'msg' is an optional description of the assertion.

## t.doesNotThrow(fn, expected, msg)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notOk"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notOk (value, msg, extra)](#apidoc.element.tape.Test.prototype.notOk)
- description and source-code
```javascript
notOk = function (value, msg, extra) {
    this._assert(!value, {
        message : defined(msg, 'should be falsy'),
        operator : 'notOk',
        expected : false,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.ok(value, msg)

Assert that 'value' is truthy with an optional description of the assertion 'msg'.

Aliases: 't.true()', 't.assert()'

## t.notOk(value, msg)

Assert that 'value' is falsy with an optional description of the assertion 'msg'.

Aliases: 't.false()', 't.notok()'

## t.error(err, msg)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notSame"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notSame (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notSame)
- description and source-code
```javascript
notSame = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notEquivalent()', 't.notDeeply()', 't.notSame()',
't.isNotDeepEqual()', 't.isNotDeeply()', 't.isNotEquivalent()',
't.isInequivalent()'

## t.deepLooseEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
...
```

#### <a name="apidoc.element.tape.Test.prototype.notStrictEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notStrictEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notStrictEqual)
- description and source-code
```javascript
notStrictEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.notStrictEquals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notStrictEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.notStrictEquals)
- description and source-code
```javascript
notStrictEquals = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.notok"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>notok (value, msg, extra)](#apidoc.element.tape.Test.prototype.notok)
- description and source-code
```javascript
notok = function (value, msg, extra) {
    this._assert(!value, {
        message : defined(msg, 'should be falsy'),
        operator : 'notOk',
        expected : false,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.true()', 't.assert()'

## t.notOk(value, msg)

Assert that 'value' is falsy with an optional description of the assertion 'msg'.

Aliases: 't.false()', 't.notok()'

## t.error(err, msg)

Assert that 'err' is falsy. If 'err' is non-falsy, use its 'err.message' as the
description message.

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.ok"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>ok (value, msg, extra)](#apidoc.element.tape.Test.prototype.ok)
- description and source-code
```javascript
ok = function (value, msg, extra) {
    this._assert(value, {
        message : defined(msg, 'should be truthy'),
        operator : 'ok',
        expected : true,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
...

Automatically timeout the test after X ms.

## t.skip(msg)

Generate an assertion that will be skipped over.

## t.ok(value, msg)

Assert that 'value' is truthy with an optional description of the assertion 'msg'.

Aliases: 't.true()', 't.assert()'

## t.notOk(value, msg)
...
```

#### <a name="apidoc.element.tape.Test.prototype.pass"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>pass (msg, extra)](#apidoc.element.tape.Test.prototype.pass)
- description and source-code
```javascript
pass = function (msg, extra) {
    this._assert(true, {
        message : msg,
        operator : 'pass',
        extra : extra
    });
}
```
- example usage
```shell
...
Declare the end of a test explicitly. If 'err' is passed in 't.end' will assert
that it is falsey.

## t.fail(msg)

Generate a failing assertion with a message 'msg'.

## t.pass(msg)

Generate a passing assertion with a message 'msg'.

## t.timeoutAfter(ms)

Automatically timeout the test after X ms.
...
```

#### <a name="apidoc.element.tape.Test.prototype.plan"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>plan (n)](#apidoc.element.tape.Test.prototype.plan)
- description and source-code
```javascript
plan = function (n) {
    this._plan = n;
    this.emit('plan', n);
}
```
- example usage
```shell
...

# example

''' js
var test = require('tape');

test('timing test', function (t) {
t.plan(2);

t.equal(typeof Date.now, 'function');
var start = Date.now();

setTimeout(function () {
    t.equal(Date.now() - start, 100);
}, 100);
...
```

#### <a name="apidoc.element.tape.Test.prototype.run"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>run ()](#apidoc.element.tape.Test.prototype.run)
- description and source-code
```javascript
run = function () {
    if (this._skip) {
        this.comment('SKIP ' + this.name);
    }
    if (!this._cb || this._skip) {
        return this._end();
    }
    if (this._timeout != null) {
        this.timeoutAfter(this._timeout);
    }
    this.emit('prerun');
    this._cb(this);
    this.emit('run');
}
```
- example usage
```shell
...
        output.queue('TAP version 13\n');
        self._stream.pipe(output);
    }

    nextTick(function next() {
        var t;
        while (t = getNextTest(self)) {
            t.run();
            if (!t.ended) return t.once('end', function(){ nextTick(next); });
        }
        self.emit('done');
    });

    return output;
};
...
```

#### <a name="apidoc.element.tape.Test.prototype.same"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>same (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.same)
- description and source-code
```javascript
same = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

## t.deepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.deepEquals()', 't.isEquivalent()', 't.same()'

## t.notDeepEqual(actual, expected, msg)

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with strict comparisons ('===') on leaf nodes and an optional description of the assertion 'msg'.
...
```

#### <a name="apidoc.element.tape.Test.prototype.skip"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>skip (msg, extra)](#apidoc.element.tape.Test.prototype.skip)
- description and source-code
```javascript
skip = function (msg, extra) {
    this._assert(true, {
        message : msg,
        operator : 'skip',
        skip : true,
        extra : extra
    });
}
```
- example usage
```shell
...
  See test.timeoutAfter.
- opts.objectPrintDepth = 5. Configure max depth of expected / actual object
  printing.

If you forget to 't.plan()' out how many assertions you are going to run and you
don't call 't.end()' explicitly, your test will hang.

## test.skip(name, cb)

Generate a new test that will be skipped over.

## test.onFinish(fn)

The onFinish hook will get invoked when ALL tape tests have finished
right before tape is about to print the test summary.
...
```

#### <a name="apidoc.element.tape.Test.prototype.strictEqual"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>strictEqual (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.strictEqual)
- description and source-code
```javascript
strictEqual = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...

Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
...
```

#### <a name="apidoc.element.tape.Test.prototype.strictEquals"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>strictEquals (a, b, msg, extra)](#apidoc.element.tape.Test.prototype.strictEquals)
- description and source-code
```javascript
strictEquals = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
...
Aliases: 't.ifError()', 't.ifErr()', 't.iferror()'

## t.equal(actual, expected, msg)

Assert that 'actual === expected' with an optional description of the assertion 'msg'.

Aliases: 't.equals()', 't.isEqual()', 't.is()', 't.strictEqual()',
't.strictEquals()'

## t.notEqual(actual, expected, msg)

Assert that 'actual !== expected' with an optional description of the assertion 'msg'.

Aliases: 't.notEquals()', 't.notStrictEqual()', 't.notStrictEquals()',
't.isNotEqual()', 't.isNot()', 't.not()', 't.doesNotEqual()', 't.isInequal()'
...
```

#### <a name="apidoc.element.tape.Test.prototype.test"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>test (name, opts, cb)](#apidoc.element.tape.Test.prototype.test)
- description and source-code
```javascript
test = function (name, opts, cb) {
    var self = this;
    var t = new Test(name, opts, cb);
    this._progeny.push(t);
    this.pendingCount++;
    this.emit('test', t);
    t.on('prerun', function () {
        self.assertCount++;
    })

    if (!self._pendingAsserts()) {
        nextTick(function () {
            self._end();
        });
    }

    nextTick(function() {
        if (!self._plan && self.pendingCount == self._progeny.length) {
            self._end();
        }
    });
}
```
- example usage
```shell
...

Assert that the function call 'fn()' throws an exception. 'expected', if present, must be a 'RegExp' or 'Function'. The 'RegExp'
matches the string representation of the exception, as generated by 'err.toString()'. The 'Function' is the exception thrown (e.
g. 'Error'). 'msg' is an optional description of the assertion.

## t.doesNotThrow(fn, expected, msg)

Assert that the function call 'fn()' does not throw an exception. 'msg' is an optional description of the assertion.

## t.test(name, [opts], cb)

Create a subtest with a new test handle 'st' from 'cb(st)' inside the current
test 't'. 'cb(st)' will only fire when 't' finishes. Additional tests queued up
after 't' will not be run until all subtests finish.

You may pass the same options that ['test()'](#testname-opts-cb) accepts.
...
```

#### <a name="apidoc.element.tape.Test.prototype.throws"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>throws (fn, expected, msg, extra)](#apidoc.element.tape.Test.prototype.throws)
- description and source-code
```javascript
throws = function (fn, expected, msg, extra) {
    if (typeof expected === 'string') {
        msg = expected;
        expected = undefined;
    }

    var caught = undefined;

    try {
        fn();
    } catch (err) {
        caught = { error : err };
        if ((err != null) && (!isEnumerable(err, 'message') || !has(err, 'message'))) {
            var message = err.message;
            delete err.message;
            err.message = message;
        }
    }

    var passed = caught;

    if (expected instanceof RegExp) {
        passed = expected.test(caught && caught.error);
        expected = String(expected);
    }

    if (typeof expected === 'function' && caught) {
        passed = caught.error instanceof expected;
        caught.error = caught.error.constructor;
    }

    this._assert(typeof fn === 'function' && passed, {
        message : defined(msg, 'should throw'),
        operator : 'throws',
        actual : caught && caught.error,
        expected : expected,
        error: !passed && caught && caught.error,
        extra : extra
    });
}
```
- example usage
```shell
...

Assert that 'actual' and 'expected' do not have the same structure and nested values using
[node's deepEqual() algorithm](https://github.com/substack/node-deep-equal)
with loose comparisons ('==') on leaf nodes and an optional description of the assertion 'msg'.

Aliases: 't.notLooseEqual()', 't.notLooseEquals()'

## t.throws(fn, expected, msg)

Assert that the function call 'fn()' throws an exception. 'expected', if present, must be a 'RegExp' or 'Function'. The 'RegExp'
matches the string representation of the exception, as generated by 'err.toString()'. The 'Function' is the exception thrown (e.
g. 'Error'). 'msg' is an optional description of the assertion.

## t.doesNotThrow(fn, expected, msg)

Assert that the function call 'fn()' does not throw an exception. 'msg' is an optional description of the assertion.
...
```

#### <a name="apidoc.element.tape.Test.prototype.timeoutAfter"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>timeoutAfter (ms)](#apidoc.element.tape.Test.prototype.timeoutAfter)
- description and source-code
```javascript
timeoutAfter = function (ms) {
    if (!ms) throw new Error('timeoutAfter requires a timespan');
    var self = this;
    var timeout = safeSetTimeout(function() {
        self.fail('test timed out after ' + ms + 'ms');
        self.end();
    }, ms);
    this.once('end', function() {
        clearTimeout(timeout);
    });
}
```
- example usage
```shell
...

Generate a failing assertion with a message 'msg'.

## t.pass(msg)

Generate a passing assertion with a message 'msg'.

## t.timeoutAfter(ms)

Automatically timeout the test after X ms.

## t.skip(msg)

Generate an assertion that will be skipped over.
...
```

#### <a name="apidoc.element.tape.Test.prototype.true"></a>[function <span class="apidocSignatureSpan">tape.Test.prototype.</span>true (value, msg, extra)](#apidoc.element.tape.Test.prototype.true)
- description and source-code
```javascript
true = function (value, msg, extra) {
    this._assert(value, {
        message : defined(msg, 'should be truthy'),
        operator : 'ok',
        expected : true,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
...

Generate an assertion that will be skipped over.

## t.ok(value, msg)

Assert that 'value' is truthy with an optional description of the assertion 'msg'.

Aliases: 't.true()', 't.assert()'

## t.notOk(value, msg)

Assert that 'value' is falsy with an optional description of the assertion 'msg'.

Aliases: 't.false()', 't.notok()'
...
```



# <a name="apidoc.module.tape.results"></a>[module tape.results](#apidoc.module.tape.results)

#### <a name="apidoc.element.tape.results.results"></a>[function <span class="apidocSignatureSpan">tape.</span>results ()](#apidoc.element.tape.results.results)
- description and source-code
```javascript
function Results() {
    if (!(this instanceof Results)) return new Results;
    this.count = 0;
    this.fail = 0;
    this.pass = 0;
    this._stream = through();
    this.tests = [];
    this._only = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tape.results.super_"></a>[function <span class="apidocSignatureSpan">tape.results.</span>super_ ()](#apidoc.element.tape.results.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tape.results.prototype"></a>[module tape.results.prototype](#apidoc.module.tape.results.prototype)

#### <a name="apidoc.element.tape.results.prototype._watch"></a>[function <span class="apidocSignatureSpan">tape.results.prototype.</span>_watch (t)](#apidoc.element.tape.results.prototype._watch)
- description and source-code
```javascript
_watch = function (t) {
    var self = this;
    var write = function (s) { self._stream.queue(s) };
    t.once('prerun', function () {
        write('# ' + t.name + '\n');
    });

    t.on('result', function (res) {
        if (typeof res === 'string') {
            write('# ' + res + '\n');
            return;
        }
        write(encodeResult(res, self.count + 1));
        self.count ++;

        if (res.ok) self.pass ++
        else self.fail ++
    });

    t.on('test', function (st) { self._watch(st) });
}
```
- example usage
```shell
...

    return output;
};

Results.prototype.push = function (t) {
    var self = this;
    self.tests.push(t);
    self._watch(t);
    self.emit('_push', t);
};

Results.prototype.only = function (t) {
    this._only = t;
};
...
```

#### <a name="apidoc.element.tape.results.prototype.close"></a>[function <span class="apidocSignatureSpan">tape.results.prototype.</span>close ()](#apidoc.element.tape.results.prototype.close)
- description and source-code
```javascript
close = function () {
    var self = this;
    if (self.closed) self._stream.emit('error', new Error('ALREADY CLOSED'));
    self.closed = true;
    var write = function (s) { self._stream.queue(s) };

    write('\n1..' + self.count + '\n');
    write('# tests ' + self.count + '\n');
    write('# pass  ' + self.pass + '\n');
    if (self.fail) write('# fail  ' + self.fail + '\n')
    else write('\n# ok\n')

    self._stream.queue(null);
}
```
- example usage
```shell
...
            var only = harness._results._only;
            for (var i = 0; i < harness._tests.length; i++) {
                var t = harness._tests[i];
                if (only && t !== only) continue;
                t._exit();
            }
        }
        harness.close();
        process.exit(code || harness._exitCode);
    });

    return harness;
}

exports.createHarness = createHarness;
...
```

#### <a name="apidoc.element.tape.results.prototype.createStream"></a>[function <span class="apidocSignatureSpan">tape.results.prototype.</span>createStream (opts)](#apidoc.element.tape.results.prototype.createStream)
- description and source-code
```javascript
createStream = function (opts) {
    if (!opts) opts = {};
    var self = this;
    var output, testId = 0;
    if (opts.objectMode) {
        output = through();
        self.on('_push', function ontest (t, extra) {
            if (!extra) extra = {};
            var id = testId++;
            t.once('prerun', function () {
                var row = {
                    type: 'test',
                    name: t.name,
                    id: id
                };
                if (has(extra, 'parent')) {
                    row.parent = extra.parent;
                }
                output.queue(row);
            });
            t.on('test', function (st) {
                ontest(st, { parent: id });
            });
            t.on('result', function (res) {
                res.test = id;
                res.type = 'assert';
                output.queue(res);
            });
            t.on('end', function () {
                output.queue({ type: 'end', test: id });
            });
        });
        self.on('done', function () { output.queue(null) });
    }
    else {
        output = resumer();
        output.queue('TAP version 13\n');
        self._stream.pipe(output);
    }

    nextTick(function next() {
        var t;
        while (t = getNextTest(self)) {
            t.run();
            if (!t.ended) return t.once('end', function(){ nextTick(next); });
        }
        self.emit('done');
    });

    return output;
}
```
- example usage
```shell
...
lazyLoad.createStream = function (opts) {
    if (!opts) opts = {};
    if (!harness) {
        var output = through();
        getHarness({ stream: output, objectMode: opts.objectMode });
        return output;
    }
    return harness.createStream(opts);
};

lazyLoad.onFinish = function () {
    return getHarness().onFinish.apply(this, arguments);
};

lazyLoad.getHarness = getHarness
...
```

#### <a name="apidoc.element.tape.results.prototype.only"></a>[function <span class="apidocSignatureSpan">tape.results.prototype.</span>only (t)](#apidoc.element.tape.results.prototype.only)
- description and source-code
```javascript
only = function (t) {
    this._only = t;
}
```
- example usage
```shell
...
};

var only = false;
test.only = function () {
    if (only) throw new Error('there can only be one only test');
    only = true;
    var t = test.apply(null, arguments);
    results.only(t);
    return t;
};
test._exitCode = 0;

test.close = function () { results.close() };

return test;
...
```

#### <a name="apidoc.element.tape.results.prototype.push"></a>[function <span class="apidocSignatureSpan">tape.results.prototype.</span>push (t)](#apidoc.element.tape.results.prototype.push)
- description and source-code
```javascript
push = function (t) {
    var self = this;
    self.tests.push(t);
    self._watch(t);
    self.emit('_push', t);
}
```
- example usage
```shell
...
var results = createResult();
if (conf_.autoclose !== false) {
    results.once('done', function () { results.close() });
}

var test = function (name, conf, cb) {
    var t = new Test(name, conf, cb);
    test._tests.push(t);

    (function inspectCode (st) {
        st.on('test', function sub (st_) {
            inspectCode(st_);
        });
        st.on('result', function (r) {
            if (!r.ok && typeof r !== 'string') test._exitCode = 1
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
