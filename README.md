# plantuml-encoder
PlantUML encoder for browsers and Node.js.

[![npm Version](https://img.shields.io/npm/v/plantuml-encoder.svg)](https://www.npmjs.com/package/plantuml-encoder) [![build-status](https://travis-ci.org/markushedvall/plantuml-encoder.svg?branch=master)](https://travis-ci.org/markushedvall/plantuml-encoder) [![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)

Encoded PlantUML can be used to create PlantUML URL links.

# Install

Node.js:

```
npm install plantuml-encoder
```

browser:

```
bower install plantuml-encoder
```

# Example

```javascript
var plantumlEncoder = require('plantuml-encoder')

var encoded = plantumlEncoder.encode('A -> B: Hello')
console.log(encoded) // UDfpLD2rKt2oKl18pSd91m0KGWDz

var url = 'http://www.plantuml.com/plantuml/img/' + encoded
```

The URL can then be used to display the diagram:

![alt tag](http://www.plantuml.com/plantuml/img/UDfpLD2rKt2oKl18pSd91m0KGWDz)

# Decode example

```javascript
var plantumlEncoder = require('plantuml-encoder')

var plain = plantumlEncoder.decode('UDfpLD2rKt2oKl18pSd91m0KGWDz')
console.log(plain) // A -> B: Hello

```

# License
MIT
