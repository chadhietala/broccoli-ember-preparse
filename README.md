# broccoli-ember-preparse
Broccoli plugin that applies some compile time performance optimizations to an ember build.

Essentially a broccoli plugin version of [define-rewriter](https://github.com/chadhietala/define-rewriter).

Credit to [Chad Hietala](https://github.com/chadhietala) and [Kris Selden](https://github.com/krisselden) for the idea and the proof of concept.

## Usage

``` javascript
var emberPreparse = require('broccoli-ember-preparse');

// distTree must include the ember.debug.js and ember.prod.js files
// loaderPackageTree must include ember's loader package
var newDistTree = emberPreparse(distTree, loaderPackageTree);
```
