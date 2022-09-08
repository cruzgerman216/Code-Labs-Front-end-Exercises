# JavaScript Intermediate Concepts

** Read before getting started. Create a folder called `code-labs`. In `code-labs`, create an additional folder called `class-7`. You will be working in class 7 for today**

_This is the time to experiment_

## Exercise #1: Closures - Check number

Create a folder in `class-7` called `exercise-1`. Create the necessary files in this folder to solve the exercise.

The function sayHi uses an external variable name. When the function runs, which value is it going to use?

```js
function numberGenerator() {
  // Local “free” variable that ends up within the closure
  let num = 1;
  function checkNumber() {
    console.log(num);
  }
  num++;
  return checkNumber;
}

var number = numberGenerator();
number();
```

What will `number()` log to the console?

You have solved this exercise when you understand the solution.

[source](https://www.freecodecamp.org/news/lets-learn-javascript-closures-66feb44f6a44/)

---

---

## Exercise #2: Closures - Hello world!

In `class-7`, create a folder called `exercise-2`. Create the necessary files in this folder to solve the exercise.

```js
function sayHello() {
  let say = function () {
    console.log(hello);
  };
  // Local variable that ends up within the closure
  let hello = "Hello, world!";
  return say;
}
var sayHelloClosure = sayHello();
sayHelloClosure();
```

What will `sayHelloClosure()` log to the console?

You have solved this exercise when you understand the solution.

[source](https://javascript.info/closure)

---

---

## Exercise #3: Closures - Nested functions

In `class-6`, create a folder called `exercise-3`. Create the necessary files in this folder to solve the exercise.

You may need a piece of paper.

```js
let x = 10;

function foo(a) {
  let b = 20;

  function bar(c) {
    let d = 30;
    return boop(x + a + b + c + d);
  }

  function boop(e) {
    console.log(e * -1);
  }

  return bar;
}

let moar = foo(5); // Closure

moar(15);
```

What will `moar` log to the console?

Before executing the code, think about this. To check your answer, execute this code.

You have solved this exercise when you understand the solution.

[source](https://www.freecodecamp.org/news/lets-learn-javascript-closures-66feb44f6a44/)


## Exercise #4: High order function
Create a folder in `class-7` called `exercise-4`. Create the necessary files in this folder to solve the exercise.


**Aim**: Write a function `redundantReturn` that takes in a string `str` as a parameter and returns a function that returns this parameter. 

---

---

## Exercise #5: More closures
Create a folder in `class-7` called `exercise-5`. Create the necessary files in this folder to solve the exercise.

Closures are functions that remember their lexical environments. Lexical environments mean the environment in which the function was declared.

```javascript
function parent(x) {
  return function closure() {
    // Closure is declared here.
    return x;
  };
}

const remember = parent("remembers me");
// Seems like the variable x would be gone after
// parent is executed, but it's not.

closure(); // WRONG, the global scope doesn't have access to its inner scopes and the closure method
// Returns "remembers me" because the inner
// function remembers x.
```

**Aim**: Fix this code so it ultimately prints 'remembers me'.


---

---

## Exercise #6: Drinks on a summer day
Create a folder in `class-7` called `exercise-6`. Create the necessary files in this folder to solve the exercise.

You will be given an array of drinks, with each drink being an object with two properties: `name` and `price`. Define a function with the parameter representing the array of drinks and return the drinks objects sorted by price in ascending order.

Assume that the following array of drink objects needs to be sorted:

```js
drinks = [
  { name: "lemonade", price: 50 },
  { name: "lime", price: 10 },
  {name: 'carrot', price: 34}
];
```

The output of the sorted drinks object will be:

_Examples_

```js
sortDrinkByPrice(drinks)    // ->    [ {name: "lemonade", price: 50}, {name: 'carrot', price: 34}, {name: "lime", price: 10}]
```

---

---


## Exercise #7: Everyone's life savings put together
Create a folder in `class-7` called `exercise-7`. Create the necessary files in this folder to solve the exercise.

**Aim**: Define a function that takes an array with objects and returns the sum of people's budgets.

_Examples_

```js
getBudgets([
  { name: "John", age: 21, budget: 23000 },
  { name: "Steve",  age: 32, budget: 40000 },
  { name: "Martin",  age: 16, budget: 2700 }
])   // ➞    65700

getBudgets([
  { name: "John",  age: 21, budget: 29000 },
  { name: "Steve",  age: 32, budget: 32000 },
  { name: "Martin",  age: 16, budget: 1600 }
])   // ➞    62600
```

---

---

## Exercise #8: Objects to arrays
Create a folder in `class-7` called `exercise-8`. Create the necessary files in this folder to solve the exercise.

Define a function that converts an object into an array, where each element represents a key-value pair in the form of an array.

_Examples_

```js
toArray({ a: 1, b: 2 })   // ➞    [["a", 1], ["b", 2]]

toArray({ shrimp: 15, tots: 12 })  //  ➞    [["shrimp", 15], ["tots", 12]]

toArray({})    ➞   // []
```


# Bonus challenges - Test Your Might 

## Exercise #9: Greatest Common Divisor 
Create a folder in `class-7` called `exercise-9`. Create the necessary files in this folder to solve the exercise.

How would you find the greatest common divisor of two numbers?

```js 
function greatestCommonDivisor(a, b){

}

greatestCommonDivisor(14, 21); // returns 7
greatestCommonDivisor(69, 169); // returns 1
```