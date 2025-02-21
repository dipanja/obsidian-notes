---
id: "02: Variables and Data Types"
aliases:
  - "02: Variables and Data Types"
tags:
  - javascript
  - javascript/fundamental
---

Date: 15-02-2025
Time: 20:40

# 02: Variables and Data Types

## Variables

### `let` `const` `var`

`let`, `const`, `var` are used to declare a variable.

- `let`: Block-scoped, can be reassigned
- `const`: Block-scoped, _cannot_ be reassigned
- `var`: Function-scoped, can be redeclared (not recomended)

```javascript
// let const var are used to declare a variable
let storage_name = "value";
const num = 324;
```

### _passed by value_

When a variable of premetive type is assigned to another variable the value of the variable is passed. No changes happen to the original variable that is assigned.

### _passed by reference_

## Data Types

### Primitive Data Types

1. `String`
2. `Number`
3. `Boolean`
4. `Undefined`
5. `Null`
6. `BigInt`
7. `Symbol`

### Non-Primitive Data Types

1. `Object`: Collection of key-value pairs
2. `Array`: Ordered list of values
3. `Function`

```javascript
// student is here an Object
let student = {
  name: "Ollie",
  age: 12,
  isEnrolled: true,
};
// to access any value by key
console.log(student.name);
```

## Resources

- YouTube: [02: Variables and Data Types](https://www.youtube.com/watch?v=tVqy4Tw0i64)
- [AST Explorer:](https://astexplorer.net/)
- All the topics are here [[40 Days of JavaScript]]

## Images

![apdhs image](image-resources/APDHS.jpeg)
how
