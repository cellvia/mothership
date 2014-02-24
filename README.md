# mothership [![build status](https://secure.travis-ci.org/thlorenz/mothership.png)](http://travis-ci.org/thlorenz/mothership)

Helps a module find its package.json mothership.

```js
var findShip = require('mothership')
  , path = require('path');

findShip(
    path.join(__dirname, 'uno', 'dos', 'tres')
  , function ismothership (pack) {
      return !!(pack.dependencies && pack.dependencies.unodep);
    }
  , function (err, res) {
      if (err) return console.error(err);
      console.log('first mothership', res.path);  // => [..]/example/uno/package.json
  }
)
```

## Installation

    npm install mothership

## API


## License

MIT
