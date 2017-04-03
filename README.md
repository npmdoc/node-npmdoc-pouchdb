# api documentation for  [pouchdb (v6.1.2)](https://github.com/pouchdb/pouchdb#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-pouchdb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pouchdb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pouchdb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pouchdb)
#### PouchDB is a pocket-sized database

[![NPM](https://nodei.co/npm/pouchdb.png?downloads=true)](https://www.npmjs.com/package/pouchdb)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pouchdb/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-pouchdb_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pouchdb/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pouchdb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pouchdb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dale Harvey",
        "email": "dale@arandomurl.com"
    },
    "browser": {
        "./lib/index.js": "./lib/index-browser.js",
        "./lib/index.es.js": "./lib/index-browser.es.js"
    },
    "bugs": {
        "url": "https://github.com/pouchdb/pouchdb/issues"
    },
    "dependencies": {
        "argsarray": "0.0.1",
        "buffer-from": "0.1.1",
        "clone-buffer": "1.0.0",
        "debug": "2.6.0",
        "double-ended-queue": "2.1.0-0",
        "immediate": "3.0.6",
        "inherits": "2.0.3",
        "level-codec": "7.0.0",
        "level-write-stream": "1.0.0",
        "leveldown": "1.5.0",
        "levelup": "1.3.3",
        "lie": "3.1.0",
        "ltgt": "2.1.2",
        "readable-stream": "1.0.33",
        "request": "2.79.0",
        "scope-eval": "0.0.3",
        "spark-md5": "3.0.0",
        "through2": "2.0.1",
        "vuvuzela": "1.0.3"
    },
    "description": "PouchDB is a pocket-sized database",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "5ceb310f705f0a7fd23d25fe1a365f36b30ac28b",
        "tarball": "https://registry.npmjs.org/pouchdb/-/pouchdb-6.1.2.tgz"
    },
    "files": [
        "lib",
        "dist",
        "tonic-example.js"
    ],
    "homepage": "https://github.com/pouchdb/pouchdb#readme",
    "jsnext:main": "./lib/index.es.js",
    "jspm": {
        "main": "dist/pouchdb.js"
    },
    "keywords": [
        "db",
        "couchdb",
        "pouchdb"
    ],
    "license": "Apache-2.0",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "chesles",
            "email": "john@chesl.es"
        },
        {
            "name": "cwmma",
            "email": "calvin.metcalf@gmail.com"
        },
        {
            "name": "daleharvey",
            "email": "dale@arandomurl.com"
        },
        {
            "name": "eckoit",
            "email": "ryan.ramage@gmail.com"
        },
        {
            "name": "nickcolley",
            "email": "nickcolley7@gmail.com"
        },
        {
            "name": "nolanlawson",
            "email": "nolan@nolanlawson.com"
        }
    ],
    "name": "pouchdb",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/pouchdb/pouchdb.git"
    },
    "scripts": {},
    "tags": [
        "db",
        "couchdb",
        "pouchdb"
    ],
    "tonicExampleFilename": "tonic-example.js",
    "version": "6.1.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module pouchdb](#apidoc.module.pouchdb)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>adapter (id, obj$$1, addToPreferredAdapters)](#apidoc.element.pouchdb.adapter)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>adapters.http (opts, callback)](#apidoc.element.pouchdb.adapters.http)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>adapters.leveldb (opts, callback)](#apidoc.element.pouchdb.adapters.leveldb)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>addListener ()](#apidoc.element.pouchdb.addListener)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>debug (namespace)](#apidoc.element.pouchdb.debug)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>defaults (defaultOpts)](#apidoc.element.pouchdb.defaults)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>emit ()](#apidoc.element.pouchdb.emit)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>eventNames ()](#apidoc.element.pouchdb.eventNames)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>getMaxListeners ()](#apidoc.element.pouchdb.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>listenerCount ()](#apidoc.element.pouchdb.listenerCount)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>listeners ()](#apidoc.element.pouchdb.listeners)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>on ()](#apidoc.element.pouchdb.on)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>once ()](#apidoc.element.pouchdb.once)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>plugin (obj$$1)](#apidoc.element.pouchdb.plugin)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>prependListener ()](#apidoc.element.pouchdb.prependListener)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>prependOnceListener ()](#apidoc.element.pouchdb.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>removeAllListeners ()](#apidoc.element.pouchdb.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>removeListener ()](#apidoc.element.pouchdb.removeListener)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>replicate (src, target, opts, callback)](#apidoc.element.pouchdb.replicate)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>setMaxListeners ()](#apidoc.element.pouchdb.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>super_ ()](#apidoc.element.pouchdb.super_)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>sync (src, target, opts, callback)](#apidoc.element.pouchdb.sync)
1.  object <span class="apidocSignatureSpan">pouchdb.</span>_destructionListeners
1.  object <span class="apidocSignatureSpan">pouchdb.</span>adapters
1.  object <span class="apidocSignatureSpan">pouchdb.</span>debug.formatters
1.  object <span class="apidocSignatureSpan">pouchdb.</span>preferredAdapters
1.  object <span class="apidocSignatureSpan">pouchdb.</span>super_.prototype
1.  string <span class="apidocSignatureSpan">pouchdb.</span>prefix
1.  string <span class="apidocSignatureSpan">pouchdb.</span>version

