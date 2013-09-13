
# event

  Element event binding component.

## Installation

    $ component install kewah/event

## Example

```js
var events = require('event');
var a = document.querySelector('a');

function onclick(e) {
  e.preventDefault();
  console.log(e.target);
}

events.once(a, 'click', onclick);
```

## API

### .on(el, type, callback, [capture])

  Bind to `el`'s event `type` with `callback`,
  returns the `callback` passed.

### .off(el, type, callback, [capture])

  Unbind `el`'s event `type` `callback`,
  returns the `callback` passed.

### .once(el, type, callback, [capture])

  Bind to `el`'s event `type` with `callback`,
  returns the `callback` passed.

## License

  MIT
