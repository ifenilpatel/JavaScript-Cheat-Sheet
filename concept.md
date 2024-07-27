# JavaScript Cheat Sheet

Welcome to the JavaScript Cheat Sheet! This guide is designed to provide a quick reference to essential JavaScript concepts, syntax, and best practices. Whether you're a beginner or an experienced developer, this cheat sheet will help you recall important JavaScript features.

## Table of Contents

1. [Variables](#variables)
2. [Data Types](#data-types)
3. [Operators](#operators)
4. [Functions](#functions)
5. [Conditionals](#conditionals)
6. [Loops](#loops)
7. [DOM Manipulation](#dom-manipulation)
8. [Additional Examples](#additional-examples)

## Variables

### ES5

```javascript
var name = "Fenil Patel";
```

### ES6+

```javascript
let userName = "ifenilpatel";
const fullName = "Fenil Patel";
```

## Data Types

### Primitive

```javascript
let str = "Hi"; // String
let num = 101; // Number
let bool = true; // Boolean
let undf; // Undefined
let n = null; // Null
let sys = Symbol("symbol"); // Symbol
```

### Non-primitive

```javascript
let array = ["abc", "def", "ghi"]; // Array
let obj = { firstName: "Fenil", lastName: "Patel" }; // Object
```

## Operators

### Arithmetic

```javascript
let sum = 1 + 1; // 2
let diff = 10 - 5; // 5
let prod = 10 * 1; // 10
let quotient = 10 / 5; // 2
let remainder = 10 % 5; // 0
```

### Comparison

```javascript
let isEqual = 10 == "10"; // true
let isStrictEqual = 10 === "10"; // false
let isNotEqual = 10 != 5; // true
let isStrictNotEqual = 10 !== 5; // true
```

### Logical

```javascript
let and = true && false; // false
let or = true || false; // true
let not = !true; // false
```

## Functions

### Function Declaration

```javascript
function greet(name) {
  return `Hello ${name}`;
}
```

### Function Expression

```javascript
const greet = function (name) {
  return `Hello ${name}`;
};
```

### Arrow Function

```javascript
const greet = (name) => `Hello ${name}`;
```

## Conditionals

### If-else

```javascript
if (condition) {
  // code
} else if (condition) {
  // code
} else {
  // code
}
```

### Ternary Operator

```javascript
let result = condition ? "true" : "false";
```

## Loops

### For Loop

```javascript
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```

### While Loop

```javascript
let i = 0;
while (i < 10) {
  console.log(i);
  i++;
}
```

### Do-While Loop

```javascript
let j = 0;
do {
  console.log(j);
  j++;
} while (j < 10);
```

### For..of Loop (for arrays)

```javascript
let array = [1, 2, 3];
for (let value of array) {
  console.log(value);
}
```

### For..in Loop (for objects)

```javascript
let object = { a: 1, b: 2, c: 3 };
for (let key in object) {
  console.log(key, object[key]);
}
```

## DOM Manipulation

### Selecting Elements

```javascript
let element = document.getElementById("id");
let elements = document.getElementsByClassName("class");
let element = document.querySelector("selector");
let elements = document.querySelectorAll("selector");
```

### Changing Content

```javascript
element.textContent = "New text";
element.innerHTML = "<p>Hi</p>";
```

### Changing Styles

```javascript
element.style.color = "red";
```

### Adding/Removing Classes

```javascript
element.classList.add("className");
element.classList.remove("className");
```

### Event Listeners

```javascript
element.addEventListener("click", function () {
  console.log("clicked");
});
```

## Additional Examples

### Template Literals

```javascript
let name = "Fenil";
let greeting = `Hello, ${name}!`; // "Hello, Fenil!"
```

### Spread Operator

```javascript
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5, 6]; // [1, 2, 3, 4, 5, 6]

let obj1 = { a: 1, b: 2 };
let obj2 = { ...obj1, c: 3 }; // { a: 1, b: 2, c: 3 }
```

### Destructuring

```javascript
let [a, b] = [1, 2]; // a = 1, b = 2
let { x, y } = { x: 10, y: 20 }; // x = 10, y = 20
```

### Promises

```javascript
let promise = new Promise((resolve, reject) => {
  let success = true;
  if (success) {
    resolve("Success!");
  } else {
    reject("Error!");
  }
});

promise
  .then((response) => {
    console.log(response); // "Success!"
  })
  .catch((error) => {
    console.log(error); // "Error!"
  });
```

### Async/Await

```javascript
async function fetchData() {
  try {
    let response = await fetch("https://api.example.com/data");
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Error:", error);
  }
}

fetchData();
```

### Dates

```javascript
let now = new Date();
let specificDate = new Date("2020-01-01");
let year = now.getFullYear();
let month = now.getMonth();
let day = now.getDate();
let hours = now.getHours();
let minutes = now.getMinutes();
let seconds = now.getSeconds();

now.setFullYear(2022);
now.setMonth(11);
now.setDate(25);
now.setHours(10);
now.setMinutes(30);
now.setSeconds(45);
```

### Timers

```javascript
let timeoutId = setTimeout(function () {
  // code
}, 1000);

clearTimeout(timeoutId);

let intervalId = setInterval(function () {
  // code
}, 1000);

clearInterval(intervalId);
```

### Modules

```javascript
// Exporting
export const myVar = 42;
export function myFunction() {
  // code
}
export default function () {
  // code
}

// Importing
import { myVar, myFunction } from "./myModule";
import myDefaultFunction from "./myModule";
```

### Local Storage

```javascript
// Set Item
localStorage.setItem("key", "value");

// Get Item
let value = localStorage.getItem("key");

// Remove Item
localStorage.removeItem("key");

// Clear Storage
localStorage.clear();
```

### Session Storage

```javascript
// Set Item
sessionStorage.setItem("key", "value");

// Get Item
let value = sessionStorage.getItem("key");

// Remove Item
sessionStorage.removeItem("key");

// Clear Storage
sessionStorage.clear();
```
