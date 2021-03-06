# js-prototype

[![npm](https://img.shields.io/npm/v/js-prototype.svg)](https://www.npmjs.com/package/js-prototype)
[![license](https://img.shields.io/github/license/thinkholic/js-prototype.svg)](https://github.com/thinkholic/js-prototype/blob/master/LICENSE)

Modified prototype methods for JS

## Installation

```
npm i -S js-prototype
```

## Usage

### String

#### String.allReplace()

```js
require 'js-prototype'; // or require 'js-prototype/string';

var str = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.';

var list = {
    'ipsum': 'REPLACED-ipsum',
    'amet': 'REPLACED-amet'
};
var newStr = str.allReplace(list);
console.log(newStr); // Lorem REPLACED-ipsum dolor sit REPLACED-amet, consectetur adipiscing elit.
```

#### String.toTitleCase()

```js
require 'js-prototype'; // or require 'js-prototype/string';

var str = 'Lorem ipsum dolor';
var result = str.toTitleCase();
console.log(result); // Lorem Ipsum Dolor

```

### Object

#### Object.isEmpty()

```js
require 'js-prototype'; // or require 'js-prototype/object';

const a = {};
const b = {a: 1, b:3};
console.log(a.isEmpty()); // true
console.log(b.isEmpty()); // false
```

### Array

#### Array.drop()

```js
require 'js-prototype'; // or require 'js-prototype/array';

// By Value
const arr = [1, 2, 3, 4, 5, 6];
arr.drop(2);
console.log(arr); // [1, 3, 4, 5, 6]

// By Index
arr.drop(null, 0);
console.log(arr); // [3, 4, 5, 6]
```

## License

MIT