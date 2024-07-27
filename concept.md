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
