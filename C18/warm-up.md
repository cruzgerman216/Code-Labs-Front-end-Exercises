# Warm Up Exercise


## Exercise 1 
Create a function that filters a list of users whose `confirmation_email` property is ONLY set to true. User the built in filter method to do just this.

https://www.w3schools.com/jsref/jsref_filter.asp

```js
let users = [
  {
    username: "John123",
    confirmation_email: true
  }, 
  {
    username: "Amy123",
    confirmation_email: false
  },
  {
    username: "Jamie123",
    confirmation_email: true
  }
]

```

Expected result: 
let users = [
  {
    username: "John123",
    confirmation_email: true
  }, 
  {
    username: "Jamie123",
    confirmation_email: true
  }
]

## Exercise 2
Define a function that will convert a number (kilometers) into miles.
