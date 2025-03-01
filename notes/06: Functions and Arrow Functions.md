---
id: "06: Functions and Arrow Functions"
aliases:
  - "06: Functions and Arrow Functions"
tags:
  - javascript
  - javascript/fundamental
---

Date: 27-02-2025
Time: 23:59

# 06: Functions and Arrow Functions

## Functions

```javascript
function printThis() {
  console.log("Print me......");
}
printThis();
```

```javascript
// Functions as Expression
let printMe = function () {
  console.log("Print Me.....");
};
printMe();
```

```javascript
// Parameters and Arguments
function sum(a, b) {
  const result = a + b;
  console.log(result);
  return result;
}

result = sum(1 + 1.5);
console.log(result);
```

```javascript
// Rest Parameters
// rest parameter will always be the last parameter
function calulateThis(a, s, d, ...rest) {
  console.log(a, s, d, rest); // a, s, d, [rest]
}
```

```javascript
// Nested function

function outerFunc() {
  console.log("Outer Funtion");

  function inner() {
    console.log("inner Function");
  }
  inner();
}
outerFunc();

function outer() {
  console.log("outer");
  return function inner() {
    console.log("inner");
  };
}

let returnFunction = outer(); // log's outer
returnFunction(); // log's inner
```

```javascript
// callback functions
function foo(func) {
  console.log("foo");
  func();
}

foo(function () {
  console.log("bar.....");
});
```

```javascript
// arrow function
const greet = (name) => {
  return `Hello, ${name}!`;
};

const greet = (name) => `Hello, ${name}!`;
```

```javascript
// Basic Immediately Invoked Function Expressions (IIFEs)
(function () {
  console.log("This function is executed immediately");
})();

// IIFE with parameters
(function (message) {
  console.log(message);
})("Hello from IIFE!");

// IIFE with arrow function
(() => {
  console.log("This is an arrow function IIFE");
})();

// IIFE that returns a value
const result = (function () {
  const x = 10;
  const y = 20;
  return x + y;
})();
console.log(result); // Outputs: 30

// IIFE for creating private scope
const counter = (function () {
  let count = 0; // Private variable

  return {
    increment: function () {
      count++;
      return count;
    },
    decrement: function () {
      count--;
      return count;
    },
    getValue: function () {
      return count;
    },
  };
})();

console.log(counter.increment()); // 1
console.log(counter.increment()); // 2
console.log(counter.getValue()); // 2
console.log(counter.decrement()); // 1
```

## Resources

- YouTube: [06: Functions and Arrow Functions](https://www.youtube.com/watch?v=6UJ9SyHvkJY&t=0s)
- All the topics are here [[40 Days of JavaScript]]
