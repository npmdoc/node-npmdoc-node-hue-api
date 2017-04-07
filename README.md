# api documentation for  [node-hue-api (v2.4.2)](https://github.com/peter-murray/node-hue-api#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-hue-api.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-hue-api) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-hue-api.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-hue-api)
#### Phillips Hue API Library for Node.js

[![NPM](https://nodei.co/npm/node-hue-api.png?downloads=true)](https://www.npmjs.com/package/node-hue-api)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-hue-api/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-hue-api_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-hue-api/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-hue-api/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-hue-api/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Peter Murray",
        "email": "peter.murray@osirisoft.com"
    },
    "bugs": {
        "url": "https://github.com/peter-murray/node-hue-api/issues"
    },
    "contributors": [
        {
            "name": "Peter Murray",
            "email": "peter.murray@osirisoft.com"
        },
        {
            "name": "Ilari Mäkimattila",
            "email": "ilari.makimattila@gmail.com"
        },
        {
            "name": "Bryan Schlief"
        },
        {
            "name": "Sebastian B",
            "url": "SBejga"
        },
        {
            "email": "jon@linesandwaves.com"
        },
        {
            "name": "Knut Sveidqvist"
        }
    ],
    "dependencies": {
        "axios": "~0.15.3",
        "deep-extend": "~0.4.0",
        "q": "~1.4",
        "traits": "~0.4.0",
        "xml2js": "~0.4"
    },
    "description": "Phillips Hue API Library for Node.js",
    "devDependencies": {
        "chai": "~3.5",
        "mocha": "~3.2",
        "semver": "~5.0"
    },
    "directories": {},
    "dist": {
        "shasum": "f721aba415a6c4a8d0b4c2af0ab36939f0ab5cb7",
        "tarball": "https://registry.npmjs.org/node-hue-api/-/node-hue-api-2.4.2.tgz"
    },
    "engines": {
        "node": ">= 4.0.0"
    },
    "gitHead": "96dba498c9cca3e818bef5af31969349993be841",
    "homepage": "https://github.com/peter-murray/node-hue-api#readme",
    "keywords": [
        "philips",
        "hue",
        "api",
        "living",
        "color",
        "colour",
        "automation",
        "light",
        "lighting",
        "bridge"
    ],
    "license": "Apache-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "peter-murray",
            "email": "pmurray@osirisoft.com"
        }
    ],
    "name": "node-hue-api",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/peter-murray/node-hue-api.git"
    },
    "scripts": {
        "test": "mocha test"
    },
    "version": "2.4.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-hue-api](#apidoc.module.node-hue-api)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>ApiError (error)](#apidoc.element.node-hue-api.ApiError)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>ApiError.super_ (msg, constr)](#apidoc.element.node-hue-api.ApiError.super_)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>BridgeApi (host, username, timeout, port)](#apidoc.element.node-hue-api.BridgeApi)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>HueApi (host, username, timeout, port)](#apidoc.element.node-hue-api.HueApi)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>api (host, username, timeout, port)](#apidoc.element.node-hue-api.api)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>connect (config)](#apidoc.element.node-hue-api.connect)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>locateBridges ()](#apidoc.element.node-hue-api.locateBridges)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>nupnpSearch (cb)](#apidoc.element.node-hue-api.nupnpSearch)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>searchForBridges ()](#apidoc.element.node-hue-api.searchForBridges)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>upnpSearch (timeout)](#apidoc.element.node-hue-api.upnpSearch)
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>bridge_discovery
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>errors
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>httpPromise
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>lightState
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>rgb
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>scene
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>scheduledEvent
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>search
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>timer
1.  object <span class="apidocSignatureSpan">node-hue-api.</span>utils

