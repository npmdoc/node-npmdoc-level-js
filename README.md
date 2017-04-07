# api documentation for  [level-js (v2.2.4)](https://github.com/maxogden/level.js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-level-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-level-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-level-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-level-js)
#### leveldown/leveldb library for browsers using IndexedDB

[![NPM](https://nodei.co/npm/level-js.png?downloads=true)](https://www.npmjs.com/package/level-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-level-js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-level-js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-level-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-level-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-level-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "max ogden"
    },
    "bugs": {
        "url": "https://github.com/maxogden/level.js/issues"
    },
    "dependencies": {
        "abstract-leveldown": "~0.12.0",
        "idb-wrapper": "^1.5.0",
        "isbuffer": "~0.0.0",
        "ltgt": "^2.1.2",
        "typedarray-to-buffer": "~1.0.0",
        "xtend": "~2.1.2"
    },
    "description": "leveldown/leveldb library for browsers using IndexedDB",
    "devDependencies": {
        "beefy": "~0.3.0",
        "browserify": "^4.1.2",
        "levelup": "~0.18.2",
        "tape": "^4.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "bc055f4180635d4489b561c9486fa370e8c11697",
        "tarball": "https://registry.npmjs.org/level-js/-/level-js-2.2.4.tgz"
    },
    "gitHead": "e819338e87aa305e57ec9c2fe58168ab5dca6da3",
    "homepage": "https://github.com/maxogden/level.js#readme",
    "keywords": [
        "level",
        "leveldb"
    ],
    "license": "BSD-2-Clause",
    "main": "index.js",
    "maintainers": [
        {
            "name": "jameskyburz",
            "email": "james.kyburz@gmail.com"
        },
        {
            "name": "juliangruber",
            "email": "julian@juliangruber.com"
        },
        {
            "name": "matteo.collina",
            "email": "hello@matteocollina.com"
        },
        {
            "name": "maxogden",
            "email": "max@maxogden.com"
        },
        {
            "name": "nolanlawson",
            "email": "nolan@nolanlawson.com"
        }
    ],
    "name": "level-js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/maxogden/level.js.git"
    },
    "scripts": {
        "test": "beefy test/test.js:test.js test/test-levelup.js:test-levelup.js"
    },
    "testling": {
        "files": "test/test.js",
        "browsers": [
            "ie/10..latest",
            "firefox/17..latest",
            "chrome/25..latest",
            "opera/15..latest",
            "safari/6.0..latest"
        ]
    },
    "version": "2.2.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module level-js](#apidoc.module.level-js)
