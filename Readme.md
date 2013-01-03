 [![Build Status](https://secure.travis-ci.org/gjohnson/pluck.png?branch=master)](http://travis-ci.org/gjohnson/pluck)

# pluck

  pluck property path from arrays or an object.

## Installation

*component*

```sh
  $ component install redventures/pluck
```

or

*npm*

```sh
  $ npm install pluck
```

## Example

Pluck from arrays.

```javascript
var pluck = require('pluck');

var firstName = pluck('name.first');

var items = [
  { name: { first: 'john', last: 'doe' } }
];

var names = firstName(items);
```

Pluck from simple objects.

```javascript
var pluck = require('pluck');

var item = {
  name: {
    first: 'john',
    last: 'doe'
  }
};

var name = firstName(item);
```

## API

### pluck(path)

Creates the property lookup function.
   
## License

MIT