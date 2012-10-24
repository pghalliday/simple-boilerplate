boilerplate
=========

A simple, configurable, template based boilerplate project generator

## Features

- should copy the template files to the given folder
- should make replacements in the files and file names it copies
- should fail gracefully on errors

## Installation

```
npm install boilerplate
```

## API

```javascript
var Boilerplate = require('boilerplate');

var REPLACEMENTS = [{
  what: 'A_FIELD',
  with: 'some text'
}, {
  what: 'ANOTHER_FIELD',
  with: 'some other text'
}];

var boilerplate = new Boilerplate(TEMPLATE_DIRECTORY);
boilerplate.generate(TARGET_DIRECTORY, REPLACEMENTS, function(error) {
  if (error) {
    // a problem occurred generating the boiler plate
  } else {
    // the boiler plate project will have been generated in TARGET_DIRECTORY,
    // copying the contents of the TEMPLATE_DIRECTORY and making the specified
    // replacements both in file names and within the file contents
  }
});
```

## Roadmap

- None at this time

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using ``./grunt.sh`` or ``.\grunt.bat``.

## Release History
_(Nothing yet)_

## License
Copyright (c) 2012 Peter Halliday  
Licensed under the MIT license.