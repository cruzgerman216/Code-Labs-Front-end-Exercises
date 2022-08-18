# JavaScript Foundations - Part 1 (Class 2)

## Exercise #0: Before getting started 
- Create a file called foundations.txt 
- Answer the following questions in your own words:
1. What are data types? 
2. What are operators used for? 
3. What are conditional statements? 
4. What are loops? 

## Exercise #1: Variables

**Aim**: Create a variable for every JavaScript Data Type

- Create a file called variables.js
- Create a variable that holds a _string_ value
- Create a variable that holds a _number_ value
- Create a variable that holds a _boolean_ value
- Create a variable that holds a _null_ value
- Create a variable that holds an _undefined_ value
- Create a variable that points to an _object_ instance
- Create a variable that points to an _array_ instance
- Create a variable that has no default value declaration

---

---

## Exercise #2: Operators 
- Create operators.js

- Code an example of each of the following operators 
  - `+`
  - `-`
  - `/`
  - `*`
  - `>`
  - `<`
  - `===`
  - `!==`

---

---

## Exercise 3: Conditional Statements 
- Create conditional-statements.js
- Code an example of a conditional statement

---

---

## Exercise 4: For loop 
- Create for-loop-example.js
Given the array 
```js
  let students = ['John', 'Jane', 'Jimmy']
```

Use a for loop to print out the names of each student. 

---

---

## Exercise 5: Found John!

Give the array 
```js 
  let people = [
    {
      name: "james",
      age: 34
    }, 
    {
      name: "John",
      age: 43
    },
    {
      name: "Jane",
      age: 23
    }
  ]
```
- Iterate through the array using a loop. 
  - If an object contains the name `John`, then print to the console "I found John!"
  - If an object contains the name `Jane`, then print to the console "Hey Jane, do you know where John is?"
  - If all else fails, then print `Hey do you happen to know someone by the name of John?`.

---

---

### Further Challenges
## Exercise 6: Multiples

**Aim**: Create a function that takes two numbers as arguments (num, length) and returns an array of multiples of num until the array length reaches length.

_Examples_

```js
arrayOfMultiples(7, 5)    ➞    [7, 14, 21, 28, 35]

arrayOfMultiples(12, 10)    ➞    [12, 24, 36, 48, 60, 72, 84, 96, 108, 120]

arrayOfMultiples(17, 6)    ➞    [17, 34, 51, 68, 85, 102]
```

## Exercise #7: Html and JS

**Aim**: Dynamically display a list of food items and prices using HTML & JavaScript

- Create a LIST of OBJECTS, each object having a name and price property
- LOOP over that LIST, dynamically create a new list item `<li></li>` with the food name inside, and append that item to an existing HTML `<ul></ul>` element