`ainakan-load` has been deprecated. You should use [ainakan-compile](https://github.com/ainakan/ainakan-compile).

-----

# ainakan-load

Load a Ainakan script comprised of one or more Node.js modules.

## Example

```js
var ainakan = require('ainakan');
var load = require('ainakan-load');

load(require.resolve('./agent.js'))
.then(function (source) {
  ainakan.attach('Skype')
  .then(function (session) {
    session.createScript(source)
    .then(...) // and so on
  });
});
```

## Installation

```bash
$ npm install ainakan-load
```
