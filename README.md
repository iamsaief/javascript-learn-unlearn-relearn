<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png">
  <h1>Learn Unlearn Relearn JavaScript 🔄</h1>
</div>

<p align="center">
Test how well you know JavaScript, refresh your knowledge or prepare yourself for coding interview! 💪 <br/>
Feel free to study as you wish! 🎓 The details are in the collapsed sections, simply click to expand 🔽. <br/>
I've created those for fun. If you find it helpful, I would really appreciate a reference to this repo. Best of luck! 👍
</p>

<p align="center">
💬 In case you want to reach out or just say hi, ↩️ <br/>
<a href="https://www.facebook.com/saiefalemon">Facebook</a> | <a href="https://www.linkedin.com/in/saiefalemon">LinkedIn</a> | <a href="https://www.iamsaief.com/">Blog</a>
</p>

- [1. 🧐 Understanding *Truthy* and *Falsy* in JavaScript](#1--understanding-truthy-and-falsy-in-javascript)
  - [✅ Primitive Types](#primitive-types)
  - [✅ Reference Types](#reference-types)
  - [🤔 Why are Function Constructors Truthy?](#why-are-function-constructors-truthy)
  - [✨ Simple Analogy](#-simple-analogy)
- [2. 👨‍👩‍👧‍👦 Understanding Prototypal Inheritance in JavaScript](#2--understanding-prototypal-inheritance-in-javascript)
  - [💡Simple Analogy](#simple-analogy)
  - [📝 Handle with Care](#handle-with-care)
  - [🎓 The Takeaway](#the-takeaway)
- [3. 🤝 What Are Promises in JavaScript?](#3-what-are-promises-in-javascript)
  - [✨ Simple Analogy](#simple-analogy-1)
- [4. 🗃️ What Are Closures in JavaScript?](#4-️what-are-closures-in-javascript)
  - [🧩 Simple Analogy: The Picnic Basket](#-simple-analogy-the-picnic-basket)
  - [🔥 Use Cases and Benefits](#use-cases-and-benefits)


<!-- ---

Available Translations: [🇧🇩 বাংলা](./bn-BD/README_bn-BD.md)

--- -->

## 1. 🧐 Understanding *Truthy* and *Falsy* in JavaScript

<details><summary><b>Click to expand details</b></summary>

### ✅ Primitive Types

- 💡 Represent single, immutable values. Primitive types in JavaScript include `undefined`, `null`, `boolean`, `number`, `string`, `symbol`, and `BigInt`.

- 💡 If a primitive type has a value that is considered falsy (like `0`, `false`, `""`, `null`, `undefined`, or `NaN`), it will behave as false in a Boolean context.

- 💡 They are stored directly in the location where the variable accesses them.

### ✅ Reference Types

- 💡 Include objects such as `function`, `array`, and other `objects`, and they are mutable.

- 💡 When you create a reference type, JavaScript allocates memory for it and the variable you assign it to holds a reference (or pointer) to that memory space, not the actual data itself.

- 💡 Since a reference points to an object, and objects in JavaScript are inherently truthy, a reference type cannot be falsy. Even if an object is empty (like `{}`) or an array has no elements (`[]`), it is still truthy because a reference to an allocated memory space exists.

### 🤔 Why are Function Constructors Truthy?

- 💡 Function constructors like `new Number()` or `new Boolean()` create object wrappers around primitive values.

- 💡 Despite the primitive value inside the object being falsy (like `0` or `false`), the object wrapper itself is a reference type.

- 💡 As we’ve established, reference types are always truthy because they refer to a memory location, not the value itself.

### ✨ Simple Analogy

Think of primitive types as individual pieces of paper with something written on them. If the paper is blank (a falsy value), it’s like having nothing or false. Reference types, on the other hand, are like folders (objects) that can hold these papers. Even if the folder is designed to hold a blank paper, the folder itself still exists and is something (truthy). The function constructors like `new Number()` and `new Boolean()` are like special folders that come with a label and even if the label says `0` or `false` (falsy), the folder is still an item you can reference and use (truthy).

🧠 Remember, in JavaScript, the type of value determines its **truthiness** or **falsiness**. Objects will always be your go-to for a guaranteed truthy value!

</details>

## 2. 👨‍👩‍👧‍👦 Understanding Prototypal Inheritance in JavaScript
<details><summary><b>Click to expand details</b></summary>
<p>

In JavaScript, a ’prototype’ is like a blueprint for creating objects. It’s an object itself, and every function in JavaScript has a prototype property that’s used when creating new objects. This prototype object includes properties and methods that should be available to the objects created from the function.

### 💡Simple Analogy

Imagine you have a recipe for a cake. This recipe includes all the steps and ingredients you need to make the cake. In JavaScript, the recipe is like the ’prototype’. When you bake a cake using this recipe, the cake (an ‘object’) inherits all the properties from the recipe (the ‘prototype’). If you decide to add a new step to the recipe, like adding icing, all the cakes made from that recipe will now have icing too.

> ℹ️ Similarly, when you create an object from a constructor function in JavaScript, the object inherits all the properties and methods from the constructor’s prototype. This allows all objects created from the same constructor to share the same properties and methods, which can save memory and allow for a consistent structure.
>
>ℹ️ So, prototypal inheritance is a way objects in JavaScript can inherit properties and methods from a prototype, much like how multiple cakes can be made from the same recipe. But if a properties/methods is removed from the prototype, all objects that inherit from that prototype lose access to that properties/methods.

### 📝 Handle with Care
While it’s tempting to keep adding to prototypes, it’s generally not recommended because it can lead to unexpected behavior in code, especially if libraries or frameworks are used that might also modify the prototype. Remember that with great power comes great responsibility.

### 🎓 The Takeaway
Prototypal inheritance is a powerful feature in JavaScript that allows objects to share and extend behaviors efficiently. It’s what makes JavaScript dynamic and flexible, enabling us to write more reusable and maintainable code.

✨ So, the next time you’re working with JavaScript objects, remember the family tree of prototypes and how it empowers your code with shared DNA.

__🧠 Now that we have basic understanding, lets go through the following examples.__

**Example: Barking Dog**

```jsx
class Dog {
  constructor(name) {
    this.name = name;
  }
}

Dog.prototype.bark = function () {
  console.log(`Woof I am ${this.name}`);
};

const pet = new Dog('Mara');

pet.bark(); // Outputs: Woof I am Mara
```

**Explanation:** A `Dog` class is created with a constructor to assign the name to the dog. A method `bark` is added to `Dog`’s prototype, which allows all instances of `Dog` to use this method. A new instance of `Dog` named ‘Mara’ is created, and `pet.bark()` is called, which outputs “Woof I am Mara”.

**Example: String.prototype**

```jsx
// Adding a method to String.prototype
String.prototype.shout = function() {
  return this.toUpperCase() + '!!!';
};

let greeting = 'hello';
console.log(greeting.shout()); // Outputs: HELLO!!!
```

**Explanation:** Here, we add a method called `shout` to `String.prototype`. This means every string created in JavaScript will now have access to this `shout` method. The method converts the string to uppercase and adds exclamation marks.

**Example: Array.prototype**

```jsx
// Adding a method to Array.prototype
Array.prototype.firstElement = function() {
  return this.length > 0 ? this[0] : undefined;
};

let numbers = [1, 2, 3];
console.log(numbers.firstElement()); // Outputs: 1
```

**Explanation:** We add a method called `firstElement` to `Array.prototype`. This method returns the first element of an array if it exists. Now, any array we create will have this `firstElement` method available.

**Example: Object.prototype**

```jsx
// Adding a method to Object.prototype
Object.prototype.keysCount = function() {
  return Object.keys(this).length;
};

let person = { name: 'Alice', age: 25 };
console.log(person.keysCount()); // Outputs: 2
```

**Explanation:** we add a method called `keysCount` to `Object.prototype`. This method returns the number of keys (properties) in an object. By adding this method to `Object.prototype`, every object created in JavaScript, including `person`, now has access to the `keysCount` method. When we call `person.keysCount()`, it outputs `2` because there are two keys in the `person` object: `name` and `age`.

</p>
</details>

## 3. 🤝 What Are Promises in JavaScript?

<details><summary><b>Click to expand details</b></summary>
<p>

A promise is a special JavaScript object that connects the “producing code” (which performs an asynchronous operation) with the “consuming code” (which handles the result of that operation). Think of it as a subscription list: the promise ensures that the result will be available to all subscribed code when it’s ready.

### ✨ Simple Analogy

Imagine you’re making a reservation at a restaurant for your niece’s birthday party next week. When you make the reservation, the restaurant gives you a promise that a table will be available for you at the specified time. In this analogy:

- **👉 Producing code:** The restaurant staff (like a waiter) takes whatever time they need to prepare the table (the promised result).

- **👉 Promise:** The reservation itself acts as the promise. It ensures that the table will be ready for your party when you arrive.

**🧩 Now, let’s break down the key concepts of promises:**

1. **States of a Promise:**

    - **👉 Pending:** The promise is awaiting a response (like waiting for the table to be set).

    - **👉 Resolved (Fulfilled):** The promise has successfully returned a value (like when the table is ready).

    - **👉 Rejected:** The promise encountered an error (like when the restaurant couldn’t accommodate your reservation).

2. **Creating a Promise in JavaScript:**

    - 👉 You can create a promise using the ”Promise” constructor. It takes a callback function with two parameters: ”resolve” and ”reject”

    - 👉 Inside the callback, you perform your asynchronous operation (e.g., fetching data, loading an image, etc.).

    - 👉 If everything goes well, you call ”resolve” with the result. If there’s an error, you call ”reject” with an error message.

🧠 Remember, promises allow you to handle asynchronous operations more elegantly, making your code cleaner and easier to reason about. Just like a restaurant reservation, they ensure that the result will be available when needed! 🍽️

**🕹️ Now that we have basic understanding, lets go through the following examples.**

**Example: creating and using a promise**

```jsx
// Creating a promise
const reservationPromise = new Promise((resolve, reject) => {
  // Simulating an asynchronous operation (e.g., fetching data)
  const condition = true;

  if (condition) {
	  setTimeout(() => {
	    const data = 'Stuff worked!';
	    resolve(data); // Resolve the promise;
	  }, 2000); // Simulating a delay
  } else {
	  setTimeout(() => {
	      reject(Error('Promise is rejected.')); // Reject the promise;
	   }, 2000); // Simulating a delay
  }
});

// Consuming the promise
reservationPromise
  .then(result => {
    console.log('Promise worked!', result); // Handle success
  })
  .catch(err => {
    console.log('Something went wrong!', err.message); // Handle error
  });
```

**Explanation:** 

- We create a promise that resolves/reject based on the condition after a 2-second delay.
- If `condition` is `true`, it logs “Promise worked! Stuff worked!” to the console.
- If `condition` is `false`,  it logs “Something went wrong! Promise is rejected.” (you can customize the error message).

---

**Example: using __async/await__ with __Fetch API__**

```jsx
async function getData() {
  try {
    const response = await fetch('https://jsonplaceholder.typicode.com/posts');
    if (response.status === 200) {
      const data = await response.json(); // Await the JSON parsing
      return data;
    } else {
      throw new Error(`Error fetching data. Status: ${response.status}`);
    }
  } catch (error) {
    console.error('An error occurred:', error.message);
    // Handle the error gracefully (e.g., show a user-friendly message)
    return null;
  }
}

// Usage
try {
  const result = await getData();
  if (result && result.length > 0) {
    console.log('Data received:', result);
  } else {
    console.log('Failed to fetch data.');
  }
} catch (error) {
  console.error('An error occurred during data retrieval:', error.message);
}
```

**Explanation:** 

- The `getData` function is defined as an **async function**. This means it always returns a **promise**.
- We use `await` directly in the `getData()` function to wait for the `fetch` request to complete and handle the response.
- If the response status is 200, we parse the JSON data.
- If there’s an error (e.g., non-200 status or network issues), we throw an error and catch it in the `try`/`catch` block.
- The usage section demonstrates how to call the `getData()` function and handle the result or error.

</p>
</details>

## 4. 🗃️ What Are Closures in JavaScript?

<details><summary><b>Click to expand details</b></summary>

<p>

A closure is a fundamental concept in JavaScript. It occurs when a function “remembers” its lexical scope even after it has finished executing. In simpler terms, a closure allows a function to retain access to variables from its outer (enclosing) function, even when that outer function has completed execution.

### 🧩 Simple Analogy: The Picnic Basket

Imagine you’re going on a picnic with friends. You pack a picnic basket with all the essentials: sandwiches, fruits, drinks, and utensils. As you head to the park, you carry the basket with you. Now, here’s the interesting part: the basket itself is like a closure!

**❇️ The Basket (Closure):**

- ✨ The picnic basket encapsulates everything you need for the picnic.
- ✨ It “closes over” its contents, keeping them private and secure.
- ✨  Similarly, a closure in JavaScript encapsulates variables and functions within a specific context.

**🔥 How Do Closures Work?**

1. **ℹ️ Lexical Scope:**
    - ✨ JavaScript uses lexical scoping, which means that functions have access to variables defined in their containing (parent) functions.
    - ✨ When a function is defined, it “captures” its surrounding scope, creating a closure.
2. **ℹ️ Creating a Closure:** A closure is formed when:
    - ✨ An inner function is defined within an outer function.
    - ✨ The inner function references variables from the outer function.
    - ✨ The inner function is returned or passed as an argument to other functions.

### 🔥 Use Cases and Benefits

- **ℹ️ Data Privacy:**
    - ✨ By enclosing variables within a closure, you create private variables.
    - ✨ These variables are accessible only within the closure’s scope, providing data privacy.
    - ✨ This approach emulates private methods in object-oriented programming.
- **ℹ️ Function Factories:**
    - ✨ You can generate specialized functions (function factories) using closures. For instance, consider a function that generates related functions based on an initial value.
- **ℹ️ Event Handling:**
    - ✨ When you attach an event handler (like a click event) to an HTML element, you’re creating a closure.
    - ✨ The event handler function “remembers” the surrounding context (variables, functions) - even after it’s detached from the element.
- **ℹ️ Timeouts and Intervals:**
    - ✨ Closures are essential for managing timeouts and intervals, ’setTimeout’ or ’setInterval’.
    - ✨ They ensure that the correct context is maintained when the callback executes.

**🕹️ Now that we have the understanding, lets go through the following examples.**

**Example: Data Privacy**

```jsx
function createCounter() {
  let count = 0;
  return function() {
    count += 1;
    return count;
  };
}

const counter = createCounter();
console.log(counter()); // 1
console.log(counter()); // 2
// 'count' is not accessible from outside the 'createCounter' function.
```

**Explanation:** 

- The `createCounter` function encapsulates a `count` variable. It returns an anonymous function that, when called, increments `count` and returns its value.
- The `count` variable is private and cannot be accessed or modified directly outside of `createCounter`.**

---

**Example: Function Factories**

```jsx
function makeMultiplier(multiplier) {
  return function(number) {
    return number * multiplier;
  };
}

const double = makeMultiplier(2);
console.log(double(5)); // 10
```

**Explanation:** 

- The `makeMultiplier` function takes a `multiplier` argument and returns a new function. This returned function takes a `number` argument and returns the product of `number` and `multiplier`.
- Each function created by `makeMultiplier` retains its own `multiplier` value.

---

**Example: Event Handling**

```jsx
let countClicks = (function() {
  let count = 0;
  return function() {
    count += 1;
    console.log(`Button clicked ${count} times`);
  };
})();

document.getElementById('myButton').addEventListener('click', countClicks);
```

**Explanation:**

- The `countClicks` IIFE (Immediately Invoked Function Expression) creates a private `count` variable for counting clicks.
- The returned function is used as an event handler for clicks, which increments the count and logs it to the console.

---

**Example: Timeouts and Intervals**

```jsx
function delayedAlert(message, delay) {
  setTimeout(function() {
    alert(message);
  }, delay);
}

delayedAlert('Hello after 2 seconds', 2000);
```

**Explanation:** 

- The `delayedAlert` function demonstrates a closure where the `message` and `delay` parameters are used by the anonymous function inside the `setTimeout`.
- Even after `delayedAlert` has finished executing, the callback function can still access the `message` and `delay`.

</p>
</details>