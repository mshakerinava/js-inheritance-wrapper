# JavaScript Inheritance Wrapper

Javascript inheritance in one line. The way it's meant to be.

## Example

```javascript

var A = Class.extend({
  constructor: function (a) {
    this.a = a
  },

  getA: function () {
    return this.a
  }
})

var B = A.extend({
  constructor: function (a, b) {
    this.super.constructor.call(this, a)
    this.b = b
  },

  getB: function () {
    return this.b
  }
})

var b = new B(1, 2)

console.log('1 =? ', b.getA())
console.log('2 =? ', b.getB())
console.log('true =? ', b instanceof B)
console.log('true =? ', b instanceof b.constructor)

```

## Install

* **npm**

```sh
npm install inheritance-wrapper
```

* **bower**

```sh
bower install inheritance-wrapper
```

* **Or** just download the class.js file.

## License

The MIT License (MIT)
Copyright (c) 2016 Mehran Shakerinava
