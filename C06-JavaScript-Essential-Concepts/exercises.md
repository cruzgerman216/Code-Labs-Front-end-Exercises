# JavaScript Essential Concepts 
** Read before getting started. Create a folder called `code-labs`. In `code-labs`, create an additional folder called `class-6`. You will be working in class 6 for today**

*This is the time to experiment*

## Exercise #1: Scopes - Will it show "John" or "Pete"?
Create a folder in `class-6` called `exercise-1`. Create the necessary files in this folder to solve the exercise.

The function sayHi uses an external variable name. When the function runs, which value is it going to use?

```js
let name = "John";

function sayHi() {
  alert("Hi, " + name);
}

name = "Pete";

sayHi(); // what will it show: "John" or "Pete"?
```

Such situations are common both in browser and server-side development. A function may be scheduled to execute later than it is created, for instance after a user action or a network request.

So, the question is: does it pick up the latest changes?

Will the sayHi call show 'john' or 'pete'. Before executing the code, think about this. To check your answer, execute this code.

You have solved this exercise when you understand the solution.

[source](https://javascript.info/closure)

---

---

## Exercise #2: Scopes - Will it show "John" or "Pete"? Part 2
In `class-6`, create a folder called `exercise-2`. Create the necessary files in this folder to solve the exercise.

The function makeWorker below makes another function and returns it. That new function can be called from somewhere else.

Will it have access to the outer variables from its creation place, or the invocation place, or both?

```js
function makeWorker() {
  let name = "Pete";

  return function() {
    alert(name);
  };
}

let name = "John";

// create a function
let work = makeWorker();

// call it
work(); // what will it show?
```
Which value it will show? “Pete” or “John”? Before executing the code, think about this. To check your answer, execute this code.

You have solved this exercise when you understand the solution.

[source](https://javascript.info/closure)

---

---

## Exercise #3: Scopes - Are counters independent?
In `class-6`, create a folder called `exercise-3`. Create the necessary files in this folder to solve the exercise.

Here we make two counters: counter and counter2 using the same makeCounter function.

Are they independent? What is the second counter going to show? 0,1 or 2,3 or something else?

```js
function makeCounter() {
  let count = 0;

  return function() {
    return count++;
  };
}

let counter = makeCounter();
let counter2 = makeCounter();

alert( counter() ); // 0
alert( counter() ); // 1

alert( counter2() ); // ?
alert( counter2() ); // ?
```
Before executing the code, think about this. To check your answer, execute this code.

You have solved this exercise when you understand the solution.

[source](https://javascript.info/closure)

## Exercise #4: Base times height

**Aim**: Create a function that calculates the area of a triangle given the base and height as arguments. Call the function a few times with different inputs.

---

---

## Exercise #5: Range

**Aim**: Write a function that returns an array containing all the numbers inclusive to that range given the start and end values. See examples below.

_Examples_

```js
reversibleInclusiveList(1, 5)    ➞    [1, 2, 3, 4, 5]

reversibleInclusiveList(2, 8)    ➞    [2, 3, 4, 5, 6, 7, 8]

reversibleInclusiveList(10, 20)    ➞   [10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]

reversibleInclusiveList(24, 17)    ➞   [24, 23, 22, 21, 20, 19, 18, 17]
```

_Notes_

- The resulting array's sort order is dependent on the input values.
- All inputs provided in the test scenarios are valid.
- If the start is greater than the end, return a descendingly sorted array; otherwise, ascendingly sorted.

---

---

## Exercise #6: Add all multiplied paired numbers 

**Aim**: Create a function that takes three collections of arguments and returns the sum of the product of the grouped numbers.

_Examples_

```js
product([[1,2],[1,1],[2,3]])    ➞    9
// 1 * 2 + 1 * 1 + 2 * 3

product([[10,2],[5,0],[2,3]])    ➞    26
// 10 * 2 + 5 * 0 + 2 * 3

product([[1,2],[2,3],[3,4]])   ➞    20
// 1 * 2 + 2 * 3 + 3 * 4

product([[1,2],[0,3],[3,0]])    ➞    2
// 1 * 2 + 0 * 3 + 3 * 0
```

---

---

## Exercise #7: Verify if a number is a prime number.
