# JavaScript Foundations - Part 2 (Class 3)

## Exercise #1: 

**Aim**: Create a function that takes in an argument and uses string interpolation to print that arguments value somewhere in a text string

- [ ] Create a function
- [ ] Have that function take in an argument
- [ ] Print a statement that uses the variable along with some other text

---

---

## Exercise #2a: 

**Aim**: Create an application that, on button click, runs a function that prints out a user's name, age, and occupation

- [ ] Create the HTML with a button
- [ ] Create a function that takes in a _user_ object
- [ ] Print each item in the user object out in a string to the console


## Exercise #2.b

Instead of printing each item to the console, add them to the webpage. 

## Exercise #2.c 
If the user's name so happens to be more than 5 letters long, color the element's background it's in to a random color. 

---

---

## Exercise #3: 

**Aim**: Create a function that takes an object and returns the keys and values as separate arrays. Return the keys sorted alphabetically and their corresponding values in the same order.

_Examples_

```js
keysAndValues({ a: 1, b: 2, c: 3 })
   ➞    [["a", "b", "c"], [1, 2, 3]]

keysAndValues({ a: "Apple", b: "Microsoft", c: "Google" })
   ➞    [["a", "b", "c"], ["Apple", "Microsoft", "Google"]]

keysAndValues({ key1: true, key2: false, key3: undefined })
   ➞    [["key1", "key2", "key3"], [true, false, undefined]]
```

---

---
## Exercise #4: Function min(a, b)

Write a function min(a,b) which returns the least of two numbers a and b.

For instance:

min(2, 5) == 2
min(3, -1) == -1
min(1, 1) == 1

---

---
## Exercise #5: Function pow(x,n)

Write a function pow(x,n) that returns x in power n. Or, in other words, multiplies x by itself n times and returns the result.

pow(3, 2) = 3 * 3 = 9
pow(3, 3) = 3 * 3 * 3 = 27
pow(1, 100) = 1 * 1 * ...* 1 = 1

---

---

## Exercise #6a: Even and Odd 
Loop through numbers 0 - 100. When a number is even, print for example `0 is an even number`. Otherwise print for example, `1 is an odd number`. 

---

---

## Exercise #6b: Prime numbers 
To add onto #6a, if a number is a prime number, print for example `1 is a prime number`.

## Exercise #7: Creating a Modal
Create a button and once clicked, the user will see a modal with the message "Here's another annoying pop up!". The modal should also include a button that will allow the user to click out.