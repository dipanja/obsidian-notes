---
id: "05: Loops and Iterations"
aliases:
  - "05: Loops and Iterations"
tags:
  - javascript
  - javascript/fundamental
---

# 05: Loops and Iterations

- for loops
- while loops
- do while loops

## `for` loop

```javascript
// for loops
// used when we know exactly how many times to loop
// for (initialization; conditon; update) {
//   //code
// }
for (let count = 1; count <= 5; count++) {
  console.log("the count", count);
}
// add all even numbers between 1 and 100
let sum = 0;
for (leti = 1; i <= 100; i++) {
  if (i % 2 === 0) {
    sum = sum + i;
    //sun += i
  }
}
console.log("sum is", sum);

let language = "javascript";
for (let i = 0; i < language.length; i++) {
  console.log(language.charAt(i));
}

// break and continue

// break
for (let i = 1; i <= 5; i++) {
  console.log(i);
  if (i === 3) break; // breakes the loop here
}

// continue
for (let i = 1; i <= 5; i++) {
  if (1 === 3) continue;
  console.log(i);
}

// Multiple Counters for single loop
for (let i = 1, j = 10; i <= 10 && j >= 1; i++, j--) {
  console.log("i = ", i, " j = ", j);
}
```

## `while` loop

```javascript
// while loop
let counter = 1;
while (counter <= 5) {
  console.log(counter);
  counter++;
}
```

## `do while` loop

```javascript
// do while loop
// the code will garuntee to execute atleast one
let num = 1;
do {
  console.log(num);
  num++;
} while (num <= 5);
```

## Resources

- YouTube: [05: Loops and Iterations](https://www.youtube.com/watch?v=MDR43-2GvtA)
- All the topics are here [40 Days of JavaScript](notes/40%20Days%20of%20JavaScript.md)