#### [module node-hue-api.ApiError](#apidoc.module.node-hue-api.ApiError)
1.  [function <span class="apidocSignatureSpan">node-hue-api.</span>ApiError (error)](#apidoc.element.node-hue-api.ApiError.ApiError)
1.  [function <span class="apidocSignatureSpan">node-hue-api.ApiError.</span>super_ (msg, constr)](#apidoc.element.node-hue-api.ApiError.super_)

#### [module node-hue-api.ApiError.super_](#apidoc.module.node-hue-api.ApiError.super_)
1.  [function <span class="apidocSignatureSpan">node-hue-api.ApiError.</span>super_ ()](#apidoc.element.node-hue-api.ApiError.super_.super_)

#### [module node-hue-api.bridge_discovery](#apidoc.module.node-hue-api.bridge_discovery)
1.  [function <span class="apidocSignatureSpan">node-hue-api.bridge_discovery.</span>description (host)](#apidoc.element.node-hue-api.bridge_discovery.description)
1.  [function <span class="apidocSignatureSpan">node-hue-api.bridge_discovery.</span>locateBridges (cb)](#apidoc.element.node-hue-api.bridge_discovery.locateBridges)
1.  [function <span class="apidocSignatureSpan">node-hue-api.bridge_discovery.</span>networkSearch (timeout)](#apidoc.element.node-hue-api.bridge_discovery.networkSearch)

#### [module node-hue-api.errors](#apidoc.module.node-hue-api.errors)
1.  [function <span class="apidocSignatureSpan">node-hue-api.errors.</span>ApiError (error)](#apidoc.element.node-hue-api.errors.ApiError)

#### [module node-hue-api.httpPromise](#apidoc.module.node-hue-api.httpPromise)
1.  [function <span class="apidocSignatureSpan">node-hue-api.httpPromise.</span>invoke (command, parameters)](#apidoc.element.node-hue-api.httpPromise.invoke)
1.  [function <span class="apidocSignatureSpan">node-hue-api.httpPromise.</span>simpleGet (uri)](#apidoc.element.node-hue-api.httpPromise.simpleGet)

#### [module node-hue-api.lightState](#apidoc.module.node-hue-api.lightState)
1.  [function <span class="apidocSignatureSpan">node-hue-api.lightState.</span>create (values)](#apidoc.element.node-hue-api.lightState.create)
1.  [function <span class="apidocSignatureSpan">node-hue-api.lightState.</span>isLightState (obj)](#apidoc.element.node-hue-api.lightState.isLightState)

#### [module node-hue-api.rgb](#apidoc.module.node-hue-api.rgb)
1.  [function <span class="apidocSignatureSpan">node-hue-api.rgb.</span>convertRGBtoXY (rgb, modelid)](#apidoc.element.node-hue-api.rgb.convertRGBtoXY)
1.  [function <span class="apidocSignatureSpan">node-hue-api.rgb.</span>convertXYtoRGB (x, y, brightness)](#apidoc.element.node-hue-api.rgb.convertXYtoRGB)

#### [module node-hue-api.scene](#apidoc.module.node-hue-api.scene)
1.  [function <span class="apidocSignatureSpan">node-hue-api.scene.</span>create ()](#apidoc.element.node-hue-api.scene.create)

#### [module node-hue-api.scheduledEvent](#apidoc.module.node-hue-api.scheduledEvent)
1.  [function <span class="apidocSignatureSpan">node-hue-api.scheduledEvent.</span>create ()](#apidoc.element.node-hue-api.scheduledEvent.create)

#### [module node-hue-api.search](#apidoc.module.node-hue-api.search)
1.  [function <span class="apidocSignatureSpan">node-hue-api.search.</span>locateBridges (timeout)](#apidoc.element.node-hue-api.search.locateBridges)

#### [module node-hue-api.timer](#apidoc.module.node-hue-api.timer)
1.  [function <span class="apidocSignatureSpan">node-hue-api.timer.</span>create ()](#apidoc.element.node-hue-api.timer.create)

#### [module node-hue-api.utils](#apidoc.module.node-hue-api.utils)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>combine (obj, values)](#apidoc.element.node-hue-api.utils.combine)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>createStringValueArray (values)](#apidoc.element.node-hue-api.utils.createStringValueArray)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>getStringValue (value, maxLength)](#apidoc.element.node-hue-api.utils.getStringValue)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>isFunction (object)](#apidoc.element.node-hue-api.utils.isFunction)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>parseErrors (results)](#apidoc.element.node-hue-api.utils.parseErrors)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>promiseOrCallback (promise, cb)](#apidoc.element.node-hue-api.utils.promiseOrCallback)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>resolvePromise (promise, callback)](#apidoc.element.node-hue-api.utils.resolvePromise)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>valueForType (type, value)](#apidoc.element.node-hue-api.utils.valueForType)
1.  [function <span class="apidocSignatureSpan">node-hue-api.utils.</span>wasSuccessful (result)](#apidoc.element.node-hue-api.utils.wasSuccessful)



# <a name="apidoc.module.node-hue-api"></a>[module node-hue-api](#apidoc.module.node-hue-api)

#### <a name="apidoc.element.node-hue-api.ApiError"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>ApiError (error)](#apidoc.element.node-hue-api.ApiError)
- description and source-code
```javascript
ApiError = function (error) {
    var errorMessage,
        type;

    if (typeof(error) === 'string') {
        errorMessage = error;
        type = 0;
    } else {
        errorMessage = error.message || error.description;
        type = error.type;
    }

    ApiError.super_.call(this, errorMessage, this.constructor);
    this.type = type;

    if (error.address) {
        this.address = error.address;
    }
}
```
- example usage
```shell
...

options.timeout = parameters.timeout || 10000;
options.method = command.method || "GET";

if (command.getPath) {
  urlObj.pathname = command.getPath(parameters);
} else {
  throw new errors.ApiError("Cannot get the path to invoke from the command");
}
options.url = url.format(urlObj);

// Check if the command has body arguments and process them accordingly
if (command.bodyArguments && command.buildRequestBody) {
  body = command.buildRequestBody(parameters.values);
...
```

#### <a name="apidoc.element.node-hue-api.ApiError.super_"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>ApiError.super_ (msg, constr)](#apidoc.element.node-hue-api.ApiError.super_)
- description and source-code
```javascript
ApiError.super_ = function (msg, constr) {
    // If defined, pass the constr property to V8's captureStackTrace to clean up the output
    Error.captureStackTrace(this, constr || this);

    // If defined, store a custom error message
    this.message = msg || "Error";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.BridgeApi"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>BridgeApi (host, username, timeout, port)](#apidoc.element.node-hue-api.BridgeApi)
- description and source-code
```javascript
BridgeApi = function (host, username, timeout, port) {
    var config = {
        hostname: host,
        username: username,
        timeout: timeout || 10000,
        port: port || 80
    };

    return new HueApi(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.HueApi"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>HueApi (host, username, timeout, port)](#apidoc.element.node-hue-api.HueApi)
- description and source-code
```javascript
HueApi = function (host, username, timeout, port) {
    var config = {
        hostname: host,
        username: username,
        timeout: timeout || 10000,
        port: port || 80
    };

    return new HueApi(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.api"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>api (host, username, timeout, port)](#apidoc.element.node-hue-api.api)
- description and source-code
```javascript
api = function (host, username, timeout, port) {
    var config = {
        hostname: host,
        username: username,
        timeout: timeout || 10000,
        port: port || 80
    };

    return new HueApi(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.connect"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>connect (config)](#apidoc.element.node-hue-api.connect)
- description and source-code
```javascript
connect = function (config) {
    return new Hue(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.locateBridges"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>locateBridges ()](#apidoc.element.node-hue-api.locateBridges)
- description and source-code
```javascript
locateBridges = function () {
    var args = Array.prototype.slice.call(arguments);
    console.error(message);
    return fn.apply(this, args);
}
```
- example usage
```shell
...
* may need to be adjusted to locate the Hue Bridge.
*
* @param timeout The maximum time to wait for Hue Devices to be located. If not specified will use the default of 5
* seconds.
* @return A promise that will resolve the Hue Bridges as an Array of {"id": {String}, "ipaddress": {String}} objects.
*/
module.exports.networkSearch = function (timeout) {
   return search.locateBridges(timeout).then(_identifyBridges);
};

/**
* Uses the http://www.meethue.com/api/nupnp call to search for any bridges locally on the network. This lookup can be
* significantly faster than issuing search requests in the {locateBridges} function.
*
* @param cb An option callback function that will be informed of results.
...
```

#### <a name="apidoc.element.node-hue-api.nupnpSearch"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>nupnpSearch (cb)](#apidoc.element.node-hue-api.nupnpSearch)
- description and source-code
```javascript
nupnpSearch = function (cb) {
    var promise = http.invoke(discovery.upnpLookup, {host: "www.meethue.com", ssl: true});
    return utils.promiseOrCallback(promise, cb);
}
```
- example usage
```shell
...

var displayBridges = function(bridge) {
	console.log("Hue Bridges Found: " + JSON.stringify(bridge));
};

// --------------------------
// Using a promise
hue.nupnpSearch().then(displayBridges).done();

// --------------------------
// Using a callback
hue.nupnpSearch(function(err, result) {
	if (err) throw err;
	displayBridges(result);
});
...
```

#### <a name="apidoc.element.node-hue-api.searchForBridges"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>searchForBridges ()](#apidoc.element.node-hue-api.searchForBridges)
- description and source-code
```javascript
searchForBridges = function () {
    var args = Array.prototype.slice.call(arguments);
    console.error(message);
    return fn.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.upnpSearch"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>upnpSearch (timeout)](#apidoc.element.node-hue-api.upnpSearch)
- description and source-code
```javascript
upnpSearch = function (timeout) {
    return search.locateBridges(timeout).then(_identifyBridges);
}
```
- example usage
```shell
...
var hue = require("node-hue-api"),
	timeout = 2000; // 2 seconds

var displayBridges = function(bridge) {
	console.log("Hue Bridges Found: " + JSON.stringify(bridge));
};

hue.upnpSearch(timeout).then(displayBridges).done();
'''
A timeout can be provided to the function to increase/decrease the amount of time that it waits for responses from the
search request, by default this is set to 5 seconds (the above example sets this to 2 seconds).

The results from this function call will be of the form;
'''
Hue Bridges Found: [{"id":"001788096103","ipaddress":"192.168.2.129"}]
...
```



# <a name="apidoc.module.node-hue-api.ApiError"></a>[module node-hue-api.ApiError](#apidoc.module.node-hue-api.ApiError)

#### <a name="apidoc.element.node-hue-api.ApiError.ApiError"></a>[function <span class="apidocSignatureSpan">node-hue-api.</span>ApiError (error)](#apidoc.element.node-hue-api.ApiError.ApiError)
- description and source-code
```javascript
ApiError = function (error) {
    var errorMessage,
        type;

    if (typeof(error) === 'string') {
        errorMessage = error;
        type = 0;
    } else {
        errorMessage = error.message || error.description;
        type = error.type;
    }

    ApiError.super_.call(this, errorMessage, this.constructor);
    this.type = type;

    if (error.address) {
        this.address = error.address;
    }
}
```
- example usage
```shell
...

options.timeout = parameters.timeout || 10000;
options.method = command.method || "GET";

if (command.getPath) {
  urlObj.pathname = command.getPath(parameters);
} else {
  throw new errors.ApiError("Cannot get the path to invoke from the command");
}
options.url = url.format(urlObj);

// Check if the command has body arguments and process them accordingly
if (command.bodyArguments && command.buildRequestBody) {
  body = command.buildRequestBody(parameters.values);
...
```

#### <a name="apidoc.element.node-hue-api.ApiError.super_"></a>[function <span class="apidocSignatureSpan">node-hue-api.ApiError.</span>super_ (msg, constr)](#apidoc.element.node-hue-api.ApiError.super_)
- description and source-code
```javascript
super_ = function (msg, constr) {
    // If defined, pass the constr property to V8's captureStackTrace to clean up the output
    Error.captureStackTrace(this, constr || this);

    // If defined, store a custom error message
    this.message = msg || "Error";
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-hue-api.ApiError.super_"></a>[module node-hue-api.ApiError.super_](#apidoc.module.node-hue-api.ApiError.super_)

#### <a name="apidoc.element.node-hue-api.ApiError.super_.super_"></a>[function <span class="apidocSignatureSpan">node-hue-api.ApiError.</span>super_ ()](#apidoc.element.node-hue-api.ApiError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-hue-api.bridge_discovery"></a>[module node-hue-api.bridge_discovery](#apidoc.module.node-hue-api.bridge_discovery)

#### <a name="apidoc.element.node-hue-api.bridge_discovery.description"></a>[function <span class="apidocSignatureSpan">node-hue-api.bridge_discovery.</span>description (host)](#apidoc.element.node-hue-api.bridge_discovery.description)
- description and source-code
```javascript
description = function (host) {
    return http.invoke(discovery.description, {"host": host})
        .then(_parseDescription);
}
```
- example usage
```shell
...
username = "08a902b95915cdd9b75547cb50892dc4",
api;

api = new HueApi(hostname, username);

// --------------------------
// Using a promise
api.description().then(displayResult).done();
// using alias getDescription()
api.getDescription().then(displayResult).done();

// --------------------------
// Using a callback
api.description(function(err, config) {
if (err) throw err;
...
```

#### <a name="apidoc.element.node-hue-api.bridge_discovery.locateBridges"></a>[function <span class="apidocSignatureSpan">node-hue-api.bridge_discovery.</span>locateBridges (cb)](#apidoc.element.node-hue-api.bridge_discovery.locateBridges)
- description and source-code
```javascript
locateBridges = function (cb) {
    var promise = http.invoke(discovery.upnpLookup, {host: "www.meethue.com", ssl: true});
    return utils.promiseOrCallback(promise, cb);
}
```
- example usage
```shell
...
* may need to be adjusted to locate the Hue Bridge.
*
* @param timeout The maximum time to wait for Hue Devices to be located. If not specified will use the default of 5
* seconds.
* @return A promise that will resolve the Hue Bridges as an Array of {"id": {String}, "ipaddress": {String}} objects.
*/
module.exports.networkSearch = function (timeout) {
   return search.locateBridges(timeout).then(_identifyBridges);
};

/**
* Uses the http://www.meethue.com/api/nupnp call to search for any bridges locally on the network. This lookup can be
* significantly faster than issuing search requests in the {locateBridges} function.
*
* @param cb An option callback function that will be informed of results.
...
```

#### <a name="apidoc.element.node-hue-api.bridge_discovery.networkSearch"></a>[function <span class="apidocSignatureSpan">node-hue-api.bridge_discovery.</span>networkSearch (timeout)](#apidoc.element.node-hue-api.bridge_discovery.networkSearch)
- description and source-code
```javascript
networkSearch = function (timeout) {
    return search.locateBridges(timeout).then(_identifyBridges);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-hue-api.errors"></a>[module node-hue-api.errors](#apidoc.module.node-hue-api.errors)

#### <a name="apidoc.element.node-hue-api.errors.ApiError"></a>[function <span class="apidocSignatureSpan">node-hue-api.errors.</span>ApiError (error)](#apidoc.element.node-hue-api.errors.ApiError)
- description and source-code
```javascript
ApiError = function (error) {
    var errorMessage,
        type;

    if (typeof(error) === 'string') {
        errorMessage = error;
        type = 0;
    } else {
        errorMessage = error.message || error.description;
        type = error.type;
    }

    ApiError.super_.call(this, errorMessage, this.constructor);
    this.type = type;

    if (error.address) {
        this.address = error.address;
    }
}
```
- example usage
```shell
...

options.timeout = parameters.timeout || 10000;
options.method = command.method || "GET";

if (command.getPath) {
  urlObj.pathname = command.getPath(parameters);
} else {
  throw new errors.ApiError("Cannot get the path to invoke from the command");
}
options.url = url.format(urlObj);

// Check if the command has body arguments and process them accordingly
if (command.bodyArguments && command.buildRequestBody) {
  body = command.buildRequestBody(parameters.values);
...
```



# <a name="apidoc.module.node-hue-api.httpPromise"></a>[module node-hue-api.httpPromise](#apidoc.module.node-hue-api.httpPromise)

#### <a name="apidoc.element.node-hue-api.httpPromise.invoke"></a>[function <span class="apidocSignatureSpan">node-hue-api.httpPromise.</span>invoke (command, parameters)](#apidoc.element.node-hue-api.httpPromise.invoke)
- description and source-code
```javascript
invoke = function (command, parameters) {
  var options = buildOptions(command, parameters)
    , promise
    ;

  //promise = requestUtil.request(options);
  promise = wrapAxios(axios(options));

  if (command.statusCodeMap) {
    promise = promise.then(generateErrorsIfMatched(command.statusCodeMap));
  }

  promise = promise
    .then(requireStatusCode200)
    .then(function (requestResult) {
      var result;

      if (options.headers.Accept === "application/json") {
        result = checkForError(requestResult);
      } else {
        result = requestResult.data;
      }
      return result;
    });

  if (command.postProcessing) {
    command.postProcessing.forEach(function (fn) {
      promise = promise.then(fn);
    });
  }

  return promise;
}
```
- example usage
```shell
...
* Uses the http://www.meethue.com/api/nupnp call to search for any bridges locally on the network. This lookup can be
* significantly faster than issuing search requests in the {locateBridges} function.
*
* @param cb An option callback function that will be informed of results.
* @returns {Q.promise} A promise that will resolve the addresses of the bridges, or {null} if a callback was provided.
*/
module.exports.locateBridges = function (cb) {
   var promise = http.invoke(discovery.upnpLookup, {host: "www.meethue.com", ssl: true});
   return utils.promiseOrCallback(promise, cb);
};

/**
* Obtains an object representation of the Description XML.
*
* @param host The host to get the description XML from.
...
```

#### <a name="apidoc.element.node-hue-api.httpPromise.simpleGet"></a>[function <span class="apidocSignatureSpan">node-hue-api.httpPromise.</span>simpleGet (uri)](#apidoc.element.node-hue-api.httpPromise.simpleGet)
- description and source-code
```javascript
simpleGet = function (uri) {
  return wrapAxios(axios.get(uri, defaultOptions))
      .then(requireStatusCode200)
      .then(function(result) {
          return result.data;
      });
}
```
- example usage
```shell
...

/**
 * Performs a GET on the provided path, the location response from the bridge.
 * This function expects there to be an XML description document present at the provided path.
 * @param path The path in the LOCATION response from SSDP lookup.
 */
function followLocationResponse(path) {
    return http.simpleGet(path)
        .then(_parseDescription)
        .fail(function (err) {
            // Do nothing with services that do not respond with an XML document
        })
        ;
}
...
```



# <a name="apidoc.module.node-hue-api.lightState"></a>[module node-hue-api.lightState](#apidoc.module.node-hue-api.lightState)

#### <a name="apidoc.element.node-hue-api.lightState.create"></a>[function <span class="apidocSignatureSpan">node-hue-api.lightState.</span>create (values)](#apidoc.element.node-hue-api.lightState.create)
- description and source-code
```javascript
create = function (values) {
    var state = new State();

    // If values are provided then load the ones that have values to match our functions
    if (values) {
        Object.keys(values).forEach(function (value) {
            var fn;

            if (values.hasOwnProperty(value)) {
                fn = state[value];

                if (utils.isFunction(fn)) {
                    fn.apply(state, [values[value]]);
                }
            }
        });
    }

    return state;
}
```
- example usage
```shell
...

var host = "192.168.2.129",
username = "08a902b95915cdd9b75547cb50892dc4",
api = new HueApi(host, username),
state;

// Set light state to 'on' with warm white value of 500 and brightness set to 100%
state = lightState.create().on().white(500, 100);

// --------------------------
// Using a promise
api.setLightState(5, state)
.then(displayResult)
.done();
...
```

#### <a name="apidoc.element.node-hue-api.lightState.isLightState"></a>[function <span class="apidocSignatureSpan">node-hue-api.lightState.</span>isLightState (obj)](#apidoc.element.node-hue-api.lightState.isLightState)
- description and source-code
```javascript
isLightState = function (obj) {
    return obj && obj instanceof State;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-hue-api.rgb"></a>[module node-hue-api.rgb](#apidoc.module.node-hue-api.rgb)

#### <a name="apidoc.element.node-hue-api.rgb.convertRGBtoXY"></a>[function <span class="apidocSignatureSpan">node-hue-api.rgb.</span>convertRGBtoXY (rgb, modelid)](#apidoc.element.node-hue-api.rgb.convertRGBtoXY)
- description and source-code
```javascript
convertRGBtoXY = function (rgb, modelid) {
    var limits = _getLimits(modelid);
    return _getXYStateFromRGB(rgb[0], rgb[1], rgb[2], limits);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.rgb.convertXYtoRGB"></a>[function <span class="apidocSignatureSpan">node-hue-api.rgb.</span>convertXYtoRGB (x, y, brightness)](#apidoc.element.node-hue-api.rgb.convertXYtoRGB)
- description and source-code
```javascript
function _getRGBFromXYState(x, y, brightness) {
    var Y = brightness
      , X = (Y / y) * x
      , Z = (Y / y) * (1 - x - y)
      , rgb =  [
          X * 1.612 - Y * 0.203 - Z * 0.302,
          -X * 0.509 + Y * 1.412 + Z * 0.066,
          X * 0.026 - Y * 0.072 + Z * 0.962
      ]
      ;

    // Apply reverse gamma correction.
    rgb = rgb.map(function (x) {
        return (x <= 0.0031308) ? (12.92 * x) : ((1.0 + 0.055) * Math.pow(x, (1.0 / 2.4)) - 0.055);
    });

    // Bring all negative components to zero.
    rgb = rgb.map(function (x) { return Math.max(0, x); });

    // If one component is greater than 1, weight components by that value.
    var max = Math.max(rgb[0], rgb[1], rgb[2]);
    if (max > 1) {
        rgb = rgb.map(function (x) { return x / max; });
    }

    rgb = rgb.map(function (x) { return Math.floor(x * 255); });

    return rgb;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-hue-api.scene"></a>[module node-hue-api.scene](#apidoc.module.node-hue-api.scene)

#### <a name="apidoc.element.node-hue-api.scene.create"></a>[function <span class="apidocSignatureSpan">node-hue-api.scene.</span>create ()](#apidoc.element.node-hue-api.scene.create)
- description and source-code
```javascript
create = function () {
  var scene
    , arg
    ;

  if (arguments.length == 0) {
    scene = new Scene();
  } else {
    arg = arguments[0];

    if (arg instanceof Scene) {
      scene = arg;
    } else {
      scene = new Scene();

      // try to populate the new scene using any values that match scene properties
      if (arg.name) {
        scene.withName(arg.name);
      }

      if (arg.lights) {
        scene.withLights(arg.lights);
      }

      if (arg.transitionTime) {
        scene.withTransitionTime(arg.transitionTime);
      }

      if (arg.data || arg.appData) {
        scene.withAppData(arg.data || arg.appData);
      }

      if (arg.picture) {
        scene.withPicture(arg.picture);
      }
    }
  }
  return scene;
}
```
- example usage
```shell
...

var host = "192.168.2.129",
username = "08a902b95915cdd9b75547cb50892dc4",
api = new HueApi(host, username),
state;

// Set light state to 'on' with warm white value of 500 and brightness set to 100%
state = lightState.create().on().white(500, 100);

// --------------------------
// Using a promise
api.setLightState(5, state)
.then(displayResult)
.done();
...
```



# <a name="apidoc.module.node-hue-api.scheduledEvent"></a>[module node-hue-api.scheduledEvent](#apidoc.module.node-hue-api.scheduledEvent)

#### <a name="apidoc.element.node-hue-api.scheduledEvent.create"></a>[function <span class="apidocSignatureSpan">node-hue-api.scheduledEvent.</span>create ()](#apidoc.element.node-hue-api.scheduledEvent.create)
- description and source-code
```javascript
create = function () {
  var schedule,
    arg;

  if (arguments.length == 0) {
    schedule = new Schedule();
  } else {
    arg = arguments[0];
    if (arg instanceof Schedule) {
      schedule = arg;
    } else {
      schedule = new Schedule();

      // try to populate the new schedule using any values that match schedule properties
      if (arg.name) {
        schedule.withName(arg.name);
      }

      if (arg.description) {
        schedule.withDescription(arg.description);
      }

      if (arg.time || arg.localtime) {
        schedule.at(arg.time || arg.localtime);
      }

      if (arg.command) {
        schedule.withCommand(arg.command);
      }

      if (arg.status) {
        schedule.withEnabledState(arg.status);
      }
    }
  }

  return schedule;
}
```
- example usage
```shell
...

var host = "192.168.2.129",
username = "08a902b95915cdd9b75547cb50892dc4",
api = new HueApi(host, username),
state;

// Set light state to 'on' with warm white value of 500 and brightness set to 100%
state = lightState.create().on().white(500, 100);

// --------------------------
// Using a promise
api.setLightState(5, state)
.then(displayResult)
.done();
...
```



# <a name="apidoc.module.node-hue-api.search"></a>[module node-hue-api.search](#apidoc.module.node-hue-api.search)

#### <a name="apidoc.element.node-hue-api.search.locateBridges"></a>[function <span class="apidocSignatureSpan">node-hue-api.search.</span>locateBridges (timeout)](#apidoc.element.node-hue-api.search.locateBridges)
- description and source-code
```javascript
function locateBridges(timeout) {
    var deferred = Q.defer(),
        search = new SSDPSearch(timeout),
        results = [];

    search.on("response", function(value) {
        results.push(value);
    });
    search.search();

    // Give up after the timeout and process whatever results we have
    setTimeout(function() {
        _close(search);
        deferred.resolve(_filterResults(results));
    }, timeout || 5000);

    return deferred.promise;
}
```
- example usage
```shell
...
* may need to be adjusted to locate the Hue Bridge.
*
* @param timeout The maximum time to wait for Hue Devices to be located. If not specified will use the default of 5
* seconds.
* @return A promise that will resolve the Hue Bridges as an Array of {"id": {String}, "ipaddress": {String}} objects.
*/
module.exports.networkSearch = function (timeout) {
   return search.locateBridges(timeout).then(_identifyBridges);
};

/**
* Uses the http://www.meethue.com/api/nupnp call to search for any bridges locally on the network. This lookup can be
* significantly faster than issuing search requests in the {locateBridges} function.
*
* @param cb An option callback function that will be informed of results.
...
```



# <a name="apidoc.module.node-hue-api.timer"></a>[module node-hue-api.timer](#apidoc.module.node-hue-api.timer)

#### <a name="apidoc.element.node-hue-api.timer.create"></a>[function <span class="apidocSignatureSpan">node-hue-api.timer.</span>create ()](#apidoc.element.node-hue-api.timer.create)
- description and source-code
```javascript
create = function () {
  return new Timer();
}
```
- example usage
```shell
...

var host = "192.168.2.129",
username = "08a902b95915cdd9b75547cb50892dc4",
api = new HueApi(host, username),
state;

// Set light state to 'on' with warm white value of 500 and brightness set to 100%
state = lightState.create().on().white(500, 100);

// --------------------------
// Using a promise
api.setLightState(5, state)
.then(displayResult)
.done();
...
```



# <a name="apidoc.module.node-hue-api.utils"></a>[module node-hue-api.utils](#apidoc.module.node-hue-api.utils)

#### <a name="apidoc.element.node-hue-api.utils.combine"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>combine (obj, values)](#apidoc.element.node-hue-api.utils.combine)
- description and source-code
```javascript
combine = function (obj, values) {
    var argIdx = 1,
        value,
        property;

    while (argIdx < arguments.length) {
        value = arguments[argIdx];
        for (property in value) {
            if (value.hasOwnProperty(property)) {
                obj[property] = value[property];
            }
        }
        argIdx++;
    }

    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.utils.createStringValueArray"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>createStringValueArray (values)](#apidoc.element.node-hue-api.utils.createStringValueArray)
- description and source-code
```javascript
createStringValueArray = function (values) {
    var result = [];

    if (Array.isArray(values)) {
        values.forEach(function (value) {
            result.push(_asStringValue(value));
        });
    } else {
        result.push(_asStringValue(values));
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.utils.getStringValue"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>getStringValue (value, maxLength)](#apidoc.element.node-hue-api.utils.getStringValue)
- description and source-code
```javascript
getStringValue = function (value, maxLength) {
    var result = value || "";

    if (maxLength && result.length > maxLength) {
        result = result.substr(0, maxLength);
    }
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.utils.isFunction"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>isFunction (object)](#apidoc.element.node-hue-api.utils.isFunction)
- description and source-code
```javascript
isFunction = function (object) {
    var getClass = {}.toString;

    return object && getClass.call(object) === '[object Function]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.utils.parseErrors"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>parseErrors (results)](#apidoc.element.node-hue-api.utils.parseErrors)
- description and source-code
```javascript
parseErrors = function (results) {
    var errors = [];

    if (util.isArray(results)) {
        results.forEach(function (result) {
            if (result.error) {
                errors.push(result.error);
            }
        });
    } else {
        if (results.error) {
            errors.push(results.error);
        } else {
            //TODO this should not occur
            console.log("UNPARSED");
            console.log(results);
        }
    }

    //TODO actually find the error messages
    return errors;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.utils.promiseOrCallback"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>promiseOrCallback (promise, cb)](#apidoc.element.node-hue-api.utils.promiseOrCallback)
- description and source-code
```javascript
promiseOrCallback = function (promise, cb) {
    var promiseResult = promise;

    if (cb && typeof cb === "function") {
        module.exports.resolvePromise(promise, cb);
        // Do not return the promise, as the callbacks will have forced it to resolve
        promiseResult = null;
    }

    return promiseResult;
}
```
- example usage
```shell
...
* significantly faster than issuing search requests in the {locateBridges} function.
*
* @param cb An option callback function that will be informed of results.
* @returns {Q.promise} A promise that will resolve the addresses of the bridges, or {null} if a callback was provided.
*/
module.exports.locateBridges = function (cb) {
   var promise = http.invoke(discovery.upnpLookup, {host: "www.meethue.com", ssl: true});
   return utils.promiseOrCallback(promise, cb);
};

/**
* Obtains an object representation of the Description XML.
*
* @param host The host to get the description XML from.
* @return {*} The object representing some of the values in the description XML.
...
```

#### <a name="apidoc.element.node-hue-api.utils.resolvePromise"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>resolvePromise (promise, callback)](#apidoc.element.node-hue-api.utils.resolvePromise)
- description and source-code
```javascript
resolvePromise = function (promise, callback) {
    function resolveValue(value) {
        if (callback) {
            callback(null, value);
        }
    }

    function resolveError(err) {
        if (callback) {
            callback(err, null);
        }
    }

    promise.then(resolveValue).catch(resolveError);
}
```
- example usage
```shell
...
 * @param cb The callback function, which is optional
 * @returns {*} The promise if there is not a valid callback, or null, if the callback is used to resolve the promise.
 */
module.exports.promiseOrCallback = function (promise, cb) {
    var promiseResult = promise;

    if (cb && typeof cb === "function") {
        module.exports.resolvePromise(promise, cb);
        // Do not return the promise, as the callbacks will have forced it to resolve
        promiseResult = null;
    }

    return promiseResult;
};
...
```

#### <a name="apidoc.element.node-hue-api.utils.valueForType"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>valueForType (type, value)](#apidoc.element.node-hue-api.utils.valueForType)
- description and source-code
```javascript
valueForType = function (type, value) {
    var result;

    if (type === "bool") {
        result = Boolean(value);
    } else if (type === "uint8" || type === "uint16" || type === "int8" || type === "int16") {
        result = Math.floor(value);

        if (/^uint.*/.test(type) && result < 0) {
            result = 0;
        }
    } else if (type === "string") {
        result = String(value);
    } else if (type === "float") {
        result = Number(value);
    } else if (type === "list") {
        result = util.isArray(value) ? value : [];
    } else {
        result = value;
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-hue-api.utils.wasSuccessful"></a>[function <span class="apidocSignatureSpan">node-hue-api.utils.</span>wasSuccessful (result)](#apidoc.element.node-hue-api.utils.wasSuccessful)
- description and source-code
```javascript
wasSuccessful = function (result) {
    var success = true,
        idx,
        len;

    if (util.isArray(result)) {
        for (idx = 0, len = result.length; idx < len; idx++) {
            success = success && module.exports.wasSuccessful(result[idx]);
        }
    } else {
        success = result.success !== 'undefined';
    }
    return success;
}
```
- example usage
```shell
...
module.exports.wasSuccessful = function (result) {
    var success = true,
        idx,
        len;

    if (util.isArray(result)) {
        for (idx = 0, len = result.length; idx < len; idx++) {
            success = success && module.exports.wasSuccessful(result[idx]);
        }
    } else {
        success = result.success !== 'undefined';
    }
    return success;
};
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
