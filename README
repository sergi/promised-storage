Promised Storage is basically a port of
[Mozilla's async_storage.js](https://github.com/mozilla-b2g/gaia/blob/master/shared/js/async_storage.js) to Promises.

With Promised Storage you can store data in a persistent Key/Value database in the browser
similarly to how you do it with [localStorage](http://diveintohtml5.info/storage.html)
but in a non-blocking way (localStorage methods block the main thread). It does so
by leveraging the more powerful [IndexedDB](https://developer.mozilla.org/en/docs/IndexedDB)
database behind the scenes.

Usage
-----

For example:

```javascript
var p = promisedStorage.setItem("solution", 42);
p.then(function() {
  return promisedStorage.getItem("solution")
}).then(function(value) {
    console.log("The Stored value is", value); // 42
});
```

License
-------

Apache 2.0