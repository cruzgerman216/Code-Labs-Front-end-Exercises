# Warm Up Exercise

## Exercise 1: Waiter

You are a confident(perhaps cocky) waiter. You think you can write down all the information down from the top of your head.

Given the array of orders. Log each order onto the console by defining the logic in a function called `reciteMyOrders`.

```js
const orders = [
  {
    order: "Nachos with Cheese",
    name: "Sandy",
    price: "$13.99",
  },
  {
    order: "Chile Relleno, Burrito, & Rice",
    name: "John",
    price: "$13.99",
  },
  {
    order: "Flauta, Chicken Quesadilla, & Taco",
    name: "Amy",
    price: "$13.99",
  },
];

function reciteMyOrders(customerOrders) {
  // write your logic here
}

reciteMyOrders(orders);

// Solution
// Nachos with Cheese
// Chile Relleno, Burrito, & Rice
// Flauta, Chicken Quesadilla, & Taco
```

## Exercise 2: Random Image
When a user clicks a button, add a random dog image to the webpage.

Send a request to `https://dog.ceo/api/breeds/image/random` to receive a random image address.