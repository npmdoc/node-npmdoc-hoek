# api documentation for  [hoek (v4.1.1)](https://github.com/hapijs/hoek#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-hoek.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-hoek) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-hoek.svg)](https://travis-ci.org/npmdoc/node-npmdoc-hoek)
#### General purpose node utilities

[![NPM](https://nodei.co/npm/hoek.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/hoek)

[![apidoc](https://npmdoc.github.io/node-npmdoc-hoek/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-hoek/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-hoek/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-hoek/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/hapijs/hoek/issues"
    },
    "dependencies": {},
    "description": "General purpose node utilities",
    "devDependencies": {
        "code": "4.x.x",
        "lab": "13.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "9cc573ffba2b7b408fb5e9c2a13796be94cddce9",
        "tarball": "https://registry.npmjs.org/hoek/-/hoek-4.1.1.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "6319080cdf8c23b5c3f4e8896b3de1a96f649da7",
    "homepage": "https://github.com/hapijs/hoek#readme",
    "keywords": [
        "utilities"
    ],
    "license": "BSD-3-Clause",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "hueniverse"
        },
        {
            "name": "marsup"
        },
        {
            "name": "nlf"
        },
        {
            "name": "wyatt"
        }
    ],
    "name": "hoek",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/hapijs/hoek.git"
    },
    "scripts": {
        "test": "lab -a code -t 100 -L",
        "test-cov-html": "lab -a code -t 100 -L -r html -o coverage.html"
    },
    "version": "4.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module hoek](#apidoc.module.hoek)
1.  boolean <span class="apidocSignatureSpan">hoek.</span>abortThrow
1.  [function <span class="apidocSignatureSpan">hoek.</span>Bench ()](#apidoc.element.hoek.Bench)
1.  [function <span class="apidocSignatureSpan">hoek.</span>Timer ()](#apidoc.element.hoek.Timer)
1.  [function <span class="apidocSignatureSpan">hoek.</span>abort (message, hideStack)](#apidoc.element.hoek.abort)
1.  [function <span class="apidocSignatureSpan">hoek.</span>applyToDefaults (defaults, options, isNullOverride)](#apidoc.element.hoek.applyToDefaults)
1.  [function <span class="apidocSignatureSpan">hoek.</span>applyToDefaultsWithShallow (defaults, options, keys)](#apidoc.element.hoek.applyToDefaultsWithShallow)
1.  [function <span class="apidocSignatureSpan">hoek.</span>assert (condition)](#apidoc.element.hoek.assert)
1.  [function <span class="apidocSignatureSpan">hoek.</span>base64urlDecode (value, encoding)](#apidoc.element.hoek.base64urlDecode)
1.  [function <span class="apidocSignatureSpan">hoek.</span>base64urlEncode (value, encoding)](#apidoc.element.hoek.base64urlEncode)
1.  [function <span class="apidocSignatureSpan">hoek.</span>callStack (slice)](#apidoc.element.hoek.callStack)
1.  [function <span class="apidocSignatureSpan">hoek.</span>clone (obj, seen)](#apidoc.element.hoek.clone)
1.  [function <span class="apidocSignatureSpan">hoek.</span>cloneWithShallow (source, keys)](#apidoc.element.hoek.cloneWithShallow)
1.  [function <span class="apidocSignatureSpan">hoek.</span>contain (ref, values, options)](#apidoc.element.hoek.contain)
1.  [function <span class="apidocSignatureSpan">hoek.</span>deepEqual (obj, ref, options, seen)](#apidoc.element.hoek.deepEqual)
1.  [function <span class="apidocSignatureSpan">hoek.</span>displayStack (slice)](#apidoc.element.hoek.displayStack)
1.  [function <span class="apidocSignatureSpan">hoek.</span>escapeHeaderAttribute (attribute)](#apidoc.element.hoek.escapeHeaderAttribute)
1.  [function <span class="apidocSignatureSpan">hoek.</span>escapeHtml (string)](#apidoc.element.hoek.escapeHtml)
1.  [function <span class="apidocSignatureSpan">hoek.</span>escapeJavaScript (string)](#apidoc.element.hoek.escapeJavaScript)
1.  [function <span class="apidocSignatureSpan">hoek.</span>escapeRegex (string)](#apidoc.element.hoek.escapeRegex)
1.  [function <span class="apidocSignatureSpan">hoek.</span>flatten (array, target)](#apidoc.element.hoek.flatten)
1.  [function <span class="apidocSignatureSpan">hoek.</span>format (f)](#apidoc.element.hoek.format)
1.  [function <span class="apidocSignatureSpan">hoek.</span>formatStack (stack)](#apidoc.element.hoek.formatStack)
1.  [function <span class="apidocSignatureSpan">hoek.</span>formatTrace (trace)](#apidoc.element.hoek.formatTrace)
1.  [function <span class="apidocSignatureSpan">hoek.</span>ignore ()](#apidoc.element.hoek.ignore)
1.  [function <span class="apidocSignatureSpan">hoek.</span>inherits (ctor, superCtor)](#apidoc.element.hoek.inherits)
1.  [function <span class="apidocSignatureSpan">hoek.</span>intersect (array1, array2, justFirst)](#apidoc.element.hoek.intersect)
1.  [function <span class="apidocSignatureSpan">hoek.</span>isInteger ()](#apidoc.element.hoek.isInteger)
1.  [function <span class="apidocSignatureSpan">hoek.</span>mapToObject (array, key)](#apidoc.element.hoek.mapToObject)
1.  [function <span class="apidocSignatureSpan">hoek.</span>merge (target, source, isNullOverride, isMergeArrays)](#apidoc.element.hoek.merge)
1.  [function <span class="apidocSignatureSpan">hoek.</span>nextTick (callback)](#apidoc.element.hoek.nextTick)
1.  [function <span class="apidocSignatureSpan">hoek.</span>once (method)](#apidoc.element.hoek.once)
1.  [function <span class="apidocSignatureSpan">hoek.</span>reach (obj, chain, options)](#apidoc.element.hoek.reach)
1.  [function <span class="apidocSignatureSpan">hoek.</span>reachTemplate (obj, template, options)](#apidoc.element.hoek.reachTemplate)
1.  [function <span class="apidocSignatureSpan">hoek.</span>shallow (source)](#apidoc.element.hoek.shallow)
1.  [function <span class="apidocSignatureSpan">hoek.</span>stringify ()](#apidoc.element.hoek.stringify)
1.  [function <span class="apidocSignatureSpan">hoek.</span>transform (source, transform, options)](#apidoc.element.hoek.transform)
1.  [function <span class="apidocSignatureSpan">hoek.</span>unique (array, key)](#apidoc.element.hoek.unique)
1.  [function <span class="apidocSignatureSpan">hoek.</span>uniqueFilename (path, extension)](#apidoc.element.hoek.uniqueFilename)
1.  object <span class="apidocSignatureSpan">hoek.</span>Bench.prototype
1.  object <span class="apidocSignatureSpan">hoek.</span>Timer.prototype

#### [module hoek.Bench](#apidoc.module.hoek.Bench)
1.  [function <span class="apidocSignatureSpan">hoek.</span>Bench ()](#apidoc.element.hoek.Bench.Bench)
1.  [function <span class="apidocSignatureSpan">hoek.Bench.</span>now ()](#apidoc.element.hoek.Bench.now)

#### [module hoek.Bench.prototype](#apidoc.module.hoek.Bench.prototype)
1.  [function <span class="apidocSignatureSpan">hoek.Bench.prototype.</span>elapsed ()](#apidoc.element.hoek.Bench.prototype.elapsed)
1.  [function <span class="apidocSignatureSpan">hoek.Bench.prototype.</span>reset ()](#apidoc.element.hoek.Bench.prototype.reset)

#### [module hoek.Timer](#apidoc.module.hoek.Timer)
1.  [function <span class="apidocSignatureSpan">hoek.</span>Timer ()](#apidoc.element.hoek.Timer.Timer)

#### [module hoek.Timer.prototype](#apidoc.module.hoek.Timer.prototype)
1.  [function <span class="apidocSignatureSpan">hoek.Timer.prototype.</span>elapsed ()](#apidoc.element.hoek.Timer.prototype.elapsed)
1.  [function <span class="apidocSignatureSpan">hoek.Timer.prototype.</span>reset ()](#apidoc.element.hoek.Timer.prototype.reset)



# <a name="apidoc.module.hoek"></a>[module hoek](#apidoc.module.hoek)

#### <a name="apidoc.element.hoek.Bench"></a>[function <span class="apidocSignatureSpan">hoek.</span>Bench ()](#apidoc.element.hoek.Bench)
- description and source-code
```javascript
Bench = function () {

    this.ts = 0;
    this.reset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.Timer"></a>[function <span class="apidocSignatureSpan">hoek.</span>Timer ()](#apidoc.element.hoek.Timer)
- description and source-code
```javascript
Timer = function () {

    this.ts = 0;
    this.reset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.abort"></a>[function <span class="apidocSignatureSpan">hoek.</span>abort (message, hideStack)](#apidoc.element.hoek.abort)
- description and source-code
```javascript
abort = function (message, hideStack) {

    if (process.env.NODE_ENV === 'test' || exports.abortThrow === true) {
        throw new Error(message || 'Unknown error');
    }

    let stack = '';
    if (!hideStack) {
        stack = exports.displayStack(1).join('\n\t');
    }
    console.log('ABORT: ' + message + '\n\t' + stack);
    process.exit(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.applyToDefaults"></a>[function <span class="apidocSignatureSpan">hoek.</span>applyToDefaults (defaults, options, isNullOverride)](#apidoc.element.hoek.applyToDefaults)
- description and source-code
```javascript
applyToDefaults = function (defaults, options, isNullOverride) {

    exports.assert(defaults && typeof defaults === 'object', 'Invalid defaults value: must be an object');
    exports.assert(!options || options === true || typeof options === 'object', 'Invalid options value: must be true, falsy or an
 object');

    if (!options) {                                                 // If no options, return null
        return null;
    }

    const copy = exports.clone(defaults);

    if (options === true) {                                         // If options is set to true, use defaults
        return copy;
    }

    return exports.merge(copy, options, isNullOverride === true, false);
}
```
- example usage
```shell
...

For example, to use Hoek to set configuration with default options:
'''javascript
const Hoek = require('hoek');

const default = {url : "www.github.com", port : "8000", debug : true};

const config = Hoek.applyToDefaults(default, {port : "3000", admin : true});

// In this case, config would be { url: 'www.github.com', port: '3000', debug: true, admin: true }
'''

## Documentation

[**API Reference**](API.md)
...
```

#### <a name="apidoc.element.hoek.applyToDefaultsWithShallow"></a>[function <span class="apidocSignatureSpan">hoek.</span>applyToDefaultsWithShallow (defaults, options, keys)](#apidoc.element.hoek.applyToDefaultsWithShallow)
- description and source-code
```javascript
applyToDefaultsWithShallow = function (defaults, options, keys) {

    exports.assert(defaults && typeof defaults === 'object', 'Invalid defaults value: must be an object');
    exports.assert(!options || options === true || typeof options === 'object', 'Invalid options value: must be true, falsy or an
 object');
    exports.assert(keys && Array.isArray(keys), 'Invalid keys');

    if (!options) {                                                 // If no options, return null
        return null;
    }

    const copy = exports.cloneWithShallow(defaults, keys);

    if (options === true) {                                         // If options is set to true, use defaults
        return copy;
    }

    const storage = internals.store(options, keys);   // Move shallow copy items to storage
    exports.merge(copy, options, false, false);     // Deep copy the rest
    internals.restore(copy, options, storage);      // Shallow copy the stored items and restore
    return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.assert"></a>[function <span class="apidocSignatureSpan">hoek.</span>assert (condition)](#apidoc.element.hoek.assert)
- description and source-code
```javascript
assert = function (condition) {

    if (condition) {
        return;
    }

    if (arguments.length === 2 && arguments[1] instanceof Error) {
        throw arguments[1];
    }

    let msgs = [];
    for (let i = 1; i < arguments.length; ++i) {
        if (arguments[i] !== '') {
            msgs.push(arguments[i]);            // Avoids Array.slice arguments leak, allowing for V8 optimizations
        }
    }

    msgs = msgs.map((msg) => {

        return typeof msg === 'string' ? msg : msg instanceof Error ? msg.message : exports.stringify(msg);
    });

    throw new Error(msgs.join(' ') || 'Unknown error');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.base64urlDecode"></a>[function <span class="apidocSignatureSpan">hoek.</span>base64urlDecode (value, encoding)](#apidoc.element.hoek.base64urlDecode)
- description and source-code
```javascript
base64urlDecode = function (value, encoding) {

    if (typeof value !== 'string') {

        return new Error('Value not a string');
    }

    if (!/^[\w\-]*$/.test(value)) {

        return new Error('Invalid character');
    }

    const buf = new Buffer(value, 'base64');
    return (encoding === 'buffer' ? buf : buf.toString(encoding || 'binary'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.base64urlEncode"></a>[function <span class="apidocSignatureSpan">hoek.</span>base64urlEncode (value, encoding)](#apidoc.element.hoek.base64urlEncode)
- description and source-code
```javascript
base64urlEncode = function (value, encoding) {

    exports.assert(typeof value === 'string' || Buffer.isBuffer(value), 'value must be string or buffer');
    const buf = (Buffer.isBuffer(value) ? value : new Buffer(value, encoding || 'binary'));
    return buf.toString('base64').replace(/\+/g, '-').replace(/\//g, '_').replace(/\=/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.callStack"></a>[function <span class="apidocSignatureSpan">hoek.</span>callStack (slice)](#apidoc.element.hoek.callStack)
- description and source-code
```javascript
callStack = function (slice) {

    // http://code.google.com/p/v8/wiki/JavaScriptStackTraceApi

    const v8 = Error.prepareStackTrace;
    Error.prepareStackTrace = function (_, stack) {

        return stack;
    };

    const capture = {};
    Error.captureStackTrace(capture, this);     // arguments.callee is not supported in strict mode so we use this and slice the
 trace of this off the result
    const stack = capture.stack;

    Error.prepareStackTrace = v8;

    const trace = exports.formatStack(stack);

    return trace.slice(1 + slice);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.clone"></a>[function <span class="apidocSignatureSpan">hoek.</span>clone (obj, seen)](#apidoc.element.hoek.clone)
- description and source-code
```javascript
clone = function (obj, seen) {

    if (typeof obj !== 'object' ||
        obj === null) {

        return obj;
    }

    seen = seen || new Map();

    const lookup = seen.get(obj);
    if (lookup) {
        return lookup;
    }

    let newObj;
    let cloneDeep = false;

    if (!Array.isArray(obj)) {
        if (Buffer.isBuffer(obj)) {
            newObj = new Buffer(obj);
        }
        else if (obj instanceof Date) {
            newObj = new Date(obj.getTime());
        }
        else if (obj instanceof RegExp) {
            newObj = new RegExp(obj);
        }
        else {
            const proto = Object.getPrototypeOf(obj);
            if (proto &&
                proto.isImmutable) {

                newObj = obj;
            }
            else {
                newObj = Object.create(proto);
                cloneDeep = true;
            }
        }
    }
    else {
        newObj = [];
        cloneDeep = true;
    }

    seen.set(obj, newObj);

    if (cloneDeep) {
        const keys = Object.getOwnPropertyNames(obj);
        for (let i = 0; i < keys.length; ++i) {
            const key = keys[i];
            const descriptor = Object.getOwnPropertyDescriptor(obj, key);
            if (descriptor &&
                (descriptor.get ||
                 descriptor.set)) {

                Object.defineProperty(newObj, key, descriptor);
            }
            else {
                newObj[key] = exports.clone(obj[key], seen);
            }
        }
    }

    return newObj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.cloneWithShallow"></a>[function <span class="apidocSignatureSpan">hoek.</span>cloneWithShallow (source, keys)](#apidoc.element.hoek.cloneWithShallow)
- description and source-code
```javascript
cloneWithShallow = function (source, keys) {

    if (!source ||
        typeof source !== 'object') {

        return source;
    }

    const storage = internals.store(source, keys);    // Move shallow copy items to storage
    const copy = exports.clone(source);               // Deep copy the rest
    internals.restore(copy, source, storage);       // Shallow copy the stored items and restore
    return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.contain"></a>[function <span class="apidocSignatureSpan">hoek.</span>contain (ref, values, options)](#apidoc.element.hoek.contain)
- description and source-code
```javascript
contain = function (ref, values, options) {

<span class="apidocCodeCommentSpan">    /*
        string -> string(s)
        array -> item(s)
        object -> key(s)
        object -> object (key:value)
    */
</span>
    let valuePairs = null;
    if (typeof ref === 'object' &&
        typeof values === 'object' &&
        !Array.isArray(ref) &&
        !Array.isArray(values)) {

        valuePairs = values;
        values = Object.keys(values);
    }
    else {
        values = [].concat(values);
    }

    options = options || {};            // deep, once, only, part

    exports.assert(arguments.length >= 2, 'Insufficient arguments');
    exports.assert(typeof ref === 'string' || typeof ref === 'object', 'Reference must be string or an object');
    exports.assert(values.length, 'Values array cannot be empty');

    let compare;
    let compareFlags;
    if (options.deep) {
        compare = exports.deepEqual;

        const hasOnly = options.hasOwnProperty('only');
        const hasPart = options.hasOwnProperty('part');

        compareFlags = {
            prototype: hasOnly ? options.only : hasPart ? !options.part : false,
            part: hasOnly ? !options.only : hasPart ? options.part : true
        };
    }
    else {
        compare = (a, b) => a === b;
    }

    let misses = false;
    const matches = new Array(values.length);
    for (let i = 0; i < matches.length; ++i) {
        matches[i] = 0;
    }

    if (typeof ref === 'string') {
        let pattern = '(';
        for (let i = 0; i < values.length; ++i) {
            const value = values[i];
            exports.assert(typeof value === 'string', 'Cannot compare string reference to non-string value');
            pattern += (i ? '|' : '') + exports.escapeRegex(value);
        }

        const regex = new RegExp(pattern + ')', 'g');
        const leftovers = ref.replace(regex, ($0, $1) => {

            const index = values.indexOf($1);
            ++matches[index];
            return '';          // Remove from string
        });

        misses = !!leftovers;
    }
    else if (Array.isArray(ref)) {
        for (let i = 0; i < ref.length; ++i) {
            let matched = false;
            for (let j = 0; j < values.length && matched === false; ++j) {
                matched = compare(values[j], ref[i], compareFlags) && j;
            }

            if (matched !== false) {
                ++matches[matched];
            }
            else {
                misses = true;
            }
        }
    }
    else {
        const keys = Object.getOwnPropertyNames(ref);
        for (let i = 0; i < keys.length; ++i) {
            const key = keys[i];
            const pos = values.indexOf(key);
            if (pos !== -1) {
                if (valuePairs &&
                    !compare(valuePairs[key], ref[key], compareFlags)) {

                    return false;
                }

                ++matches[pos];
            }
            else {
                misses = true;
            }
        }
    }

    let result = false;
    for (let i = 0; i < matches.length; ++i) {
        result = result || !!matches[i];
        if ((options.once && matches[i] > 1) ||
            (!options.part && !matches[i])) {

            return false;
        }
    }

    if (options.only &&
        misses) {

        return false;
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.deepEqual"></a>[function <span class="apidocSignatureSpan">hoek.</span>deepEqual (obj, ref, options, seen)](#apidoc.element.hoek.deepEqual)
- description and source-code
```javascript
deepEqual = function (obj, ref, options, seen) {

    options = options || { prototype: true };

    const type = typeof obj;

    if (type !== typeof ref) {
        return false;
    }

    if (type !== 'object' ||
        obj === null ||
        ref === null) {

        if (obj === ref) {                                                      // Copied from Deep-eql, copyright(c) 2013 Jake
Luer, jake@alogicalparadox.com, MIT Licensed, https://github.com/chaijs/deep-eql
            return obj !== 0 || 1 / obj === 1 / ref;        // -0 / +0
        }

        return obj !== obj && ref !== ref;                  // NaN
    }

    seen = seen || [];
    if (seen.indexOf(obj) !== -1) {
        return true;                            // If previous comparison failed, it would have stopped execution
    }

    seen.push(obj);

    if (Array.isArray(obj)) {
        if (!Array.isArray(ref)) {
            return false;
        }

        if (!options.part && obj.length !== ref.length) {
            return false;
        }

        for (let i = 0; i < obj.length; ++i) {
            if (options.part) {
                let found = false;
                for (let j = 0; j < ref.length; ++j) {
                    if (exports.deepEqual(obj[i], ref[j], options)) {
                        found = true;
                        break;
                    }
                }

                return found;
            }

            if (!exports.deepEqual(obj[i], ref[i], options)) {
                return false;
            }
        }

        return true;
    }

    if (Buffer.isBuffer(obj)) {
        if (!Buffer.isBuffer(ref)) {
            return false;
        }

        if (obj.length !== ref.length) {
            return false;
        }

        for (let i = 0; i < obj.length; ++i) {
            if (obj[i] !== ref[i]) {
                return false;
            }
        }

        return true;
    }

    if (obj instanceof Date) {
        return (ref instanceof Date && obj.getTime() === ref.getTime());
    }

    if (obj instanceof RegExp) {
        return (ref instanceof RegExp && obj.toString() === ref.toString());
    }

    if (options.prototype) {
        if (Object.getPrototypeOf(obj) !== Object.getPrototypeOf(ref)) {
            return false;
        }
    }

    const keys = Object.getOwnPropertyNames(obj);

    if (!options.part && keys.length !== Object.getOwnPropertyNames(ref).length) {
        return false;
    }

    for (let i = 0; i < keys.length; ++i) {
        const key = keys[i];
        const descriptor = Object.getOwnPropertyDescriptor(obj, key);
        if (descriptor.get) {
            if (!exports.deepEqual(descriptor, Object.getOwnPropertyDescriptor(ref, key), options, seen)) {
                return false;
            }
        }
        else if (!exports.deepEqual(obj[key], ref[key], options, seen)) {
            return false;
        }
    }

    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.displayStack"></a>[function <span class="apidocSignatureSpan">hoek.</span>displayStack (slice)](#apidoc.element.hoek.displayStack)
- description and source-code
```javascript
displayStack = function (slice) {

    const trace = exports.callStack(slice === undefined ? 1 : slice + 1);

    return exports.formatTrace(trace);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.escapeHeaderAttribute"></a>[function <span class="apidocSignatureSpan">hoek.</span>escapeHeaderAttribute (attribute)](#apidoc.element.hoek.escapeHeaderAttribute)
- description and source-code
```javascript
escapeHeaderAttribute = function (attribute) {

    // Allowed value characters: !#$%&'()*+,-./:;<=>?@[]^_'{|}~ and space, a-z, A-Z, 0-9, \, "

    exports.assert(/^[ \w\!#\$%&'\(\)\*\+,\-\.\/\:;<\=>\?@\[\]\^'\{\|\}~\"\\]*$/.test(attribute), 'Bad attribute value (' + attribute
 + ')');

    return attribute.replace(/\\/g, '\\\\').replace(/\"/g, '\\"');                             // Escape quotes and slash
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.escapeHtml"></a>[function <span class="apidocSignatureSpan">hoek.</span>escapeHtml (string)](#apidoc.element.hoek.escapeHtml)
- description and source-code
```javascript
escapeHtml = function (string) {

    return Escape.escapeHtml(string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.escapeJavaScript"></a>[function <span class="apidocSignatureSpan">hoek.</span>escapeJavaScript (string)](#apidoc.element.hoek.escapeJavaScript)
- description and source-code
```javascript
escapeJavaScript = function (string) {

    return Escape.escapeJavaScript(string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.escapeRegex"></a>[function <span class="apidocSignatureSpan">hoek.</span>escapeRegex (string)](#apidoc.element.hoek.escapeRegex)
- description and source-code
```javascript
escapeRegex = function (string) {

    // Escape ^$.*+-?=!:|\/()[]{},
    return string.replace(/[\^\$\.\*\+\-\?\=\!\:\|\\\/\(\)\[\]\{\}\,]/g, '\\$&');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.flatten"></a>[function <span class="apidocSignatureSpan">hoek.</span>flatten (array, target)](#apidoc.element.hoek.flatten)
- description and source-code
```javascript
flatten = function (array, target) {

    const result = target || [];

    for (let i = 0; i < array.length; ++i) {
        if (Array.isArray(array[i])) {
            exports.flatten(array[i], result);
        }
        else {
            result.push(array[i]);
        }
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.format"></a>[function <span class="apidocSignatureSpan">hoek.</span>format (f)](#apidoc.element.hoek.format)
- description and source-code
```javascript
format = function (f) {
  if (typeof f !== 'string') {
    const objects = new Array(arguments.length);
    for (var index = 0; index < arguments.length; index++) {
      objects[index] = inspect(arguments[index]);
    }
    return objects.join(' ');
  }

  var argLen = arguments.length;

  if (argLen === 1) return f;

  var str = '';
  var a = 1;
  var lastPos = 0;
  for (var i = 0; i < f.length;) {
    if (f.charCodeAt(i) === 37/*'%'*/ && i + 1 < f.length) {
      switch (f.charCodeAt(i + 1)) {
        case 100: // 'd'
          if (a >= argLen)
            break;
          if (lastPos < i)
            str += f.slice(lastPos, i);
          str += Number(arguments[a++]);
          lastPos = i = i + 2;
          continue;
        case 106: // 'j'
          if (a >= argLen)
            break;
          if (lastPos < i)
            str += f.slice(lastPos, i);
          str += tryStringify(arguments[a++]);
          lastPos = i = i + 2;
          continue;
        case 115: // 's'
          if (a >= argLen)
            break;
          if (lastPos < i)
            str += f.slice(lastPos, i);
          str += String(arguments[a++]);
          lastPos = i = i + 2;
          continue;
        case 37: // '%'
          if (lastPos < i)
            str += f.slice(lastPos, i);
          str += '%';
          lastPos = i = i + 2;
          continue;
      }
    }
    ++i;
  }
  if (lastPos === 0)
    str = f;
  else if (lastPos < f.length)
    str += f.slice(lastPos);
  while (a < argLen) {
    const x = arguments[a++];
    if (x === null || (typeof x !== 'object' && typeof x !== 'symbol')) {
      str += ' ' + x;
    } else {
      str += ' ' + inspect(x);
    }
  }
  return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.formatStack"></a>[function <span class="apidocSignatureSpan">hoek.</span>formatStack (stack)](#apidoc.element.hoek.formatStack)
- description and source-code
```javascript
formatStack = function (stack) {

    const trace = [];
    for (let i = 0; i < stack.length; ++i) {
        const item = stack[i];
        trace.push([item.getFileName(), item.getLineNumber(), item.getColumnNumber(), item.getFunctionName(), item.isConstructor
()]);
    }

    return trace;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.formatTrace"></a>[function <span class="apidocSignatureSpan">hoek.</span>formatTrace (trace)](#apidoc.element.hoek.formatTrace)
- description and source-code
```javascript
formatTrace = function (trace) {

    const display = [];

    for (let i = 0; i < trace.length; ++i) {
        const row = trace[i];
        display.push((row[4] ? 'new ' : '') + row[3] + ' (' + row[0] + ':' + row[1] + ':' + row[2] + ')');
    }

    return display;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.ignore"></a>[function <span class="apidocSignatureSpan">hoek.</span>ignore ()](#apidoc.element.hoek.ignore)
- description and source-code
```javascript
ignore = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.inherits"></a>[function <span class="apidocSignatureSpan">hoek.</span>inherits (ctor, superCtor)](#apidoc.element.hoek.inherits)
- description and source-code
```javascript
inherits = function (ctor, superCtor) {

  if (ctor === undefined || ctor === null)
    throw new TypeError('The constructor to "inherits" must not be ' +
                        'null or undefined');

  if (superCtor === undefined || superCtor === null)
    throw new TypeError('The super constructor to "inherits" must not ' +
                        'be null or undefined');

  if (superCtor.prototype === undefined)
    throw new TypeError('The super constructor to "inherits" must ' +
                        'have a prototype');

  ctor.super_ = superCtor;
  Object.setPrototypeOf(ctor.prototype, superCtor.prototype);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.intersect"></a>[function <span class="apidocSignatureSpan">hoek.</span>intersect (array1, array2, justFirst)](#apidoc.element.hoek.intersect)
- description and source-code
```javascript
intersect = function (array1, array2, justFirst) {

    if (!array1 || !array2) {
        return [];
    }

    const common = [];
    const hash = (Array.isArray(array1) ? exports.mapToObject(array1) : array1);
    const found = {};
    for (let i = 0; i < array2.length; ++i) {
        if (hash[array2[i]] && !found[array2[i]]) {
            if (justFirst) {
                return array2[i];
            }

            common.push(array2[i]);
            found[array2[i]] = true;
        }
    }

    return (justFirst ? null : common);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.isInteger"></a>[function <span class="apidocSignatureSpan">hoek.</span>isInteger ()](#apidoc.element.hoek.isInteger)
- description and source-code
```javascript
function isSafeInteger() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.mapToObject"></a>[function <span class="apidocSignatureSpan">hoek.</span>mapToObject (array, key)](#apidoc.element.hoek.mapToObject)
- description and source-code
```javascript
mapToObject = function (array, key) {

    if (!array) {
        return null;
    }

    const obj = {};
    for (let i = 0; i < array.length; ++i) {
        if (key) {
            if (array[i][key]) {
                obj[array[i][key]] = true;
            }
        }
        else {
            obj[array[i]] = true;
        }
    }

    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.merge"></a>[function <span class="apidocSignatureSpan">hoek.</span>merge (target, source, isNullOverride, isMergeArrays)](#apidoc.element.hoek.merge)
- description and source-code
```javascript
merge = function (target, source, isNullOverride, isMergeArrays) {
<span class="apidocCodeCommentSpan">/*eslint-enable */
</span>
    exports.assert(target && typeof target === 'object', 'Invalid target value: must be an object');
    exports.assert(source === null || source === undefined || typeof source === 'object', 'Invalid source value: must be null, undefined
, or an object');

    if (!source) {
        return target;
    }

    if (Array.isArray(source)) {
        exports.assert(Array.isArray(target), 'Cannot merge array onto an object');
        if (isMergeArrays === false) {                                                  // isMergeArrays defaults to true
            target.length = 0;                                                          // Must not change target assignment
        }

        for (let i = 0; i < source.length; ++i) {
            target.push(exports.clone(source[i]));
        }

        return target;
    }

    const keys = Object.keys(source);
    for (let i = 0; i < keys.length; ++i) {
        const key = keys[i];
        const value = source[key];
        if (value &&
            typeof value === 'object') {

            if (!target[key] ||
                typeof target[key] !== 'object' ||
                (Array.isArray(target[key]) !== Array.isArray(value)) ||
                value instanceof Date ||
                Buffer.isBuffer(value) ||
                value instanceof RegExp) {

                target[key] = exports.clone(value);
            }
            else {
                exports.merge(target[key], value, isNullOverride, isMergeArrays);
            }
        }
        else {
            if (value !== null &&
                value !== undefined) {                              // Explicit to preserve empty strings

                target[key] = value;
            }
            else if (isNullOverride !== false) {                    // Defaults to true
                target[key] = value;
            }
        }
    }

    return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.nextTick"></a>[function <span class="apidocSignatureSpan">hoek.</span>nextTick (callback)](#apidoc.element.hoek.nextTick)
- description and source-code
```javascript
nextTick = function (callback) {

    return function () {

        const args = arguments;
        process.nextTick(() => {

            callback.apply(null, args);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.once"></a>[function <span class="apidocSignatureSpan">hoek.</span>once (method)](#apidoc.element.hoek.once)
- description and source-code
```javascript
once = function (method) {

    if (method._hoekOnce) {
        return method;
    }

    let once = false;
    const wrapped = function () {

        if (!once) {
            once = true;
            method.apply(null, arguments);
        }
    };

    wrapped._hoekOnce = true;

    return wrapped;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.reach"></a>[function <span class="apidocSignatureSpan">hoek.</span>reach (obj, chain, options)](#apidoc.element.hoek.reach)
- description and source-code
```javascript
reach = function (obj, chain, options) {

    if (chain === false ||
        chain === null ||
        typeof chain === 'undefined') {

        return obj;
    }

    options = options || {};
    if (typeof options === 'string') {
        options = { separator: options };
    }

    const path = chain.split(options.separator || '.');
    let ref = obj;
    for (let i = 0; i < path.length; ++i) {
        let key = path[i];
        if (key[0] === '-' && Array.isArray(ref)) {
            key = key.slice(1, key.length);
            key = ref.length - key;
        }

        if (!ref ||
            !((typeof ref === 'object' || typeof ref === 'function') && key in ref) ||
            (typeof ref !== 'object' && options.functions === false)) {         // Only object and function can have properties

            exports.assert(!options.strict || i + 1 === path.length, 'Missing segment', key, 'in reach path ', chain);
            exports.assert(typeof ref === 'object' || options.functions === true || typeof ref !== 'function', 'Invalid segment',
key, 'in reach path ', chain);
            ref = options.default;
            break;
        }

        ref = ref[key];
    }

    return ref;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.reachTemplate"></a>[function <span class="apidocSignatureSpan">hoek.</span>reachTemplate (obj, template, options)](#apidoc.element.hoek.reachTemplate)
- description and source-code
```javascript
reachTemplate = function (obj, template, options) {

    return template.replace(/{([^}]+)}/g, ($0, chain) => {

        const value = exports.reach(obj, chain, options);
        return (value === undefined || value === null ? '' : value);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.shallow"></a>[function <span class="apidocSignatureSpan">hoek.</span>shallow (source)](#apidoc.element.hoek.shallow)
- description and source-code
```javascript
shallow = function (source) {

    const target = {};
    const keys = Object.keys(source);
    for (let i = 0; i < keys.length; ++i) {
        const key = keys[i];
        target[key] = source[key];
    }

    return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.stringify"></a>[function <span class="apidocSignatureSpan">hoek.</span>stringify ()](#apidoc.element.hoek.stringify)
- description and source-code
```javascript
stringify = function () {

    try {
        return JSON.stringify.apply(null, arguments);
    }
    catch (err) {
        return '[Cannot display object: ' + err.message + ']';
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.transform"></a>[function <span class="apidocSignatureSpan">hoek.</span>transform (source, transform, options)](#apidoc.element.hoek.transform)
- description and source-code
```javascript
transform = function (source, transform, options) {

    exports.assert(source === null || source === undefined || typeof source === 'object' || Array.isArray(source), 'Invalid source
 object: must be null, undefined, an object, or an array');
    const separator = (typeof options === 'object' && options !== null) ? (options.separator || '.') : '.';

    if (Array.isArray(source)) {
        const results = [];
        for (let i = 0; i < source.length; ++i) {
            results.push(exports.transform(source[i], transform, options));
        }
        return results;
    }

    const result = {};
    const keys = Object.keys(transform);

    for (let i = 0; i < keys.length; ++i) {
        const key = keys[i];
        const path = key.split(separator);
        const sourcePath = transform[key];

        exports.assert(typeof sourcePath === 'string', 'All mappings must be "." delineated strings');

        let segment;
        let res = result;

        while (path.length > 1) {
            segment = path.shift();
            if (!res[segment]) {
                res[segment] = {};
            }
            res = res[segment];
        }
        segment = path.shift();
        res[segment] = exports.reach(source, sourcePath, options);
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.unique"></a>[function <span class="apidocSignatureSpan">hoek.</span>unique (array, key)](#apidoc.element.hoek.unique)
- description and source-code
```javascript
(array, key) => {

    let result;
    if (key) {
        result = [];
        const index = new Set();
        array.forEach((item) => {

            const identifier = item[key];
            if (!index.has(identifier)) {
                index.add(identifier);
                result.push(item);
            }
        });
    }
    else {
        result = Array.from(new Set(array));
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.uniqueFilename"></a>[function <span class="apidocSignatureSpan">hoek.</span>uniqueFilename (path, extension)](#apidoc.element.hoek.uniqueFilename)
- description and source-code
```javascript
uniqueFilename = function (path, extension) {

    if (extension) {
        extension = extension[0] !== '.' ? '.' + extension : extension;
    }
    else {
        extension = '';
    }

    path = Path.resolve(path);
    const name = [Date.now(), process.pid, Crypto.randomBytes(8).toString('hex')].join('-') + extension;
    return Path.join(path, name);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hoek.Bench"></a>[module hoek.Bench](#apidoc.module.hoek.Bench)

#### <a name="apidoc.element.hoek.Bench.Bench"></a>[function <span class="apidocSignatureSpan">hoek.</span>Bench ()](#apidoc.element.hoek.Bench.Bench)
- description and source-code
```javascript
Bench = function () {

    this.ts = 0;
    this.reset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.Bench.now"></a>[function <span class="apidocSignatureSpan">hoek.Bench.</span>now ()](#apidoc.element.hoek.Bench.now)
- description and source-code
```javascript
now = function () {

    const ts = process.hrtime();
    return (ts[0] * 1e3) + (ts[1] / 1e6);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hoek.Bench.prototype"></a>[module hoek.Bench.prototype](#apidoc.module.hoek.Bench.prototype)

#### <a name="apidoc.element.hoek.Bench.prototype.elapsed"></a>[function <span class="apidocSignatureSpan">hoek.Bench.prototype.</span>elapsed ()](#apidoc.element.hoek.Bench.prototype.elapsed)
- description and source-code
```javascript
elapsed = function () {

    return exports.Bench.now() - this.ts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.Bench.prototype.reset"></a>[function <span class="apidocSignatureSpan">hoek.Bench.prototype.</span>reset ()](#apidoc.element.hoek.Bench.prototype.reset)
- description and source-code
```javascript
reset = function () {

    this.ts = exports.Bench.now();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hoek.Timer"></a>[module hoek.Timer](#apidoc.module.hoek.Timer)

#### <a name="apidoc.element.hoek.Timer.Timer"></a>[function <span class="apidocSignatureSpan">hoek.</span>Timer ()](#apidoc.element.hoek.Timer.Timer)
- description and source-code
```javascript
Timer = function () {

    this.ts = 0;
    this.reset();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hoek.Timer.prototype"></a>[module hoek.Timer.prototype](#apidoc.module.hoek.Timer.prototype)

#### <a name="apidoc.element.hoek.Timer.prototype.elapsed"></a>[function <span class="apidocSignatureSpan">hoek.Timer.prototype.</span>elapsed ()](#apidoc.element.hoek.Timer.prototype.elapsed)
- description and source-code
```javascript
elapsed = function () {

    return Date.now() - this.ts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hoek.Timer.prototype.reset"></a>[function <span class="apidocSignatureSpan">hoek.Timer.prototype.</span>reset ()](#apidoc.element.hoek.Timer.prototype.reset)
- description and source-code
```javascript
reset = function () {

    this.ts = Date.now();
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
