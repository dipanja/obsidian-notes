---
id: "03: Operators and Expressions"
aliases:
  - "03: Operators and Expressions"
tags:
  - javascript
  - javascript/fundamental
---

Date: 19-02-2025
Time: 01:27

# 03: Operators and Expressions

## Operators

- `Operators`: Symbols (+ - \* /)
- `Operands`: x + y, x and y are the Operands

### Arithmetic:

```javascript
let a = 10;
let b = 20;
console.log(a + b); // 30
console.log(a - b); // -10
console.log(b + a); // 10
console.log(a * b); // 200
console.log(a / b); // 0.5

console.log(2 ** 3); // 8 exponent
console.log(12 % 5); //2 reminder operator

// post increment: first returns the value then increment
let count = 10;
console.log(count++); // 10

// pre increment: returns the value after increment
let c = 10;
console.log(++c); // 11

let f_name = "dipanjan";
let l_name = "paul";
console.log(f_name + l_name); // dipanjanpaul
```

### Assigment:

```javascript
let x = 10;
x += 5; // is similar to // 15
x = x + 5; // 20
x - +3; // 17
x *= 3; // x = x * 3
x /= 3; // x = x / 3
```

### Comparison:

```javascript
// always use === for Comparison
console.log(2 === "2"); // false
console.log(null === null); // true
console.log(undefined === undefined); // true
// for NaN value it is always false.
// for comparing objects it compares the memory address not the value stored in
// hence it is not a good idea to compare two objects
```

### Relational:

```javascript
//
```

### Logical:

- `&&`: logical AND
- `||`: logical OR
- `??`: Nullish coalescing operator

```javascript
// op1 && op2
// if op_1 can be convered to false the returns false else returns the op_2
console.log(false && false); // false
console.log(true && false); // false
console.log(true && true); // true
console.log(false && true); // false

console.log("a" && "b"); // "b"

// OR
// if op_1 can be convered to true returns true else returns op_2

console.log(false || false); // false
console.log(true || false); // true
console.log(true || true); // true
console.log(false || true); // true

console.log("a" && "b"); // "a"

// negate !
console.log(!true); // false

// Nullish coalescifalseng operator
// if op_1 is null or undefined returns the op_2

let a1 = null ?? 1; // a1 = 1
let a2 = undefined ?? 3; // a2 = 3
let a3 = false ?? "dipanjan"; // a3 = false
let a4 = 0 ?? "dipanjan"; // a4 = 0
```

### Bitwise:

- `&`: AND
- `|`: OR
- `^`: XOR
- `~`: NOT
- `<<`: left shift
- `>>`: right shift

```javascript
// 15 & 9 this is bitwise and
// convert 15 and 9 to 32 bit binary and then do bitwise from right.
// 1111 & 1001 = 1001 convered to 9
15 & 9; // 9

// 1111 | 1001 = 1111 convered to 15
15 | 9; // 15

// 1111 ^ 1001 = 0110 convered to 6
15 ^ 9; // 6

// left shift operator shift's the digit to left and fill the remaining with 0
// 1001 << 2 100100 convered to 36
9 << 2; // 32

// 1001 >> 2 0010 convered to 2
9 >> 2; // 2
```

### Conditional (ternary):

```javascript
// condition ? value_1 : value_2
// if condition is true return value_1 else return value_2

let age = 18;
age > 18 ? "Audult" : "Minor";
```

### Grouping:

- Grouping is same as in BODMAS rule in math. the thing in brackets will have higher presidence

```javascript
let p = 1;
let q = 2;
let r = 3;
// then p + r * q = 7
p + r * q; // 7

// and (p + q) * r  = 9
(p + q) * r; // 9
```

### typeOf:

- typeOf returns the type of the selected instance as strig

```javascript
typeOf "dipanjan" // "string"
typeOf false // "boolean"

const numbers = [ 1,2,2,4]
typeOf numbers // "object"

typeOf null; // 'object'
```

### instanceOf:

```javascript
//
```

## Expression:

- `x = 2`: assignment expression
- `x = 4 + 3`: is a evaluating expression

## Resources

- YouTube: [03: Operators and Expressions](https://www.youtube.com/watch?v=vI95K-_JLOw)
  All the topics are here [40 Days of JavaScript](notes/40%20Days%20of%20JavaScript.md)
