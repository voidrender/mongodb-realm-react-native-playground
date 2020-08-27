# realm-v10.0.0-beta.10-pods-error
An example to reproduce a pod install error in realm/realm-js@10.0.0-beta.10.

## Getting Started
Using node@12 or newer, install dependencies with yarn:

```
yarn
```

Next, install iOS dependencies:

```
cd ios && pod install
```

Observe an error installing pods.

```
Installing RealmJS (10.0.0-beta.10)
[!] /bin/bash -c 
set -e
./scripts/xcode-download-realm.sh ./scripts

internal/modules/cjs/loader.js:584
    throw err;
    ^

Error: Cannot find module '/Users/you/realm-v10.0.0-beta.10-pods-error/node_modules/realm/scripts/scripts/download-realm.js'
    at Function.Module._resolveFilename (internal/modules/cjs/loader.js:582:15)
    at Function.Module._load (internal/modules/cjs/loader.js:508:25)
    at Function.Module.runMain (internal/modules/cjs/loader.js:754:12)
    at startup (internal/bootstrap/node.js:283:19)
    at bootstrapNodeJSCore (internal/bootstrap/node.js:622:3)

error Command failed with exit code 1.
```