1.  [function <span class="apidocSignatureSpan">level-js.</span>destroy (db, callback)](#apidoc.element.level-js.destroy)
1.  [function <span class="apidocSignatureSpan">level-js.</span>iterator (db, options)](#apidoc.element.level-js.iterator)
1.  [function <span class="apidocSignatureSpan">level-js.</span>super_ (location)](#apidoc.element.level-js.super_)
1.  object <span class="apidocSignatureSpan">level-js.</span>iterator.prototype
1.  object <span class="apidocSignatureSpan">level-js.</span>super_.prototype

#### [module level-js.iterator](#apidoc.module.level-js.iterator)
1.  [function <span class="apidocSignatureSpan">level-js.</span>iterator (db, options)](#apidoc.element.level-js.iterator.iterator)
1.  [function <span class="apidocSignatureSpan">level-js.iterator.</span>super_ (db)](#apidoc.element.level-js.iterator.super_)

#### [module level-js.iterator.prototype](#apidoc.module.level-js.iterator.prototype)
1.  [function <span class="apidocSignatureSpan">level-js.iterator.prototype.</span>_next (callback)](#apidoc.element.level-js.iterator.prototype._next)
1.  [function <span class="apidocSignatureSpan">level-js.iterator.prototype.</span>createIterator ()](#apidoc.element.level-js.iterator.prototype.createIterator)
1.  [function <span class="apidocSignatureSpan">level-js.iterator.prototype.</span>onItem (value, cursor, cursorTransaction)](#apidoc.element.level-js.iterator.prototype.onItem)

#### [module level-js.super_](#apidoc.module.level-js.super_)
1.  [function <span class="apidocSignatureSpan">level-js.</span>super_ (location)](#apidoc.element.level-js.super_.super_)

#### [module level-js.super_.prototype](#apidoc.module.level-js.super_.prototype)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_chainedBatch ()](#apidoc.element.level-js.super_.prototype._chainedBatch)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_checkKeyValue (obj, type)](#apidoc.element.level-js.super_.prototype._checkKeyValue)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_isBuffer (obj)](#apidoc.element.level-js.super_.prototype._isBuffer)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_setupIteratorOptions (options)](#apidoc.element.level-js.super_.prototype._setupIteratorOptions)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>approximateSize (start, end, callback)](#apidoc.element.level-js.super_.prototype.approximateSize)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>batch (array, options, callback)](#apidoc.element.level-js.super_.prototype.batch)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>close (callback)](#apidoc.element.level-js.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>del (key, options, callback)](#apidoc.element.level-js.super_.prototype.del)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>get (key, options, callback)](#apidoc.element.level-js.super_.prototype.get)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>iterator (options)](#apidoc.element.level-js.super_.prototype.iterator)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>open (options, callback)](#apidoc.element.level-js.super_.prototype.open)
1.  [function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>put (key, value, options, callback)](#apidoc.element.level-js.super_.prototype.put)



# <a name="apidoc.module.level-js"></a>[module level-js](#apidoc.module.level-js)

#### <a name="apidoc.element.level-js.destroy"></a>[function <span class="apidocSignatureSpan">level-js.</span>destroy (db, callback)](#apidoc.element.level-js.destroy)
- description and source-code
```javascript
destroy = function (db, callback) {
  if (typeof db === 'object') {
    var prefix = db.IDBOptions.storePrefix || 'IDBWrapper-'
    var dbname = db.location
  } else {
    var prefix = 'IDBWrapper-'
    var dbname = db
  }
  var request = indexedDB.deleteDatabase(prefix + dbname)
  request.onsuccess = function() {
    callback()
  }
  request.onerror = function(err) {
    callback(err)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.iterator"></a>[function <span class="apidocSignatureSpan">level-js.</span>iterator (db, options)](#apidoc.element.level-js.iterator)
- description and source-code
```javascript
function Iterator(db, options) {
  if (!options) options = {}
  this.options = options
  AbstractIterator.call(this, db)
  this._order = options.reverse ? 'DESC': 'ASC'
  this._limit = options.limit
  this._count = 0
  this._done  = false
  var lower = ltgt.lowerBound(options)
  var upper = ltgt.upperBound(options)
  try {
    this._keyRange = lower || upper ? this.db.makeKeyRange({
      lower: lower,
      upper: upper,
      excludeLower: ltgt.lowerBoundExclusive(options),
      excludeUpper: ltgt.upperBoundExclusive(options)
    }) : null
  } catch (e) {
    // The lower key is greater than the upper key.
    // IndexedDB throws an error, but we'll just return 0 results.
    this._keyRangeError = true
  }
  this.callback = null
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_"></a>[function <span class="apidocSignatureSpan">level-js.</span>super_ (location)](#apidoc.element.level-js.super_)
- description and source-code
```javascript
function AbstractLevelDOWN(location) {
  if (!arguments.length || location === undefined)
    throw new Error('constructor requires at least a location argument')

  if (typeof location != 'string')
    throw new Error('constructor requires a location string argument')

  this.location = location
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.level-js.iterator"></a>[module level-js.iterator](#apidoc.module.level-js.iterator)

#### <a name="apidoc.element.level-js.iterator.iterator"></a>[function <span class="apidocSignatureSpan">level-js.</span>iterator (db, options)](#apidoc.element.level-js.iterator.iterator)
- description and source-code
```javascript
function Iterator(db, options) {
  if (!options) options = {}
  this.options = options
  AbstractIterator.call(this, db)
  this._order = options.reverse ? 'DESC': 'ASC'
  this._limit = options.limit
  this._count = 0
  this._done  = false
  var lower = ltgt.lowerBound(options)
  var upper = ltgt.upperBound(options)
  try {
    this._keyRange = lower || upper ? this.db.makeKeyRange({
      lower: lower,
      upper: upper,
      excludeLower: ltgt.lowerBoundExclusive(options),
      excludeUpper: ltgt.upperBoundExclusive(options)
    }) : null
  } catch (e) {
    // The lower key is greater than the upper key.
    // IndexedDB throws an error, but we'll just return 0 results.
    this._keyRangeError = true
  }
  this.callback = null
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.iterator.super_"></a>[function <span class="apidocSignatureSpan">level-js.iterator.</span>super_ (db)](#apidoc.element.level-js.iterator.super_)
- description and source-code
```javascript
function AbstractIterator(db) {
  this.db = db
  this._ended = false
  this._nexting = false
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.level-js.iterator.prototype"></a>[module level-js.iterator.prototype](#apidoc.module.level-js.iterator.prototype)

#### <a name="apidoc.element.level-js.iterator.prototype._next"></a>[function <span class="apidocSignatureSpan">level-js.iterator.prototype.</span>_next (callback)](#apidoc.element.level-js.iterator.prototype._next)
- description and source-code
```javascript
_next = function (callback) {
  if (!callback) return new Error('next() requires a callback argument')
  if (this._keyRangeError) return callback()
  if (!this._started) {
    this.createIterator()
    this._started = true
  }
  this.callback = callback
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.iterator.prototype.createIterator"></a>[function <span class="apidocSignatureSpan">level-js.iterator.prototype.</span>createIterator ()](#apidoc.element.level-js.iterator.prototype.createIterator)
- description and source-code
```javascript
createIterator = function () {
  var self = this

  self.iterator = self.db.iterate(function () {
    self.onItem.apply(self, arguments)
  }, {
    keyRange: self._keyRange,
    autoContinue: false,
    order: self._order,
    onError: function(err) { console.log('horrible error', err) },
  })
}
```
- example usage
```shell
...
  if (cursor) cursor['continue']()
}

Iterator.prototype._next = function (callback) {
  if (!callback) return new Error('next() requires a callback argument')
  if (this._keyRangeError) return callback()
  if (!this._started) {
    this.createIterator()
    this._started = true
  }
  this.callback = callback
}
...
```

#### <a name="apidoc.element.level-js.iterator.prototype.onItem"></a>[function <span class="apidocSignatureSpan">level-js.iterator.prototype.</span>onItem (value, cursor, cursorTransaction)](#apidoc.element.level-js.iterator.prototype.onItem)
- description and source-code
```javascript
onItem = function (value, cursor, cursorTransaction) {
  if (!cursor && this.callback) {
    this.callback()
    this.callback = false
    return
  }
  var shouldCall = true

  if (!!this._limit && this._limit > 0 && this._count++ >= this._limit)
    shouldCall = false

  if (shouldCall) this.callback(false, cursor.key, cursor.value)
  if (cursor) cursor['continue']()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.level-js.super_"></a>[module level-js.super_](#apidoc.module.level-js.super_)

#### <a name="apidoc.element.level-js.super_.super_"></a>[function <span class="apidocSignatureSpan">level-js.</span>super_ (location)](#apidoc.element.level-js.super_.super_)
- description and source-code
```javascript
function AbstractLevelDOWN(location) {
  if (!arguments.length || location === undefined)
    throw new Error('constructor requires at least a location argument')

  if (typeof location != 'string')
    throw new Error('constructor requires a location string argument')

  this.location = location
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.level-js.super_.prototype"></a>[module level-js.super_.prototype](#apidoc.module.level-js.super_.prototype)

#### <a name="apidoc.element.level-js.super_.prototype._chainedBatch"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_chainedBatch ()](#apidoc.element.level-js.super_.prototype._chainedBatch)
- description and source-code
```javascript
_chainedBatch = function () {
  return new AbstractChainedBatch(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype._checkKeyValue"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_checkKeyValue (obj, type)](#apidoc.element.level-js.super_.prototype._checkKeyValue)
- description and source-code
```javascript
_checkKeyValue = function (obj, type) {

  if (obj === null || obj === undefined)
    return new Error(type + ' cannot be 'null' or 'undefined'')

  if (this._isBuffer(obj)) {
    if (obj.length === 0)
      return new Error(type + ' cannot be an empty Buffer')
  } else if (String(obj) === '')
    return new Error(type + ' cannot be an empty String')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype._isBuffer"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_isBuffer (obj)](#apidoc.element.level-js.super_.prototype._isBuffer)
- description and source-code
```javascript
_isBuffer = function (obj) {
  return Buffer.isBuffer(obj)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype._setupIteratorOptions"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>_setupIteratorOptions (options)](#apidoc.element.level-js.super_.prototype._setupIteratorOptions)
- description and source-code
```javascript
_setupIteratorOptions = function (options) {
  var self = this

  options = xtend(options)

  ;[ 'start', 'end', 'gt', 'gte', 'lt', 'lte' ].forEach(function (o) {
    if (options[o] && self._isBuffer(options[o]) && options[o].length === 0)
      delete options[o]
  })

  options.reverse = !!options.reverse

  // fix 'start' so it takes into account gt, gte, lt, lte as appropriate
  if (options.reverse && options.lt)
    options.start = options.lt
  if (options.reverse && options.lte)
    options.start = options.lte
  if (!options.reverse && options.gt)
    options.start = options.gt
  if (!options.reverse && options.gte)
    options.start = options.gte

  if ((options.reverse && options.lt && !options.lte)
    || (!options.reverse && options.gt && !options.gte))
    options.exclusiveStart = true // start should *not* include matching key

  return options
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype.approximateSize"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>approximateSize (start, end, callback)](#apidoc.element.level-js.super_.prototype.approximateSize)
- description and source-code
```javascript
approximateSize = function (start, end, callback) {
  if (   start == null
      || end == null
      || typeof start == 'function'
      || typeof end == 'function') {
    throw new Error('approximateSize() requires valid 'start', 'end' and 'callback' arguments')
  }

  if (typeof callback != 'function')
    throw new Error('approximateSize() requires a callback argument')

  if (!this._isBuffer(start))
    start = String(start)

  if (!this._isBuffer(end))
    end = String(end)

  if (typeof this._approximateSize == 'function')
    return this._approximateSize(start, end, callback)

  process.nextTick(function () {
    callback(null, 0)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype.batch"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>batch (array, options, callback)](#apidoc.element.level-js.super_.prototype.batch)
- description and source-code
```javascript
batch = function (array, options, callback) {
  if (!arguments.length)
    return this._chainedBatch()

  if (typeof options == 'function')
    callback = options

  if (typeof callback != 'function')
    throw new Error('batch(array) requires a callback argument')

  if (!Array.isArray(array))
    return callback(new Error('batch(array) requires an array argument'))

  if (typeof options != 'object')
    options = {}

  var i = 0
    , l = array.length
    , e
    , err

  for (; i < l; i++) {
    e = array[i]
    if (typeof e != 'object')
      continue

    if (err = this._checkKeyValue(e.type, 'type', this._isBuffer))
      return callback(err)

    if (err = this._checkKeyValue(e.key, 'key', this._isBuffer))
      return callback(err)

    if (e.type == 'put') {
      if (err = this._checkKeyValue(e.value, 'value', this._isBuffer))
        return callback(err)
    }
  }

  if (typeof this._batch == 'function')
    return this._batch(array, options, callback)

  process.nextTick(callback)
}
```
- example usage
```shell
...
        copiedOp[k] = 'remove'
      } else {
        copiedOp[k] = currentOp[k]
      }
    }
  }

  return this.idb.batch(modified, function(){ callback() }, callback)
}

Level.prototype._close = function (callback) {
  this.idb.db.close()
  callback()
}
...
```

#### <a name="apidoc.element.level-js.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>close (callback)](#apidoc.element.level-js.super_.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  if (typeof callback != 'function')
    throw new Error('close() requires a callback argument')

  if (typeof this._close == 'function')
    return this._close(callback)

  process.nextTick(callback)
}
```
- example usage
```shell
...
  }
}

return this.idb.batch(modified, function(){ callback() }, callback)
}

Level.prototype._close = function (callback) {
this.idb.db.close()
callback()
}

Level.prototype._approximateSize = function (start, end, callback) {
var err = new Error('Not implemented')
if (callback)
  return callback(err)
...
```

#### <a name="apidoc.element.level-js.super_.prototype.del"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>del (key, options, callback)](#apidoc.element.level-js.super_.prototype.del)
- description and source-code
```javascript
del = function (key, options, callback) {
  var err

  if (typeof options == 'function')
    callback = options

  if (typeof callback != 'function')
    throw new Error('del() requires a callback argument')

  if (err = this._checkKeyValue(key, 'key', this._isBuffer))
    return callback(err)

  if (!this._isBuffer(key))
    key = String(key)

  if (typeof options != 'object')
    options = {}

  if (typeof this._del == 'function')
    return this._del(key, options, callback)

  process.nextTick(callback)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype.get"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>get (key, options, callback)](#apidoc.element.level-js.super_.prototype.get)
- description and source-code
```javascript
get = function (key, options, callback) {
  var err

  if (typeof options == 'function')
    callback = options

  if (typeof callback != 'function')
    throw new Error('get() requires a callback argument')

  if (err = this._checkKeyValue(key, 'key', this._isBuffer))
    return callback(err)

  if (!this._isBuffer(key))
    key = String(key)

  if (typeof options != 'object')
    options = {}

  if (typeof this._get == 'function')
    return this._get(key, options, callback)

  process.nextTick(function () { callback(new Error('NotFound')) })
}
```
- example usage
```shell
...

xtend(idbOpts, options)
this.IDBOptions = idbOpts
this.idb = new IDB(idbOpts)
}

Level.prototype._get = function (key, options, callback) {
this.idb.get(key, function (value) {
  if (value === undefined) {
    // 'NotFound' error, consistent with LevelDOWN API
    return callback(new Error('NotFound'))
  }
  // by default return buffers, unless explicitly told not to
  var asBuffer = true
  if (options.asBuffer === false) asBuffer = false
...
```

#### <a name="apidoc.element.level-js.super_.prototype.iterator"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>iterator (options)](#apidoc.element.level-js.super_.prototype.iterator)
- description and source-code
```javascript
iterator = function (options) {
  if (typeof options != 'object')
    options = {}

  options = this._setupIteratorOptions(options)

  if (typeof this._iterator == 'function')
    return this._iterator(options)

  return new AbstractIterator(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.level-js.super_.prototype.open"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>open (options, callback)](#apidoc.element.level-js.super_.prototype.open)
- description and source-code
```javascript
open = function (options, callback) {
  if (typeof options == 'function')
    callback = options

  if (typeof callback != 'function')
    throw new Error('open() requires a callback argument')

  if (typeof options != 'object')
    options = {}

  if (typeof this._open == 'function')
    return this._open(options, callback)

  process.nextTick(callback)
}
```
- example usage
```shell
...
This library is best used with [browserify](http://browserify.org)

## code examples

'''js
var leveljs = require('level-js')
var db = leveljs('bigdata')
db.open(function onOpen() { })
'''

The test suite for this library is in the [abstract-leveldown](https://github.com/rvagg/node-abstract-leveldown) repo and is shared
 between various leveldown implementations across different environments and platforms.

For more code examples see the [abstract-leveldown test suite](https://github.com/rvagg/node-abstract-leveldown/tree/master/abstract
)

The only differences between this and leveldown is that you can store 'ArrayBuffers' in this (whereas leveldown just uses node '
Buffer' objects)
...
```

#### <a name="apidoc.element.level-js.super_.prototype.put"></a>[function <span class="apidocSignatureSpan">level-js.super_.prototype.</span>put (key, value, options, callback)](#apidoc.element.level-js.super_.prototype.put)
- description and source-code
```javascript
put = function (key, value, options, callback) {
  var err

  if (typeof options == 'function')
    callback = options

  if (typeof callback != 'function')
    throw new Error('put() requires a callback argument')

  if (err = this._checkKeyValue(key, 'key', this._isBuffer))
    return callback(err)

  if (err = this._checkKeyValue(value, 'value', this._isBuffer))
    return callback(err)

  if (!this._isBuffer(key))
    key = String(key)

  // coerce value to string in node, don't touch it in browser
  // (indexeddb can store any JS type)
  if (!this._isBuffer(value) && !process.browser)
    value = String(value)

  if (typeof options != 'object')
    options = {}

  if (typeof this._put == 'function')
    return this._put(key, value, options, callback)

  process.nextTick(callback)
}
```
- example usage
```shell
...
if (Buffer.isBuffer(obj.value)) {
  if (typeof value.toArrayBuffer === 'function') {
    obj.value = new Uint8Array(value.toArrayBuffer())
  } else {
    obj.value = new Uint8Array(value)
  }
}
this.idb.put(obj.key, obj.value, function() { callback() }, callback)
}

Level.prototype.convertEncoding = function(key, value, options) {
if (options.raw) return {key: key, value: value}
if (value) {
  var stringed = value.toString()
  if (stringed === 'NaN') value = 'NaN'
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
