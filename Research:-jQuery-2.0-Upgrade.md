** WIP **
This page can be used to keep track of changes for the jQuery 2.0 upgrade.

Deprecated Functions
----------------------------------------
* [`$.fn.andSelf`](http://api.jquery.com/andSelf/) (Replaced with [`$.fn.addBack`](http://api.jquery.com/addBack/))
    * [src/thirdparty/jstree_pre1.0_fix_1/jquery.jstree.js](../blob/master/src/thirdparty/jstree_pre1.0_fix_1/jquery.jstree.js)

* [`deferred.isRejected`](http://api.jquery.com/deferred.isRejected/) & [`deferred.isResolved`](http://api.jquery.com/deferred.isResolved/) (Replaced with [`deferred.state`](http://api.jquery.com/deferred.state/))
    * Resolved in [#3665](../pull/3665)

* [`deferred.pipe`](http://api.jquery.com/deferred.pipe/) (Replaced with [`deferred.then`](http://api.jquery.com/deferred.then/))
    * [src/brackets.js](../blob/master/src/brackets.js)
    * [src/document/DocumentCommandHandlers.js](../blob/master/src/document/DocumentCommandHandlers.js)
    * [src/language/CSSUtils.js](../blob/master/src/language/CSSUtils.js)
    * [src/project/ProjectManager.js](../blob/master/src/project/ProjectManager.js)
    * [src/utils/Async.js](../blob/master/src/utils/Async.js)
    * [src/extensibility/Package.js](../blob/master/src/extensibility/Package.js)
    * [src/extensibility/node/ExtensionManagerDomain.js](../blob/master/src/extensibility/node/ExtensionManagerDomain.js)
    * [src/extensibility/node/package-validator.js](../blob/master/src/extensibility/node/package-validator.js)
    * [test/spec/ExtensionUtils-test.js](../blob/master/test/spec/ExtensionUtils-test.js)
    * [test/spec/JSUtils-test.js](../blob/master/test/spec/JSUtils-test.js)
    * [test/spec/SpecRunnerUtils.js](../blob/master/test/spec/SpecRunnerUtils.js)

* [`$.fn.die`](http://api.jquery.com/die/)
    * Not Used?

* [`$.fn.error`](http://api.jquery.com/error/) (Replaced with [`$.fn.on('error',...`](http://api.jquery.com/on/))
    * Partial Fix in [#3814](../pull/3814)

* [`$.boxModel`](http://api.jquery.com/jQuery.boxModel/) (Removed)
    * ?

* [`$.browser`](http://api.jquery.com/jQuery.browser/) (Removed)
    * [src/thirdparty/jstree_pre1.0_fix_1/jquery.jstree.js](../blob/master/src/thirdparty/jstree_pre1.0_fix_1/jquery.jstree.js)
    * Bootstrap > Update Being Reviewed? [#3672](../pull/3672])

* [`$.sub`](http://api.jquery.com/jQuery.sub/) (Removed)
    * Not Used?

* [`$.fn.live`](http://api.jquery.com/live/) (Replaced with [`$.fn.on`](http://api.jquery.com/on/))
    * Not Used?

* [`$.fn.load`](http://api.jquery.com/load-event/) (Replaced with [`$.fn.on('load',...`](http://api.jquery.com/on/))
    * Partial Fix in [#3814](../pull/3814)

* [`$.fn.selector`](http://api.jquery.com/selector/) (Removed)
    * Not Used?

* [`$.fn.size`](http://api.jquery.com/size/) (Replaced with [`$.fn.length`](http://api.jquery.com/length/))
    * [src/thirdparty/jstree_pre1.0_fix_1/jquery.jstree.js](../blob/master/src/thirdparty/jstree_pre1.0_fix_1/jquery.jstree.js)

* [`$.fn.toggle`](http://api.jquery.com/toggle-event/)
    * ?

* [`$.fn.unload`](http://api.jquery.com/unload/) (Replaced with [`$.fn.on('unload',...`](http://api.jquery.com/on/) or [`$.fn.on('beforeunload',...`](http://api.jquery.com/on/))
    * Not Used?

jQuery 1.8 Upgrade
----------------------------------------
* [`$.fn.data('events')`]() (Removed)
    * Not Used?

* [`$.curCSS`]() (Removed)
    * Not Used?

* [`$.attrFn`]() (Removed)
    * Not Used?

jQuery 1.9 Upgrade
----------------------------------------