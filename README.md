# [tape](https://github.com/substack/tape) standalone version

For use with browser loaders like [System.js](https://github.com/systemjs/systemjs) 
or [Steal.js](https://github.com/stealjs/steal) or event just using `script` tag.

This is just a browserified version made with command:
```
browserify node_modules/tape -o tape.js -s test
```

So it is a UMD module that exports `test`

# example

So with System.js/Steal.js you can do:
``` js
var test = require('tape-standalone')
// Or even just:
// var test = require('tape') // with proper mapping - works with Steal.js without config
require('tap-browser-color')()

test('Something', t => {
  t.ok(1 === 1)
  t.end()
})
```

# install

```bash
npm install tape-standalone --save-dev
```

**Current version bundled: 4.4.0** (package.json version matches tape.js version)

# license

ISC