#### [module pouchdb.adapters](#apidoc.module.pouchdb.adapters)
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.</span>http (opts, callback)](#apidoc.element.pouchdb.adapters.http)
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.</span>https (opts, callback)](#apidoc.element.pouchdb.adapters.https)
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.</span>leveldb (opts, callback)](#apidoc.element.pouchdb.adapters.leveldb)

#### [module pouchdb.adapters.http](#apidoc.module.pouchdb.adapters.http)
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.</span>http (opts, callback)](#apidoc.element.pouchdb.adapters.http.http)
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.http.</span>valid ()](#apidoc.element.pouchdb.adapters.http.valid)

#### [module pouchdb.adapters.leveldb](#apidoc.module.pouchdb.adapters.leveldb)
1.  boolean <span class="apidocSignatureSpan">pouchdb.adapters.leveldb.</span>use_prefix
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.</span>leveldb (opts, callback)](#apidoc.element.pouchdb.adapters.leveldb.leveldb)
1.  [function <span class="apidocSignatureSpan">pouchdb.adapters.leveldb.</span>valid ()](#apidoc.element.pouchdb.adapters.leveldb.valid)

#### [module pouchdb.debug](#apidoc.module.pouchdb.debug)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>debug (namespace)](#apidoc.element.pouchdb.debug.debug)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>coerce (val)](#apidoc.element.pouchdb.debug.coerce)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>default (namespace)](#apidoc.element.pouchdb.debug.default)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>disable ()](#apidoc.element.pouchdb.debug.disable)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>enable (namespaces)](#apidoc.element.pouchdb.debug.enable)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>enabled (name)](#apidoc.element.pouchdb.debug.enabled)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>formatArgs (args)](#apidoc.element.pouchdb.debug.formatArgs)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>humanize (val, options)](#apidoc.element.pouchdb.debug.humanize)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>init (debug)](#apidoc.element.pouchdb.debug.init)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>load ()](#apidoc.element.pouchdb.debug.load)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>log ()](#apidoc.element.pouchdb.debug.log)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>save (namespaces)](#apidoc.element.pouchdb.debug.save)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.</span>useColors ()](#apidoc.element.pouchdb.debug.useColors)
1.  object <span class="apidocSignatureSpan">pouchdb.debug.</span>colors
1.  object <span class="apidocSignatureSpan">pouchdb.debug.</span>formatters
1.  object <span class="apidocSignatureSpan">pouchdb.debug.</span>inspectOpts
1.  object <span class="apidocSignatureSpan">pouchdb.debug.</span>names
1.  object <span class="apidocSignatureSpan">pouchdb.debug.</span>skips

#### [module pouchdb.debug.formatters](#apidoc.module.pouchdb.debug.formatters)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.formatters.</span>O (v)](#apidoc.element.pouchdb.debug.formatters.O)
1.  [function <span class="apidocSignatureSpan">pouchdb.debug.formatters.</span>o (v)](#apidoc.element.pouchdb.debug.formatters.o)

#### [module pouchdb.super_](#apidoc.module.pouchdb.super_)
1.  [function <span class="apidocSignatureSpan">pouchdb.</span>super_ ()](#apidoc.element.pouchdb.super_.super_)

#### [module pouchdb.super_.prototype](#apidoc.module.pouchdb.super_.prototype)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>_compact (opts, callback)](#apidoc.element.pouchdb.super_.prototype._compact)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>allDocs ()](#apidoc.element.pouchdb.super_.prototype.allDocs)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>bulkDocs ()](#apidoc.element.pouchdb.super_.prototype.bulkDocs)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>bulkGet ()](#apidoc.element.pouchdb.super_.prototype.bulkGet)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>changes (opts, callback)](#apidoc.element.pouchdb.super_.prototype.changes)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>close ()](#apidoc.element.pouchdb.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>compact ()](#apidoc.element.pouchdb.super_.prototype.compact)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>compactDocument ()](#apidoc.element.pouchdb.super_.prototype.compactDocument)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>destroy ()](#apidoc.element.pouchdb.super_.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>get ()](#apidoc.element.pouchdb.super_.prototype.get)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>getAttachment ()](#apidoc.element.pouchdb.super_.prototype.getAttachment)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>id ()](#apidoc.element.pouchdb.super_.prototype.id)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>info ()](#apidoc.element.pouchdb.super_.prototype.info)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>post ()](#apidoc.element.pouchdb.super_.prototype.post)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>put ()](#apidoc.element.pouchdb.super_.prototype.put)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>putAttachment ()](#apidoc.element.pouchdb.super_.prototype.putAttachment)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>registerDependentDatabase ()](#apidoc.element.pouchdb.super_.prototype.registerDependentDatabase)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>remove ()](#apidoc.element.pouchdb.super_.prototype.remove)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>removeAttachment ()](#apidoc.element.pouchdb.super_.prototype.removeAttachment)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>revsDiff ()](#apidoc.element.pouchdb.super_.prototype.revsDiff)
1.  [function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>type ()](#apidoc.element.pouchdb.super_.prototype.type)



# <a name="apidoc.module.pouchdb"></a>[module pouchdb](#apidoc.module.pouchdb)

#### <a name="apidoc.element.pouchdb.adapter"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>adapter (id, obj$$1, addToPreferredAdapters)](#apidoc.element.pouchdb.adapter)
- description and source-code
```javascript
adapter = function (id, obj$$1, addToPreferredAdapters) {
<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (obj$$1.valid()) {
    PouchDB$5.adapters[id] = obj$$1;
    if (addToPreferredAdapters) {
      PouchDB$5.preferredAdapters.push(id);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.adapters.http"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>adapters.http (opts, callback)](#apidoc.element.pouchdb.adapters.http)
- description and source-code
```javascript
function HttpPouch(opts, callback) {

  // The functions that will be publicly available for HttpPouch
  var api = this;

  var host = getHost(opts.name, opts);
  var dbUrl = genDBUrl(host, '');

  opts = clone(opts);
  var ajaxOpts = opts.ajax || {};

  if (opts.auth || host.auth) {
    var nAuth = opts.auth || host.auth;
    var str = nAuth.username + ':' + nAuth.password;
    var token = thisBtoa(unescape(encodeURIComponent(str)));
    ajaxOpts.headers = ajaxOpts.headers || {};
    ajaxOpts.headers.Authorization = 'Basic ' + token;
  }

  // Not strictly necessary, but we do this because numerous tests
  // rely on swapping ajax in and out.
  api._ajax = ajax;

  function ajax$$1(userOpts, options, callback) {
    var reqAjax = userOpts.ajax || {};
    var reqOpts = $inject_Object_assign(clone(ajaxOpts), reqAjax, options);
    var defaultHeaders = clone(ajaxOpts.headers || {});
    reqOpts.headers = $inject_Object_assign(defaultHeaders, reqAjax.headers,
      options.headers || {});
    log$1(reqOpts.method + ' ' + reqOpts.url);
    return api._ajax(reqOpts, callback);
  }

  function ajaxPromise(userOpts, opts) {
    return new PouchPromise$1(function (resolve, reject) {
      ajax$$1(userOpts, opts, function (err, res$$1) {
<span class="apidocCodeCommentSpan">        /* istanbul ignore if */
</span>        if (err) {
          return reject(err);
        }
        resolve(res$$1);
      });
    });
  }

  function adapterFun$$1(name, fun) {
    return adapterFun(name, getArguments(function (args) {
      setup().then(function () {
        return fun.apply(this, args);
      }).catch(function (e) {
        var callback = args.pop();
        callback(e);
      });
    }));
  }

  var setupPromise;

  function setup() {
    // TODO: Remove 'skipSetup' in favor of 'skip_setup' in a future release
    if (opts.skipSetup || opts.skip_setup) {
      return PouchPromise$1.resolve();
    }

    // If there is a setup in process or previous successful setup
    // done then we will use that
    // If previous setups have been rejected we will try again
    if (setupPromise) {
      return setupPromise;
    }

    var checkExists = {method: 'GET', url: dbUrl};
    setupPromise = ajaxPromise({}, checkExists).catch(function (err) {
      if (err && err.status && err.status === 404) {
        // Doesnt exist, create it
        res(404, 'PouchDB is just detecting if the remote exists.');
        return ajaxPromise({}, {method: 'PUT', url: dbUrl});
      } else {
        return PouchPromise$1.reject(err);
      }
    }).catch(function (err) {
      // If we try to create a database that already exists, skipped in
      // istanbul since its catching a race condition.
      /* istanbul ignore if */
      if (err && err.status && err.status === 412) {
        return true;
      }
      return PouchPromise$1.reject(err);
    });

    setupPromise.catch(function () {
      setupPromise = null;
    });

    return setupPromise;
  }

  nextTick(function () {
    callback(null, api);
  });

  api.type = function () {
    return 'http';
  };

  api.id = adapterFun$$1('id', function (callback) {
    ajax$$1({}, {method: 'GET', url: genUrl(host, '')}, function (err, result) {
      var uuid$$1 = (result && result.uuid) ?
        (result.uuid + host.db) : genDBUrl(host, '');
      callback(null, uuid$$1);
    });
  });

  api.request = adapterFun$$1('request', function (options, callback) {
    options.url = genDBUrl(host, options.url);
    ajax$$1({}, options, callback);
  });

  // Sends a POST request to the host calling the couchdb _compact function
  //    version: The version of CouchDB it is running
  api.compact = adapterFun$$1('compact', function (opts, callback) {
    if (typeof opts === 'function') {
      callback = opts;
      opts = {};
    }
    opts = clone(opts);
    ajax$$1(opts, {
      url: genDBUrl(host, '_compact'),
      method: 'POST'
    }, function () {
      function ping() {
        api.info(function (err, res$$1) {
          if (res$$1 && !res$$1.compact_running) {
            callback(null, {ok: true});
          } else {
            setTimeout(ping, opts ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.adapters.leveldb"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>adapters.leveldb (opts, callback)](#apidoc.element.pouchdb.adapters.leveldb)
- description and source-code
```javascript
function LevelDownPouch(opts, callback) {

  // Users can pass in their own leveldown alternative here, in which case
  // it overrides the default one. (This is in addition to the custom builds.)
  var leveldown = opts.db;

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (!leveldown) {
    leveldown = requireLeveldown();

    /* istanbul ignore if */
    if (leveldown instanceof Error) {
      return callback(leveldown);
    }
  }

  var _opts = $inject_Object_assign({
    db: leveldown,
    migrate: migrate
  }, opts);

  LevelPouch$1.call(this, _opts, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.addListener"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>addListener ()](#apidoc.element.pouchdb.addListener)
- description and source-code
```javascript
addListener = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>debug (namespace)](#apidoc.element.pouchdb.debug)
- description and source-code
```javascript
function createDebug(namespace) {

  function debug() {
    // disabled?
    if (!debug.enabled) return;

    var self = debug;

    // set 'diff' timestamp
    var curr = +new Date();
    var ms = curr - (prevTime || curr);
    self.diff = ms;
    self.prev = prevTime;
    self.curr = curr;
    prevTime = curr;

    // turn the 'arguments' into a proper Array
    var args = new Array(arguments.length);
    for (var i = 0; i < args.length; i++) {
      args[i] = arguments[i];
    }

    args[0] = exports.coerce(args[0]);

    if ('string' !== typeof args[0]) {
      // anything else let's inspect with %O
      args.unshift('%O');
    }

    // apply any 'formatters' transformations
    var index = 0;
    args[0] = args[0].replace(/%([a-zA-Z%])/g, function(match, format) {
      // if we encounter an escaped % then don't increase the array index
      if (match === '%%') return match;
      index++;
      var formatter = exports.formatters[format];
      if ('function' === typeof formatter) {
        var val = args[index];
        match = formatter.call(self, val);

        // now we need to remove 'args[index]' since it's inlined in the 'format'
        args.splice(index, 1);
        index--;
      }
      return match;
    });

    // apply env-specific formatting (colors, etc.)
    exports.formatArgs.call(self, args);

    var logFn = debug.log || exports.log || console.log.bind(console);
    logFn.apply(self, args);
  }

  debug.namespace = namespace;
  debug.enabled = exports.enabled(namespace);
  debug.useColors = exports.useColors();
  debug.color = selectColor(namespace);

  // env-specific initialization logic for debug instances
  if ('function' === typeof exports.init) {
    exports.init(debug);
  }

  return debug;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.defaults"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>defaults (defaultOpts)](#apidoc.element.pouchdb.defaults)
- description and source-code
```javascript
defaults = function (defaultOpts) {
  function PouchAlt(name, opts) {
    if (!(this instanceof PouchAlt)) {
      return new PouchAlt(name, opts);
    }

    opts = opts || {};

    if (name && typeof name === 'object') {
      opts = name;
      name = opts.name;
      delete opts.name;
    }

    opts = $inject_Object_assign({}, PouchAlt.__defaults, opts);
    PouchDB$5.call(this, name, opts);
  }

  inherits(PouchAlt, PouchDB$5);

  PouchAlt.preferredAdapters = PouchDB$5.preferredAdapters.slice();
  Object.keys(PouchDB$5).forEach(function (key) {
    if (!(key in PouchAlt)) {
      PouchAlt[key] = PouchDB$5[key];
    }
  });

  // make default options transitive
  // https://github.com/pouchdb/pouchdb/issues/5922
  PouchAlt.__defaults = $inject_Object_assign({}, this.__defaults, defaultOpts);

  return PouchAlt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.emit"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>emit ()](#apidoc.element.pouchdb.emit)
- description and source-code
```javascript
emit = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.eventNames"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>eventNames ()](#apidoc.element.pouchdb.eventNames)
- description and source-code
```javascript
eventNames = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.getMaxListeners"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>getMaxListeners ()](#apidoc.element.pouchdb.getMaxListeners)
- description and source-code
```javascript
getMaxListeners = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.listenerCount"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>listenerCount ()](#apidoc.element.pouchdb.listenerCount)
- description and source-code
```javascript
listenerCount = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.listeners"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>listeners ()](#apidoc.element.pouchdb.listeners)
- description and source-code
```javascript
listeners = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.on"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>on ()](#apidoc.element.pouchdb.on)
- description and source-code
```javascript
on = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.once"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>once ()](#apidoc.element.pouchdb.once)
- description and source-code
```javascript
once = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.plugin"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>plugin (obj$$1)](#apidoc.element.pouchdb.plugin)
- description and source-code
```javascript
plugin = function (obj$$1) {
  if (typeof obj$$1 === 'function') { // function style for plugins
    obj$$1(PouchDB$5);
  } else if (typeof obj$$1 !== 'object' || Object.keys(obj$$1).length === 0){
    throw new Error('Invalid plugin: got \"' + obj$$1 + '\", expected an object or a function');
  } else {
    Object.keys(obj$$1).forEach(function (id) { // object style for plugins
      PouchDB$5.prototype[id] = obj$$1[id];
    });
  }
  if (this.__defaults) {
    PouchDB$5.__defaults = $inject_Object_assign({}, this.__defaults);
  }
  return PouchDB$5;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.prependListener"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>prependListener ()](#apidoc.element.pouchdb.prependListener)
- description and source-code
```javascript
prependListener = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.prependOnceListener"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>prependOnceListener ()](#apidoc.element.pouchdb.prependOnceListener)
- description and source-code
```javascript
prependOnceListener = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.removeAllListeners"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>removeAllListeners ()](#apidoc.element.pouchdb.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.removeListener"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>removeListener ()](#apidoc.element.pouchdb.removeListener)
- description and source-code
```javascript
removeListener = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.replicate"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>replicate (src, target, opts, callback)](#apidoc.element.pouchdb.replicate)
- description and source-code
```javascript
function replicateWrapper(src, target, opts, callback) {

  if (typeof opts === 'function') {
    callback = opts;
    opts = {};
  }
  if (typeof opts === 'undefined') {
    opts = {};
  }

  if (opts.doc_ids && !Array.isArray(opts.doc_ids)) {
    throw createError(BAD_REQUEST,
                       "'doc_ids' filter parameter is not a list.");
  }

  opts.complete = callback;
  opts = clone(opts);
  opts.continuous = opts.continuous || opts.live;
  opts.retry = ('retry' in opts) ? opts.retry : false;
<span class="apidocCodeCommentSpan">  /*jshint validthis:true */
</span>  opts.PouchConstructor = opts.PouchConstructor || this;
  var replicateRet = new Replication(opts);
  var srcPouch = toPouch(src, opts);
  var targetPouch = toPouch(target, opts);
  replicate(srcPouch, targetPouch, opts, replicateRet);
  return replicateRet;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.setMaxListeners"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>setMaxListeners ()](#apidoc.element.pouchdb.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>super_ ()](#apidoc.element.pouchdb.super_)
- description and source-code
```javascript
function AbstractPouchDB() {
  events.EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.sync"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>sync (src, target, opts, callback)](#apidoc.element.pouchdb.sync)
- description and source-code
```javascript
function sync$1(src, target, opts, callback) {
  if (typeof opts === 'function') {
    callback = opts;
    opts = {};
  }
  if (typeof opts === 'undefined') {
    opts = {};
  }
  opts = clone(opts);
<span class="apidocCodeCommentSpan">  /*jshint validthis:true */
</span>  opts.PouchConstructor = opts.PouchConstructor || this;
  src = toPouch(src, opts);
  target = toPouch(target, opts);
  return new Sync(src, target, opts, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pouchdb.adapters"></a>[module pouchdb.adapters](#apidoc.module.pouchdb.adapters)

#### <a name="apidoc.element.pouchdb.adapters.http"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.</span>http (opts, callback)](#apidoc.element.pouchdb.adapters.http)
- description and source-code
```javascript
function HttpPouch(opts, callback) {

  // The functions that will be publicly available for HttpPouch
  var api = this;

  var host = getHost(opts.name, opts);
  var dbUrl = genDBUrl(host, '');

  opts = clone(opts);
  var ajaxOpts = opts.ajax || {};

  if (opts.auth || host.auth) {
    var nAuth = opts.auth || host.auth;
    var str = nAuth.username + ':' + nAuth.password;
    var token = thisBtoa(unescape(encodeURIComponent(str)));
    ajaxOpts.headers = ajaxOpts.headers || {};
    ajaxOpts.headers.Authorization = 'Basic ' + token;
  }

  // Not strictly necessary, but we do this because numerous tests
  // rely on swapping ajax in and out.
  api._ajax = ajax;

  function ajax$$1(userOpts, options, callback) {
    var reqAjax = userOpts.ajax || {};
    var reqOpts = $inject_Object_assign(clone(ajaxOpts), reqAjax, options);
    var defaultHeaders = clone(ajaxOpts.headers || {});
    reqOpts.headers = $inject_Object_assign(defaultHeaders, reqAjax.headers,
      options.headers || {});
    log$1(reqOpts.method + ' ' + reqOpts.url);
    return api._ajax(reqOpts, callback);
  }

  function ajaxPromise(userOpts, opts) {
    return new PouchPromise$1(function (resolve, reject) {
      ajax$$1(userOpts, opts, function (err, res$$1) {
<span class="apidocCodeCommentSpan">        /* istanbul ignore if */
</span>        if (err) {
          return reject(err);
        }
        resolve(res$$1);
      });
    });
  }

  function adapterFun$$1(name, fun) {
    return adapterFun(name, getArguments(function (args) {
      setup().then(function () {
        return fun.apply(this, args);
      }).catch(function (e) {
        var callback = args.pop();
        callback(e);
      });
    }));
  }

  var setupPromise;

  function setup() {
    // TODO: Remove 'skipSetup' in favor of 'skip_setup' in a future release
    if (opts.skipSetup || opts.skip_setup) {
      return PouchPromise$1.resolve();
    }

    // If there is a setup in process or previous successful setup
    // done then we will use that
    // If previous setups have been rejected we will try again
    if (setupPromise) {
      return setupPromise;
    }

    var checkExists = {method: 'GET', url: dbUrl};
    setupPromise = ajaxPromise({}, checkExists).catch(function (err) {
      if (err && err.status && err.status === 404) {
        // Doesnt exist, create it
        res(404, 'PouchDB is just detecting if the remote exists.');
        return ajaxPromise({}, {method: 'PUT', url: dbUrl});
      } else {
        return PouchPromise$1.reject(err);
      }
    }).catch(function (err) {
      // If we try to create a database that already exists, skipped in
      // istanbul since its catching a race condition.
      /* istanbul ignore if */
      if (err && err.status && err.status === 412) {
        return true;
      }
      return PouchPromise$1.reject(err);
    });

    setupPromise.catch(function () {
      setupPromise = null;
    });

    return setupPromise;
  }

  nextTick(function () {
    callback(null, api);
  });

  api.type = function () {
    return 'http';
  };

  api.id = adapterFun$$1('id', function (callback) {
    ajax$$1({}, {method: 'GET', url: genUrl(host, '')}, function (err, result) {
      var uuid$$1 = (result && result.uuid) ?
        (result.uuid + host.db) : genDBUrl(host, '');
      callback(null, uuid$$1);
    });
  });

  api.request = adapterFun$$1('request', function (options, callback) {
    options.url = genDBUrl(host, options.url);
    ajax$$1({}, options, callback);
  });

  // Sends a POST request to the host calling the couchdb _compact function
  //    version: The version of CouchDB it is running
  api.compact = adapterFun$$1('compact', function (opts, callback) {
    if (typeof opts === 'function') {
      callback = opts;
      opts = {};
    }
    opts = clone(opts);
    ajax$$1(opts, {
      url: genDBUrl(host, '_compact'),
      method: 'POST'
    }, function () {
      function ping() {
        api.info(function (err, res$$1) {
          if (res$$1 && !res$$1.compact_running) {
            callback(null, {ok: true});
          } else {
            setTimeout(ping, opts ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.adapters.https"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.</span>https (opts, callback)](#apidoc.element.pouchdb.adapters.https)
- description and source-code
```javascript
function HttpPouch(opts, callback) {

  // The functions that will be publicly available for HttpPouch
  var api = this;

  var host = getHost(opts.name, opts);
  var dbUrl = genDBUrl(host, '');

  opts = clone(opts);
  var ajaxOpts = opts.ajax || {};

  if (opts.auth || host.auth) {
    var nAuth = opts.auth || host.auth;
    var str = nAuth.username + ':' + nAuth.password;
    var token = thisBtoa(unescape(encodeURIComponent(str)));
    ajaxOpts.headers = ajaxOpts.headers || {};
    ajaxOpts.headers.Authorization = 'Basic ' + token;
  }

  // Not strictly necessary, but we do this because numerous tests
  // rely on swapping ajax in and out.
  api._ajax = ajax;

  function ajax$$1(userOpts, options, callback) {
    var reqAjax = userOpts.ajax || {};
    var reqOpts = $inject_Object_assign(clone(ajaxOpts), reqAjax, options);
    var defaultHeaders = clone(ajaxOpts.headers || {});
    reqOpts.headers = $inject_Object_assign(defaultHeaders, reqAjax.headers,
      options.headers || {});
    log$1(reqOpts.method + ' ' + reqOpts.url);
    return api._ajax(reqOpts, callback);
  }

  function ajaxPromise(userOpts, opts) {
    return new PouchPromise$1(function (resolve, reject) {
      ajax$$1(userOpts, opts, function (err, res$$1) {
<span class="apidocCodeCommentSpan">        /* istanbul ignore if */
</span>        if (err) {
          return reject(err);
        }
        resolve(res$$1);
      });
    });
  }

  function adapterFun$$1(name, fun) {
    return adapterFun(name, getArguments(function (args) {
      setup().then(function () {
        return fun.apply(this, args);
      }).catch(function (e) {
        var callback = args.pop();
        callback(e);
      });
    }));
  }

  var setupPromise;

  function setup() {
    // TODO: Remove 'skipSetup' in favor of 'skip_setup' in a future release
    if (opts.skipSetup || opts.skip_setup) {
      return PouchPromise$1.resolve();
    }

    // If there is a setup in process or previous successful setup
    // done then we will use that
    // If previous setups have been rejected we will try again
    if (setupPromise) {
      return setupPromise;
    }

    var checkExists = {method: 'GET', url: dbUrl};
    setupPromise = ajaxPromise({}, checkExists).catch(function (err) {
      if (err && err.status && err.status === 404) {
        // Doesnt exist, create it
        res(404, 'PouchDB is just detecting if the remote exists.');
        return ajaxPromise({}, {method: 'PUT', url: dbUrl});
      } else {
        return PouchPromise$1.reject(err);
      }
    }).catch(function (err) {
      // If we try to create a database that already exists, skipped in
      // istanbul since its catching a race condition.
      /* istanbul ignore if */
      if (err && err.status && err.status === 412) {
        return true;
      }
      return PouchPromise$1.reject(err);
    });

    setupPromise.catch(function () {
      setupPromise = null;
    });

    return setupPromise;
  }

  nextTick(function () {
    callback(null, api);
  });

  api.type = function () {
    return 'http';
  };

  api.id = adapterFun$$1('id', function (callback) {
    ajax$$1({}, {method: 'GET', url: genUrl(host, '')}, function (err, result) {
      var uuid$$1 = (result && result.uuid) ?
        (result.uuid + host.db) : genDBUrl(host, '');
      callback(null, uuid$$1);
    });
  });

  api.request = adapterFun$$1('request', function (options, callback) {
    options.url = genDBUrl(host, options.url);
    ajax$$1({}, options, callback);
  });

  // Sends a POST request to the host calling the couchdb _compact function
  //    version: The version of CouchDB it is running
  api.compact = adapterFun$$1('compact', function (opts, callback) {
    if (typeof opts === 'function') {
      callback = opts;
      opts = {};
    }
    opts = clone(opts);
    ajax$$1(opts, {
      url: genDBUrl(host, '_compact'),
      method: 'POST'
    }, function () {
      function ping() {
        api.info(function (err, res$$1) {
          if (res$$1 && !res$$1.compact_running) {
            callback(null, {ok: true});
          } else {
            setTimeout(ping, opts ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.adapters.leveldb"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.</span>leveldb (opts, callback)](#apidoc.element.pouchdb.adapters.leveldb)
- description and source-code
```javascript
function LevelDownPouch(opts, callback) {

  // Users can pass in their own leveldown alternative here, in which case
  // it overrides the default one. (This is in addition to the custom builds.)
  var leveldown = opts.db;

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (!leveldown) {
    leveldown = requireLeveldown();

    /* istanbul ignore if */
    if (leveldown instanceof Error) {
      return callback(leveldown);
    }
  }

  var _opts = $inject_Object_assign({
    db: leveldown,
    migrate: migrate
  }, opts);

  LevelPouch$1.call(this, _opts, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pouchdb.adapters.http"></a>[module pouchdb.adapters.http](#apidoc.module.pouchdb.adapters.http)

#### <a name="apidoc.element.pouchdb.adapters.http.http"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.</span>http (opts, callback)](#apidoc.element.pouchdb.adapters.http.http)
- description and source-code
```javascript
function HttpPouch(opts, callback) {

  // The functions that will be publicly available for HttpPouch
  var api = this;

  var host = getHost(opts.name, opts);
  var dbUrl = genDBUrl(host, '');

  opts = clone(opts);
  var ajaxOpts = opts.ajax || {};

  if (opts.auth || host.auth) {
    var nAuth = opts.auth || host.auth;
    var str = nAuth.username + ':' + nAuth.password;
    var token = thisBtoa(unescape(encodeURIComponent(str)));
    ajaxOpts.headers = ajaxOpts.headers || {};
    ajaxOpts.headers.Authorization = 'Basic ' + token;
  }

  // Not strictly necessary, but we do this because numerous tests
  // rely on swapping ajax in and out.
  api._ajax = ajax;

  function ajax$$1(userOpts, options, callback) {
    var reqAjax = userOpts.ajax || {};
    var reqOpts = $inject_Object_assign(clone(ajaxOpts), reqAjax, options);
    var defaultHeaders = clone(ajaxOpts.headers || {});
    reqOpts.headers = $inject_Object_assign(defaultHeaders, reqAjax.headers,
      options.headers || {});
    log$1(reqOpts.method + ' ' + reqOpts.url);
    return api._ajax(reqOpts, callback);
  }

  function ajaxPromise(userOpts, opts) {
    return new PouchPromise$1(function (resolve, reject) {
      ajax$$1(userOpts, opts, function (err, res$$1) {
<span class="apidocCodeCommentSpan">        /* istanbul ignore if */
</span>        if (err) {
          return reject(err);
        }
        resolve(res$$1);
      });
    });
  }

  function adapterFun$$1(name, fun) {
    return adapterFun(name, getArguments(function (args) {
      setup().then(function () {
        return fun.apply(this, args);
      }).catch(function (e) {
        var callback = args.pop();
        callback(e);
      });
    }));
  }

  var setupPromise;

  function setup() {
    // TODO: Remove 'skipSetup' in favor of 'skip_setup' in a future release
    if (opts.skipSetup || opts.skip_setup) {
      return PouchPromise$1.resolve();
    }

    // If there is a setup in process or previous successful setup
    // done then we will use that
    // If previous setups have been rejected we will try again
    if (setupPromise) {
      return setupPromise;
    }

    var checkExists = {method: 'GET', url: dbUrl};
    setupPromise = ajaxPromise({}, checkExists).catch(function (err) {
      if (err && err.status && err.status === 404) {
        // Doesnt exist, create it
        res(404, 'PouchDB is just detecting if the remote exists.');
        return ajaxPromise({}, {method: 'PUT', url: dbUrl});
      } else {
        return PouchPromise$1.reject(err);
      }
    }).catch(function (err) {
      // If we try to create a database that already exists, skipped in
      // istanbul since its catching a race condition.
      /* istanbul ignore if */
      if (err && err.status && err.status === 412) {
        return true;
      }
      return PouchPromise$1.reject(err);
    });

    setupPromise.catch(function () {
      setupPromise = null;
    });

    return setupPromise;
  }

  nextTick(function () {
    callback(null, api);
  });

  api.type = function () {
    return 'http';
  };

  api.id = adapterFun$$1('id', function (callback) {
    ajax$$1({}, {method: 'GET', url: genUrl(host, '')}, function (err, result) {
      var uuid$$1 = (result && result.uuid) ?
        (result.uuid + host.db) : genDBUrl(host, '');
      callback(null, uuid$$1);
    });
  });

  api.request = adapterFun$$1('request', function (options, callback) {
    options.url = genDBUrl(host, options.url);
    ajax$$1({}, options, callback);
  });

  // Sends a POST request to the host calling the couchdb _compact function
  //    version: The version of CouchDB it is running
  api.compact = adapterFun$$1('compact', function (opts, callback) {
    if (typeof opts === 'function') {
      callback = opts;
      opts = {};
    }
    opts = clone(opts);
    ajax$$1(opts, {
      url: genDBUrl(host, '_compact'),
      method: 'POST'
    }, function () {
      function ping() {
        api.info(function (err, res$$1) {
          if (res$$1 && !res$$1.compact_running) {
            callback(null, {ok: true});
          } else {
            setTimeout(ping, opts ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.adapters.http.valid"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.http.</span>valid ()](#apidoc.element.pouchdb.adapters.http.valid)
- description and source-code
```javascript
valid = function () {
  return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pouchdb.adapters.leveldb"></a>[module pouchdb.adapters.leveldb](#apidoc.module.pouchdb.adapters.leveldb)

#### <a name="apidoc.element.pouchdb.adapters.leveldb.leveldb"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.</span>leveldb (opts, callback)](#apidoc.element.pouchdb.adapters.leveldb.leveldb)
- description and source-code
```javascript
function LevelDownPouch(opts, callback) {

  // Users can pass in their own leveldown alternative here, in which case
  // it overrides the default one. (This is in addition to the custom builds.)
  var leveldown = opts.db;

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (!leveldown) {
    leveldown = requireLeveldown();

    /* istanbul ignore if */
    if (leveldown instanceof Error) {
      return callback(leveldown);
    }
  }

  var _opts = $inject_Object_assign({
    db: leveldown,
    migrate: migrate
  }, opts);

  LevelPouch$1.call(this, _opts, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.adapters.leveldb.valid"></a>[function <span class="apidocSignatureSpan">pouchdb.adapters.leveldb.</span>valid ()](#apidoc.element.pouchdb.adapters.leveldb.valid)
- description and source-code
```javascript
valid = function () {
  return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pouchdb.debug"></a>[module pouchdb.debug](#apidoc.module.pouchdb.debug)

#### <a name="apidoc.element.pouchdb.debug.debug"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>debug (namespace)](#apidoc.element.pouchdb.debug.debug)
- description and source-code
```javascript
function createDebug(namespace) {

  function debug() {
    // disabled?
    if (!debug.enabled) return;

    var self = debug;

    // set 'diff' timestamp
    var curr = +new Date();
    var ms = curr - (prevTime || curr);
    self.diff = ms;
    self.prev = prevTime;
    self.curr = curr;
    prevTime = curr;

    // turn the 'arguments' into a proper Array
    var args = new Array(arguments.length);
    for (var i = 0; i < args.length; i++) {
      args[i] = arguments[i];
    }

    args[0] = exports.coerce(args[0]);

    if ('string' !== typeof args[0]) {
      // anything else let's inspect with %O
      args.unshift('%O');
    }

    // apply any 'formatters' transformations
    var index = 0;
    args[0] = args[0].replace(/%([a-zA-Z%])/g, function(match, format) {
      // if we encounter an escaped % then don't increase the array index
      if (match === '%%') return match;
      index++;
      var formatter = exports.formatters[format];
      if ('function' === typeof formatter) {
        var val = args[index];
        match = formatter.call(self, val);

        // now we need to remove 'args[index]' since it's inlined in the 'format'
        args.splice(index, 1);
        index--;
      }
      return match;
    });

    // apply env-specific formatting (colors, etc.)
    exports.formatArgs.call(self, args);

    var logFn = debug.log || exports.log || console.log.bind(console);
    logFn.apply(self, args);
  }

  debug.namespace = namespace;
  debug.enabled = exports.enabled(namespace);
  debug.useColors = exports.useColors();
  debug.color = selectColor(namespace);

  // env-specific initialization logic for debug instances
  if ('function' === typeof exports.init) {
    exports.init(debug);
  }

  return debug;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.coerce"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>coerce (val)](#apidoc.element.pouchdb.debug.coerce)
- description and source-code
```javascript
function coerce(val) {
  if (val instanceof Error) return val.stack || val.message;
  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.default"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>default (namespace)](#apidoc.element.pouchdb.debug.default)
- description and source-code
```javascript
function createDebug(namespace) {

  function debug() {
    // disabled?
    if (!debug.enabled) return;

    var self = debug;

    // set 'diff' timestamp
    var curr = +new Date();
    var ms = curr - (prevTime || curr);
    self.diff = ms;
    self.prev = prevTime;
    self.curr = curr;
    prevTime = curr;

    // turn the 'arguments' into a proper Array
    var args = new Array(arguments.length);
    for (var i = 0; i < args.length; i++) {
      args[i] = arguments[i];
    }

    args[0] = exports.coerce(args[0]);

    if ('string' !== typeof args[0]) {
      // anything else let's inspect with %O
      args.unshift('%O');
    }

    // apply any 'formatters' transformations
    var index = 0;
    args[0] = args[0].replace(/%([a-zA-Z%])/g, function(match, format) {
      // if we encounter an escaped % then don't increase the array index
      if (match === '%%') return match;
      index++;
      var formatter = exports.formatters[format];
      if ('function' === typeof formatter) {
        var val = args[index];
        match = formatter.call(self, val);

        // now we need to remove 'args[index]' since it's inlined in the 'format'
        args.splice(index, 1);
        index--;
      }
      return match;
    });

    // apply env-specific formatting (colors, etc.)
    exports.formatArgs.call(self, args);

    var logFn = debug.log || exports.log || console.log.bind(console);
    logFn.apply(self, args);
  }

  debug.namespace = namespace;
  debug.enabled = exports.enabled(namespace);
  debug.useColors = exports.useColors();
  debug.color = selectColor(namespace);

  // env-specific initialization logic for debug instances
  if ('function' === typeof exports.init) {
    exports.init(debug);
  }

  return debug;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.disable"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>disable ()](#apidoc.element.pouchdb.debug.disable)
- description and source-code
```javascript
function disable() {
  exports.enable('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.enable"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>enable (namespaces)](#apidoc.element.pouchdb.debug.enable)
- description and source-code
```javascript
function enable(namespaces) {
  exports.save(namespaces);

  var split = (namespaces || '').split(/[\s,]+/);
  var len = split.length;

  for (var i = 0; i < len; i++) {
    if (!split[i]) continue; // ignore empty strings
    namespaces = split[i].replace(/\*/g, '.*?');
    if (namespaces[0] === '-') {
      exports.skips.push(new RegExp('^' + namespaces.substr(1) + '$'));
    } else {
      exports.names.push(new RegExp('^' + namespaces + '$'));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.enabled"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>enabled (name)](#apidoc.element.pouchdb.debug.enabled)
- description and source-code
```javascript
function enabled(name) {
  var i, len;
  for (i = 0, len = exports.skips.length; i < len; i++) {
    if (exports.skips[i].test(name)) {
      return false;
    }
  }
  for (i = 0, len = exports.names.length; i < len; i++) {
    if (exports.names[i].test(name)) {
      return true;
    }
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.formatArgs"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>formatArgs (args)](#apidoc.element.pouchdb.debug.formatArgs)
- description and source-code
```javascript
function formatArgs(args) {
  var name = this.namespace;
  var useColors = this.useColors;

  if (useColors) {
    var c = this.color;
    var prefix = '  \u001b[3' + c + ';1m' + name + ' ' + '\u001b[0m';

    args[0] = prefix + args[0].split('\n').join('\n' + prefix);
    args.push('\u001b[3' + c + 'm+' + exports.humanize(this.diff) + '\u001b[0m');
  } else {
    args[0] = new Date().toUTCString()
      + ' ' + name + ' ' + args[0];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.humanize"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>humanize (val, options)](#apidoc.element.pouchdb.debug.humanize)
- description and source-code
```javascript
humanize = function (val, options) {
  options = options || {}
  var type = typeof val
  if (type === 'string' && val.length > 0) {
    return parse(val)
  } else if (type === 'number' && isNaN(val) === false) {
    return options.long ?
			fmtLong(val) :
			fmtShort(val)
  }
  throw new Error('val is not a non-empty string or a valid number. val=' + JSON.stringify(val))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.init"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>init (debug)](#apidoc.element.pouchdb.debug.init)
- description and source-code
```javascript
function init(debug) {
  debug.inspectOpts = util._extend({}, exports.inspectOpts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.load"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>load ()](#apidoc.element.pouchdb.debug.load)
- description and source-code
```javascript
function load() {
  return process.env.DEBUG;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.log"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>log ()](#apidoc.element.pouchdb.debug.log)
- description and source-code
```javascript
function log() {
  return stream.write(util.format.apply(util, arguments) + '\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.save"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>save (namespaces)](#apidoc.element.pouchdb.debug.save)
- description and source-code
```javascript
function save(namespaces) {
  if (null == namespaces) {
    // If you set a process.env field to null or undefined, it gets cast to the
    // string 'null' or 'undefined'. Just delete instead.
    delete process.env.DEBUG;
  } else {
    process.env.DEBUG = namespaces;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.useColors"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.</span>useColors ()](#apidoc.element.pouchdb.debug.useColors)
- description and source-code
```javascript
function useColors() {
  return 'colors' in exports.inspectOpts
    ? Boolean(exports.inspectOpts.colors)
    : tty.isatty(fd);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pouchdb.debug.formatters"></a>[module pouchdb.debug.formatters](#apidoc.module.pouchdb.debug.formatters)

#### <a name="apidoc.element.pouchdb.debug.formatters.O"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.formatters.</span>O (v)](#apidoc.element.pouchdb.debug.formatters.O)
- description and source-code
```javascript
O = function (v) {
  this.inspectOpts.colors = this.useColors;
  return util.inspect(v, this.inspectOpts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.debug.formatters.o"></a>[function <span class="apidocSignatureSpan">pouchdb.debug.formatters.</span>o (v)](#apidoc.element.pouchdb.debug.formatters.o)
- description and source-code
```javascript
o = function (v) {
  this.inspectOpts.colors = this.useColors;
  return util.inspect(v, this.inspectOpts)
    .replace(/\s*\n\s*/g, ' ');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pouchdb.super_"></a>[module pouchdb.super_](#apidoc.module.pouchdb.super_)

#### <a name="apidoc.element.pouchdb.super_.super_"></a>[function <span class="apidocSignatureSpan">pouchdb.</span>super_ ()](#apidoc.element.pouchdb.super_.super_)
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



# <a name="apidoc.module.pouchdb.super_.prototype"></a>[module pouchdb.super_.prototype](#apidoc.module.pouchdb.super_.prototype)

#### <a name="apidoc.element.pouchdb.super_.prototype._compact"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>_compact (opts, callback)](#apidoc.element.pouchdb.super_.prototype._compact)
- description and source-code
```javascript
_compact = function (opts, callback) {
  var self = this;
  var changesOpts = {
    return_docs: false,
    last_seq: opts.last_seq || 0
  };
  var promises = [];

  function onChange(row) {
    promises.push(self.compactDocument(row.id, 0));
  }
  function onComplete(resp) {
    var lastSeq = resp.last_seq;
    PouchPromise$1.all(promises).then(function () {
      return upsert(self, '_local/compaction', function deltaFunc(doc) {
        if (!doc.last_seq || doc.last_seq < lastSeq) {
          doc.last_seq = lastSeq;
          return doc;
        }
        return false; // somebody else got here first, don't update
      });
    }).then(function () {
      callback(null, {ok: true});
    }).catch(callback);
  }
  self.changes(changesOpts)
    .on('change', onChange)
    .on('complete', onComplete)
    .on('error', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.allDocs"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>allDocs ()](#apidoc.element.pouchdb.super_.prototype.allDocs)
- description and source-code
```javascript
allDocs = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.bulkDocs"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>bulkDocs ()](#apidoc.element.pouchdb.super_.prototype.bulkDocs)
- description and source-code
```javascript
bulkDocs = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.bulkGet"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>bulkGet ()](#apidoc.element.pouchdb.super_.prototype.bulkGet)
- description and source-code
```javascript
bulkGet = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.changes"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>changes (opts, callback)](#apidoc.element.pouchdb.super_.prototype.changes)
- description and source-code
```javascript
changes = function (opts, callback) {
  if (typeof opts === 'function') {
    callback = opts;
    opts = {};
  }
  return new Changes$2(this, opts, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>close ()](#apidoc.element.pouchdb.super_.prototype.close)
- description and source-code
```javascript
close = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.compact"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>compact ()](#apidoc.element.pouchdb.super_.prototype.compact)
- description and source-code
```javascript
compact = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.compactDocument"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>compactDocument ()](#apidoc.element.pouchdb.super_.prototype.compactDocument)
- description and source-code
```javascript
compactDocument = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.destroy"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>destroy ()](#apidoc.element.pouchdb.super_.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.get"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>get ()](#apidoc.element.pouchdb.super_.prototype.get)
- description and source-code
```javascript
get = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.getAttachment"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>getAttachment ()](#apidoc.element.pouchdb.super_.prototype.getAttachment)
- description and source-code
```javascript
getAttachment = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.id"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>id ()](#apidoc.element.pouchdb.super_.prototype.id)
- description and source-code
```javascript
id = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.info"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>info ()](#apidoc.element.pouchdb.super_.prototype.info)
- description and source-code
```javascript
info = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.post"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>post ()](#apidoc.element.pouchdb.super_.prototype.post)
- description and source-code
```javascript
post = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.put"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>put ()](#apidoc.element.pouchdb.super_.prototype.put)
- description and source-code
```javascript
put = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.putAttachment"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>putAttachment ()](#apidoc.element.pouchdb.super_.prototype.putAttachment)
- description and source-code
```javascript
putAttachment = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.registerDependentDatabase"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>registerDependentDatabase ()](#apidoc.element.pouchdb.super_.prototype.registerDependentDatabase)
- description and source-code
```javascript
registerDependentDatabase = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.remove"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>remove ()](#apidoc.element.pouchdb.super_.prototype.remove)
- description and source-code
```javascript
remove = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.removeAttachment"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>removeAttachment ()](#apidoc.element.pouchdb.super_.prototype.removeAttachment)
- description and source-code
```javascript
removeAttachment = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.revsDiff"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>revsDiff ()](#apidoc.element.pouchdb.super_.prototype.revsDiff)
- description and source-code
```javascript
revsDiff = function () {
  var len = arguments.length;
  if (len) {
    var args = [];
    var i = -1;
    while (++i < len) {
      args[i] = arguments[i];
    }
    return fun.call(this, args);
  } else {
    return fun.call(this, []);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pouchdb.super_.prototype.type"></a>[function <span class="apidocSignatureSpan">pouchdb.super_.prototype.</span>type ()](#apidoc.element.pouchdb.super_.prototype.type)
- description and source-code
```javascript
type = function () {
  return (typeof this._type === 'function') ? this._type() : this.adapter;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
