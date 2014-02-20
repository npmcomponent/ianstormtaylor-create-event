*This repository is a mirror of the [component](http://component.io) module [ianstormtaylor/create-event](http://github.com/ianstormtaylor/create-event). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ianstormtaylor-create-event`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# create-event

  Create an `event` object cross browser. Useful for unit testing mostly.

## Installation

    $ component install ianstormtaylor/create-event

## Example
  
```js
var create = require('create-event');
var event = create('keydown', {
  ctrl: true,
  key: 'enter'
});
```

## API

### createEvent(type, [options])
  
  Types:

    'click'
    'dblclick'
    'keydown'
    'keyup'

  Default `options`:

    alt        : false,
    bubbles    : true,
    button     : 0,
    cancelable : true,
    clientX    : 0,
    clientY    : 0,
    ctrl       : false,
    detail     : 1,
    key        : 0, // can be a string like 'enter' for convenience
    meta       : false,
    screenX    : 0,
    screenY    : 0,
    shift      : false,
    view       : window

## License

  MIT
