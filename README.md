<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png">
  <h1>JavaScript: Learn Unlearn & Relearn 🔄</h1>
</div>

Test your **JavaScript knowledge**, refresh important concepts, or **prepare for an interview** with this **comprehensive guide**! 💪 Whether you're a **beginner or intermediate** learner, this document will help you **strengthen your understanding** with **detailed explanations, multiple examples, common mistakes, and real-world applications.**

I created this for **fun and learning in free time**, so please **forgive any mistakes**! If you find it helpful, I’d truly **appreciate a ⭐️ or a reference to this repo**. <br>
Best of luck on your **programming journey**—🙏✨ **Happy coding!** 🧑‍💻

<p align="center">
💬 In case you want to reach out or just say hi, ↩️ <br/>
<a href="https://www.facebook.com/saiefalemon">Facebook</a> | <a href="https://www.linkedin.com/in/saiefalemon">LinkedIn</a> | <a href="https://www.iamsaief.com/">Blog</a>
</p>

---

**🗂️ Table of Contents:**

- [1. 🧐 **Truthy** and **Falsy** in JavaScript](#1--truthy-and-falsy-in-javascript)
- [2. 👨‍👩‍👧‍👦 Prototypal Inheritance in JavaScript](#2--prototypal-inheritance-in-javascript)
- [3. 📜 Promises in JavaScript](#3--promises-in-javascript)
- [4. 🎭 Closures in JavaScript](#4--closures-in-javascript)
- [5. 🔄 JavaScript Event Loop \& Asynchronous Behavior](#5--javascript-event-loop--asynchronous-behavior)
- [6. 🔥 Why `this` in JavaScript Can Be Confusing (And How to Master It)](#6--why-this-in-javascript-can-be-confusing-and-how-to-master-it)
- [7. 💡 `call`, `apply`, and `bind`: The Superpowers of JavaScript Functions](#7--call-apply-and-bind-the-superpowers-of-javascript-functions)
- [8. 🚀 `map`, `filter`, and `reduce` Explained Like You’re Five](#8--map-filter-and-reduce-explained-like-youre-five)
- [9. ⏳ How `setTimeout` and `setInterval` Work in JavaScript (And Why They Matter)](#9--how-settimeout-and-setinterval-work-in-javascript-and-why-they-matter)
- [10. 🔄 `async` and `await`: The Easiest Way to Handle Promises](#10--async-and-await-the-easiest-way-to-handle-promises)
- [11. 📦 How to Use `JSON` and `localStorage` to Save Data](#11--how-to-use-json-and-localstorage-to-save-data)
- [12. 🏗️ ES6 Classes: The Simple Way to Write Object-Oriented Code](#12-️-es6-classes-the-simple-way-to-write-object-oriented-code)
- [13. 🚨 Why You Should Always Use `"use strict"` in JavaScript](#13--why-you-should-always-use-use-strict-in-javascript)
- [14. 🛡️ `try...catch` : The Secret to Handling Errors Like a Pro](#14-️-trycatch--the-secret-to-handling-errors-like-a-pro)
- [15. 🔑 The Power of `Object.keys()`, `Object.values()`, and `Object.entries()`](#15--the-power-of-objectkeys-objectvalues-and-objectentries)
- [16. ⏱️ _Debounce_ and _Throttle_ in JavaScript: Control When Your Functions Fire](#16-️-debounce-and-throttle-in-javascript-control-when-your-functions-fire)
- [17. 🎯 Event _Delegation_ in JavaScript: Handle More with Less](#17--event-delegation-in-javascript-handle-more-with-less)
- [18. 🎛️ Understanding Event Bubbling and Capturing in JavaScript](#18-️-understanding-event-bubbling-and-capturing-in-javascript)

---

Available In: [🇧🇩 বাংলা](./bn-BD/README_bn-BD.md)

---

## 1. 🧐 **Truthy** and **Falsy** in JavaScript

In JavaScript, values are classified as either **truthy** or **falsy** when used in Boolean contexts (like conditionals). Understanding this classification is crucial for writing clean and predictable code.

### 🔹 Primitive Types

Primitive types represent single, immutable values:

| **Type**    | **Examples**                | **Behavior in Boolean Context**         |
| ----------- | --------------------------- | --------------------------------------- |
| `undefined` | `undefined`                 | Falsy                                   |
| `null`      | `null`                      | Falsy                                   |
| `boolean`   | `true`, `false`             | True is truthy, False is falsy          |
| `number`    | `42`, `0`, `NaN`            | Zero & NaN are falsy, others are truthy |
| `string`    | `"Hello"`, `""`             | Empty string is falsy, others truthy    |
| `symbol`    | `Symbol("id")`              | Always truthy                           |
| `BigInt`    | `BigInt(1234)`, `BigInt(0)` | Zero is falsy, others truthy            |

**🧐 Key Observations**

- Primitive values directly hold their data in memory.
- Some primitives (`0`, `false`, `""`, `null`, `undefined`, or `NaN`) are falsy, meaning they behave as `false` in Boolean contexts.

### 🔹 Reference Types

Reference types include **objects** such as **arrays**, **functions**, and other complex structures.

**🧐 Key Observations**

- Objects (including **arrays** and **functions**) are always **truthy**, even when empty (`[]`, `{}`).
- JavaScript allocates memory for reference types, and variables store a **pointer to the memory location** rather than the actual value.

### 🔹 Why Are Function Constructors Truthy?

Function constructors like `new Number(0)` or `new Boolean(false)` wrap primitive values inside objects. These objects are **reference types**, making them truthy regardless of the contained value.

**Example:**

```js
console.log(Boolean(new Boolean(false))); // true
```

### 🎭 Analogy: Folder vs. Paper

Think of primitive values as **papers**—some blank (falsy) and some written on (truthy). Objects, on the other hand, are **folders** holding those papers. Even if a folder contains a blank paper (`new Boolean(false)`), the folder itself exists, making it truthy.

**✅ Summary**

- Primitive types store values directly; some are truthy, others falsy.
- Objects and reference types are always truthy.
- Function constructors return objects, making them truthy, even if their contents are falsy.

<br>

## 2. 👨‍👩‍👧‍👦 Prototypal Inheritance in JavaScript

JavaScript's prototypal inheritance allows objects to inherit properties and methods from a **prototype object**, enabling reusable and memory-efficient code.

### 🔹 What is a Prototype?

A **prototype** is an object that provides shared properties and behaviors for multiple instances.

### 🧐 Key Observations

- Every function has a `prototype` property, which is used for creating objects.
- Objects created from the same constructor **inherit** methods from the prototype.
- Modifying the prototype affects all instances derived from it.

### 🔹 Simple Analogy: Recipe for a Cake

A **prototype** is like a cake recipe. All cakes made from that recipe inherit its properties (flavors, layers). If the recipe changes (adding icing), all future cakes will include the new change.

**🔹 Key Advantages**

- **✅ Memory Efficiency** – Objects share prototype methods, avoiding redundant copies.
- **✅ Dynamic Extension** – Modifying a prototype extends functionality to all objects inheriting from it.

**⚠️ Handle with Care**

Modifying built-in prototypes (`Object.prototype`, `Array.prototype`) is **not recommended**, as it may introduce conflicts with external libraries.

**✅ Summary**

- Objects inherit properties and methods from a prototype.
- Modifying a prototype applies changes to all instances.
- Use prototypal inheritance carefully to ensure predictable behavior.

### 📝 Practical Examples

**📝 Example: Barking Dog**

```js
class Dog {
  constructor(name) {
    this.name = name;
  }
}

Dog.prototype.bark = function () {
  console.log(`Woof I am ${this.name}`);
};

const pet = new Dog("Mara");
pet.bark(); // Outputs: Woof I am Mara
```

**💡 Explanation:**

- A `Dog` **class** is created with a name property.
- The `bark()` method is added to `Dog.prototype`, making it available to all instances.
- Calling `pet.bark()` outputs "Woof I am Mara".

**📝 Example: Extending `String.prototype`**

```js
String.prototype.shout = function () {
  return this.toUpperCase() + "!!!";
};

console.log("hello".shout()); // Outputs: HELLO!!!
```

**💡 Explanation:**

- The `shout()` method is added to `String.prototype`, allowing all string instances to use it.

**Example: Array Prototype Extension**

```js
Array.prototype.firstElement = function () {
  return this.length > 0 ? this[0] : undefined;
};

console.log([1, 2, 3].firstElement()); // Outputs: 1
```

**💡Explanation:**

- A custom method `firstElement()` returns the first element of an array.

**📝 Example: Extending `Object.prototype`**

```js
Object.prototype.keysCount = function () {
  return Object.keys(this).length;
};

console.log({ name: "Alice", age: 25 }.keysCount()); // Outputs: 2
```

**💡 Explanation:**

- A method `keysCount()` is added to `Object.prototype` to count properties of an object.

<br>

## 3. 📜 Promises in JavaScript

A **Promise** is a JavaScript object that represents the eventual completion (or failure) of an **asynchronous operation**. It allows the **producing code** (which performs an operation) to connect with the **consuming code** (which handles the result), ensuring a structured approach to async logic.

### 🔹 Analogy: Restaurant Reservation

Think of **Promises** like making a restaurant reservation:

- **Producing Code →** The restaurant staff prepares your table (async operation).
- **Promise →** Your reservation guarantees that the table will be ready when you arrive.

If everything goes smoothly, you **get a table (resolve)**. If there's an issue, like the restaurant being full, **your reservation gets canceled (reject)**.

### 🔹 States of a Promise

A promise can have one of **3 states**:

| **State**     | **Description**                                   |
| ------------- | ------------------------------------------------- |
| **Pending**   | The operation is still in progress.               |
| **Fulfilled** | The operation completed successfully (`resolve`). |
| **Rejected**  | The operation failed (`reject`).                  |

### 🔹 Creating a Promise

To create a promise, use the Promise constructor:

```js
const myPromise = new Promise((resolve, reject) => {
  let success = true; // Simulated condition
  setTimeout(() => {
    success ? resolve("Data received!") : reject("Error occurred!");
  }, 2000);
});
```

### 🔹 Consuming a Promise

Use `.then()` and `.catch()` to handle promise results:

```js
myPromise.then((message) => console.log("Success:", message)).catch((error) => console.log("Failure:", error));
```

#### 🔹 Async/Await Approach

Using `async/await` for better readability:

```js
async function fetchData() {
  try {
    const response = await fetch("https://jsonplaceholder.typicode.com/posts");
    if (!response.ok) throw new Error(`Failed with status: ${response.status}`);
    const data = await response.json();
    console.log("Data:", data);
  } catch (error) {
    console.error("Error:", error.message);
  }
}
fetchData();
```

**✅ Summary**

- Promises handle **asynchronous operations** efficiently.
- They can be **pending, fulfilled, or rejected**.
- Use `.then()` and `.catch()` for chaining.
- `async`/`await` provides a cleaner syntax for handling async operations.

<br>

## 4. 🎭 Closures in JavaScript

A **Closure** is when a function retains access to its **lexical scope**, even after the outer function has **finished execution**. Closures allow functions to "remember" variables from their **enclosing scope**, even when invoked later.

### 🔹 Analogy: The Picnic Basket

Closures work like picnic baskets:

- You pack **sandwiches, drinks, utensils** (variables).
- Even when you leave home, **your basket holds everything**.
- Similarly, a function carries its **enclosed variables** wherever it goes!

### 🔹 How Closures Work

Closures form when:

1. A **function is defined inside another function**.
2. The inner function **accesses variables from the outer function**.
3. The inner function **remains available even after the outer function completes**.

### 🔹 Practical Applications

- **✅ Data Privacy** – Keep variables private inside a function scope.
- **✅ Function Factories** – Generate customized functions dynamically.
- **✅ Event Handling** – Preserve state when attaching event handlers.
- **✅ Timeouts/Intervals** – Maintain access to variables even with delays.

**📝 Example: Data Privacy**

```js
function createCounter() {
  let count = 0;
  return function () {
    return ++count;
  };
}
const counter = createCounter();
console.log(counter()); // 1
console.log(counter()); // 2
```

**✨ Explanation:** The `count` variable is private and persists between function calls.

**📝 Example: Function Factory**

```js
function multiplier(x) {
  return function (num) {
    return num * x;
  };
}
const double = multiplier(2);
console.log(double(5)); // 10
```

**✨ Explanation:** The returned function retains `x` from `multiplier()`.

**📝 Example: Event Handling**

```js
(function () {
  let clickCount = 0;
  document.getElementById("myButton").addEventListener("click", function () {
    clickCount++;
    console.log(`Clicked ${clickCount} times`);
  });
})();
```

**✨ Explanation:** The event handler maintains `clickCount`, even after multiple clicks.

**✅ Summary**

- Closures allow functions to **retain access to outer variables**.
- Useful for **data privacy, event handling, and function factories**.
- **`setTimeout`**, **event listeners**, and **async logic** rely on closures.

<br>

## 5. 🔄 JavaScript Event Loop & Asynchronous Behavior

JavaScript is **single-threaded**, meaning it executes **one task at a time**. But it can handle **asynchronous tasks** efficiently using the **event loop**. This allows JavaScript to **stay responsive** while waiting for tasks like data fetching or timers.

### 🧐 How It Works

#### 1️⃣ Main Thread

- JavaScript executes **synchronous** code **line by line**.
- Tasks like calculations and function calls happen immediately.

#### 2️⃣ Asynchronous Tasks

- Some operations take time, like **fetching data** or **waiting for user input**.
- These tasks are **delegated** to the browser's **Web APIs** (e.g., `setTimeout`, `fetch`).
- JavaScript **keeps running other code** while waiting for results.

#### 3️⃣ Callback Queue

- Once an **async task finishes**, its callback (function) is placed in the **callback queue**.
- The callback queue holds **tasks waiting to be executed**.

#### 4️⃣ Event Loop

- Constantly **checks if the main thread is free**.
- If the **call stack is empty**, it **takes tasks from the callback queue** and runs them.

---

### ⏱️ `setTimeout` & Web APIs

When you use `setTimeout()`, JavaScript **does NOT pause**—instead:

1. **It delegates the timer** to Web APIs.
2. The main thread **keeps running** other code.
3. Once the timer finishes, the **callback moves to the callback queue**.
4. The **event loop picks it up** when the call stack is empty.

**📝 Example: `setTimeout`**

```js
console.log("Start");

setTimeout(() => {
  console.log("Timeout callback");
}, 1000);

console.log("End");

// Output:
// "Start"
// "End"
// (After 1 second) "Timeout callback"
```

**💡 Explanation:**

- `Start` and `End` run **immediately**.
- `setTimeout()` schedules the callback but **doesn’t block execution**.
- **After 1 second**, the event loop runs the callback from the queue.

---

### 🤝 Promises & Microtask Queue

Promises handle async tasks **efficiently** using the **microtask queue**, which has **higher priority** than the callback queue.

**🧐 How Promises Work**

- A **promise** holds a future value (like API data).
- When a promise **resolves or rejects**, its `.then()` or `.catch()` callback is scheduled.
- The event loop **always checks the microtask queue first** before running normal callbacks.

**📝 Example: Promise Execution**

```js
const fetchData = () => {
  return new Promise((resolve) => {
    setTimeout(() => resolve("Data fetched"), 1000);
  });
};

fetchData().then((result) => {
  console.log(result);
});

console.log("Fetching data...");

// Output:
// "Fetching data..."
// (After 1 second) "Data fetched"
```

**💡 Explanation:**

- The `fetchData` function **returns a promise** that resolves **after 1 second**.
- The `.then()` callback **waits** until the promise resolves.
- Meanwhile, JavaScript **continues executing** other code.

**🔁 Summary**

- ✅ JavaScript is **single-threaded** but uses the **event loop** to handle async tasks.
- ✅ `setTimeout()` uses the **callback queue**, while promises use the **microtask queue** (which is processed **first**).
- ✅ The **event loop keeps JavaScript responsive**, ensuring tasks run efficiently.

<br>

## 6. 🔥 Why `this` in JavaScript Can Be Confusing (And How to Master It)

- ✅ Implicit vs. Explicit Binding <br>
- ✅ Arrow Functions and Lexical `this` <br>
- ✅ Common Pitfalls and Fixes <br>

### 💡 Simple Analogy: A Personal Assistant with Multiple Bosses

Imagine an assistant who works for different bosses depending on the situation. Sometimes, they know exactly who to report to, but in tricky cases, they might get confused. **Similarly `this` refers to different objects depending on how and where a function is called**.

### 🔍 Understanding `this` in Different Contexts

**📝 Example 1: Implicit Binding (How `this` Works Inside an Object Method)**

```javascript
const person = {
  name: "Alice",
  greet() {
    console.log(`Hello, my name is ${this.name}`);
  },
};

person.greet(); // Outputs: Hello, my name is Alice
```

**💡 Explanation:**

Since `this` is inside the greet method, it correctly refers to the `person` object.

**📝 Example 2: Explicit Binding with `call`, `apply`, and `bind`**

```javascript
function sayHello() {
  console.log(`Hello, my name is ${this.name}`);
}

const user = { name: "John" };

sayHello.call(user); // Outputs: Hello, my name is John
```

**💡 Explanation:**

We explicitly define `this` using `.call()`, making sure it refers to `user`.

**📌 Common Mistake:**

Forgetting to bind this properly inside event listeners or callbacks can lead to errors!

**📝 Example 3: Arrow Functions and Lexical `this`**

```javascript
const student = {
  name: "Emma",
  subjects: ["Math", "Science"],
  showSubjects() {
    this.subjects.forEach((subject) => console.log(`${this.name} studies ${subject}`));
  },
};

student.showSubjects();
// Outputs: Emma studies Math
// Emma studies Science
```

**💡 Explanation:**

Arrow functions **do not** have their own `this`, so they inherit it from their surrounding function (`showSubjects`).

### 📌 Where You’ll See This in the Real World

- Debugging why `this` is `undefined` inside callbacks
- Ensuring correct `this` binding for class methods
- Fixing unexpected behavior in event listeners

<br>

## 7. 💡 `call`, `apply`, and `bind`: The Superpowers of JavaScript Functions

- ✅ Borrowing Methods from Other Objects
- ✅ Key Differences Between Them
- ✅ Real-World Applications

### 💡 Simple Analogy: Borrowing Someone's Car

Imagine your friend owns a car, but you need to drive it.

- `call` lets you drive it immediately.
- `apply` works the same, but asks you to list passengers in an array (arguments).
- `bind` hands you the keys, but you can drive whenever you want.

### 🔍 Understanding How These Methods Work

**📝 Example 1: Using `call` to Invoke a Function with a Custom Context**

```javascript
const person1 = { name: "Alice" };
const person2 = { name: "Bob" };

function introduce(age) {
  console.log(`Hi, I'm ${this.name} and I'm ${age} years old.`);
}

introduce.call(person1, 25); // Outputs: Hi, I'm Alice and I'm 25 years old.
introduce.call(person2, 30); // Outputs: Hi, I'm Bob and I'm 30 years old.
```

**💡 Explanation:** `.call()` lets us execute the function immediately while assigning `this` to `person1` or `person2`.

**📝 Example 2: Using `apply` to Pass Arguments as an Array**

```javascript
introduce.apply(person1, [25]); // Outputs: Hi, I'm Alice and I'm 25 years old.
introduce.apply(person2, [30]); // Outputs: Hi, I'm Bob and I'm 30 years old.
```

**💡 Explanation:** `.apply()` works the same as `.call()`, but requires arguments in an array.

**📝 Example 3: Using `bind` to Return a New Function**

```javascript
const boundFunction = introduce.bind(person1, 28);
boundFunction(); // Outputs: Hi, I'm Alice and I'm 28 years old.
```

**💡 Explanation:** `.bind()` doesn't execute immediately—it creates a new function that remembers `this`.

### 📌 Where You’ll See This in the Real World

- Borrowing array methods for objects
- Setting event listeners while preserving `this`
- Ensuring correct `this` binding inside asynchronous functions

<br>

## 8. 🚀 `map`, `filter`, and `reduce` Explained Like You’re Five

- ✅ Transforming Data in Arrays
- ✅ When and How to Use Them
- ✅ Multiple Real-Life Examples

### 💡 Simple Analogy: Sorting Clothes

Imagine you’re organizing a pile of clothes:

- `map` irons all items neatly.
- `filter` removes worn-out pieces.
- `reduce` folds everything into a neat bundle.

### 🔍 Understanding Each Method

**📝 Example 1: Using `map` to Modify Items in an Array**

```javascript
const numbers = [1, 2, 3, 4, 5];

const doubled = numbers.map((n) => n * 2);
console.log(doubled); // Outputs: [2, 4, 6, 8, 10]
```

**💡 Explanation:** Each item in the array is transformed without changing the original array.

**📝 Example 2: Filtering Specific Values**

```javascript
const ages = [12, 20, 17, 25, 30];

const adults = ages.filter((age) => age >= 18);
console.log(adults); // Outputs: [20, 25, 30]
```

**💡 Explanation:** `filter` removes values that don’t match the condition.

**📝 Example 3: Using `reduce` to Sum Up Values**

```javascript
const prices = [10, 20, 30, 40];

const totalPrice = prices.reduce((total, price) => total + price, 0);
console.log(totalPrice); // Outputs: 100
```

**💡 Explanation:** `reduce` starts at zero, then adds each item.

### 📌 Where You’ll See This in the Real World

- Modifying and transforming data in APIs
- Filtering user lists based on conditions
- Summing up totals in e-commerce applications

<br>

## 9. ⏳ How `setTimeout` and `setInterval` Work in JavaScript (And Why They Matter)

- ✅ Scheduling Tasks Like a Pro
- ✅ Understanding Web APIs and Delayed Execution
- ✅ Clearing Timers with `clearTimeout` and `clearInterval`

### 💡 Simple Analogy: Alarm Clock vs. Recurring Notifications

- `setTimeout` acts like an alarm—it rings once after a delay.
- `setInterval` behaves like recurring notifications—it rings repeatedly at set intervals.

### 🔍 Understanding How Each Works

**📝 Example 1: Using `setTimeout` to Delay Execution**

```javascript
setTimeout(() => console.log("Hello after 2 seconds"), 2000);
```

**💡 Explanation:** The function inside `setTimeout` waits for 2 seconds before executing, allowing other code to continue running in the meantime.

**📝 Example 2: Using `setInterval` to Run a Function Repeatedly**

```javascript
let counter = 0;

const interval = setInterval(() => {
  counter++;
  console.log(`Count: ${counter}`);
  if (counter === 5) clearInterval(interval); // Stop after 5 repetitions
}, 1000);
```

**💡 Explanation:** `setInterval` runs every second until `counter` reaches 5, at which point we call `clearInterval()` to stop it.

### 📌 Where You’ll See This in the Real World

- **Countdown timers** (e.g., auction bidding, flash sales)
- **Auto-refreshing notification**s (e.g., live sports scores)
- **Delayed animations** (e.g., showing tooltips after hovering)

<br>

## 10. 🔄 `async` and `await`: The Easiest Way to Handle Promises

- ✅ Say Goodbye to Callback Hell
- ✅ Writing Clean, Maintainable Asynchronous Code
- ✅ Handling Errors in Async Functions

### 💡 Simple Analogy: Ordering Food Online

You place an order at a restaurant (**promise**) and wait (**await**) for your food before eating.

### 🔍 Understanding Asynchronous Behavior

**📝 Example 1: Basic `async` and `await` Usage**

```javascript
async function fetchData() {
  let response = await fetch("https://jsonplaceholder.typicode.com/todos/1");
  let data = await response.json();
  console.log(data);
}

fetchData();
```

**💡 Explanation:** `await` **pauses execution until the fetch request completes**, ensuring we don’t access `data` before it’s available.

**📝 Example 2: Handling Errors in Async Code**

```javascript
async function fetchUserData() {
  try {
    let response = await fetch("https://invalid-url.com");
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.log("Error fetching data:", error.message);
  }
}

fetchUserData();
```

**💡 Explanation:** Wrapping code inside `try...catch` **prevents the entire script from breaking** if the request fails.

### 📌 Where You’ll See This in the Real World

- **Fetching data from APIs** (e.g., retrieving user profiles)
- **Handling authentication flows** (e.g., logging in users)
- **Waiting for animations to complete** (e.g., fading effects in UI)

<br>

## 11. 📦 How to Use `JSON` and `localStorage` to Save Data

- ✅ Storing and Retrieving Data Easily
- ✅ Converting Objects to Strings
- ✅ Making Data Persistent

### 💡 Simple Analogy: Writing Notes in a Notebook

Think of `localStorage` as a **notebook** where you can write information and retrieve it later—even after closing the browser.

### 🔍 Understanding Data Storage

**📝 Example 1: Storing and Retrieving Data in `localStorage`**

```javascript
const user = { name: "Alice", age: 25 };

localStorage.setItem("user", JSON.stringify(user));
const retrievedUser = JSON.parse(localStorage.getItem("user"));

console.log(retrievedUser.name); // Outputs: Alice
```

**💡 Explanation:** `localStorage` **only stores strings**, so we use `JSON.stringify()` to store and `JSON.parse()` to retrieve structured data.

**📝 Example 2: Removing and Clearing Storage**

```javascript
localStorage.removeItem("user"); // Deletes specific data
localStorage.clear(); // Clears all stored data
```

**💡 Explanation:** `removeItem` **deletes one item**, while `clear` **wipes everything from storage**.

### 📌 Where You’ll See This in the Real World

- **Saving user preferences** (dark mode, language settings)
- **Storing shopping cart data** in e-commerce websites
- **Keeping temporary form inputs** (e.g., auto-filled contact details)

<br>

## 12. 🏗️ ES6 Classes: The Simple Way to Write Object-Oriented Code

- ✅ Creating Reusable Object Templates
- ✅ Understanding Constructors and Methods
- ✅ Inheritance with Classes

### 💡 Simple Analogy: A Toy Factory

A toy factory **produces different types of toys**, but they all **share a common blueprint**. **Classes** work the same way in JavaScript—they allow you to create multiple objects using a shared structure.

### 🔍 Understanding ES6 Classes

**📝 Example 1: Defining and Using a Class**

```javascript
class Toy {
  constructor(name, price) {
    this.name = name;
    this.price = price;
  }
  display() {
    console.log(`${this.name} costs $${this.price}`);
  }
}

const toyCar = new Toy("Car", 10);
toyCar.display(); // Outputs: Car costs $10
```

**💡 Explanation:** The `Toy` class acts as a **template**, allowing us to create multiple toy objects with shared properties and behaviors.

**📝 Example 2: Inheriting from Another Class**

```javascript
class Vehicle {
  constructor(type) {
    this.type = type;
  }
}

class Car extends Vehicle {
  constructor(brand, model) {
    super("Car");
    this.brand = brand;
    this.model = model;
  }
}

const myCar = new Car("Tesla", "Model X");
console.log(myCar.type); // Outputs: Car
console.log(myCar.brand); // Outputs: Tesla
```

**💡 Explanation:** **`Car` inherits from `Vehicle`**, meaning all cars automatically have the `type` property.

### 📌 Where You’ll See This in the Real World

- **Modeling game characters** (e.g., player stats in RPGs)
- **Structuring reusable UI components** in React
- **Managing user profiles in web apps** (e.g., administrator, editor, viewer roles)

<br>

## 13. 🚨 Why You Should Always Use `"use strict"` in JavaScript

- ✅ Avoiding Common Mistakes and Bugs
- ✅ Making Code Safer and More Predictable
- ✅ Preventing Accidental Global Variables

### 💡 Simple Analogy: A Strict Teacher Enforcing Rules

Strict mode **forces better coding practices** and prevents accidental errors.

### 🔍 Understanding Strict Mode

**📝 Example 1: Preventing Undeclared Variables**

```javascript
"use strict";

x = 10; // Error! `x` is not declared
```

**💡 Explanation:** Without `"use strict"`, JavaScript **allows undeclared variables**, which can cause unexpected bugs.

**📝 Example 2: Restricting Accidental Modifications to Objects**

```javascript
"use strict";

const person = Object.freeze({ name: "Alice" });

person.name = "Bob"; // Error! Object properties cannot be changed
```

**💡 Explanation:** `"use strict"` **ensures objects remain immutable when frozen**.

### 📌 Where You’ll See This in the Real World

- **Writing safer JavaScript for production**
- **Avoiding silent errors in large applications**
- **Improving debugging by catching mistakes early**

<br>

## 14. 🛡️ `try...catch` : The Secret to Handling Errors Like a Pro

- ✅ Preventing Unexpected Breakdowns
- ✅ Catching and Debugging Issues
- ✅ Writing Safer Code

### 💡 Simple Analogy: A Safety Net for Your Code

Imagine you’re walking on a tightrope. **Without a safety net, one mistake can cause a disaster**. In JavaScript, errors can completely stop execution—but `try...catch` **acts as a safety net**, preventing the script from crashing.

### 🔍 Handling Errors with `try...catch`

**📝 Example 1: Basic Error Handling**

```javascript
try {
  let result = 5 / 0;
  console.log(result);
} catch (error) {
  console.log("Error occurred:", error.message);
}
```

**💡 Explanation:** If an error happens inside `try`, execution **jumps** to `catch`, preventing the program from crashing.

**📝 Example 2: Handling API Errors**

```javascript
async function fetchData() {
  try {
    let response = await fetch("https://jsonplaceholder.typicode.com/invalid");
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.log("Failed to fetch data:", error.message);
  }
}

fetchData();
```

**💡 Explanation:** If the API request fails, instead of breaking the program, `catch` **handles the error gracefully**.

### 📌 Where You’ll See This in the Real World

- **Debugging API failures** (handling network issues)
- **Managing user input validation** (preventing invalid data from breaking forms)
- **Safeguarding critical operations** (error-proofing database transactions)

<br>

## 15. 🔑 The Power of `Object.keys()`, `Object.values()`, and `Object.entries()`

- ✅ Extracting Object Data Easily
- ✅ Making Object Manipulation Simpler
- ✅ Converting Objects into Arrays

### 💡 Simple Analogy: Organizing a Locker

Imagine **a locker with multiple compartments**—each holds valuable items (data). These methods help you **retrieve the names, values, or full details of every compartment in an organized way**.

### 🔍 Extracting Data Efficiently

**📝 Example 1: Getting Object Keys**

```javascript
const person = { name: "Alice", age: 25 };

console.log(Object.keys(person)); // ["name", "age"]
```

**💡 Explanation:** `Object.keys()` **returns an array of property names**, making it easy to loop over objects dynamically.

**📝 Example 2: Getting Object Values**

```javascript
console.log(Object.values(person)); // ["Alice", 25]
```

**💡 Explanation:** `Object.values()` returns an **array of values**, allowing you to process data easily.

**📝 Example 3: Getting Both Keys and Values Together**

```javascript
console.log(Object.entries(person)); // [["name", "Alice"], ["age", 25]]
```

**💡 Explanation:** `Object.entries()` returns **both keys and values**, making objects behave like arrays.

### 📌 Where You’ll See This in the Real World

- **Transforming objects into arrays** (useful in database queries)
- **Dynamically filtering object data** (like sorting user profiles)
- **Extracting configuration settings** (handling complex app settings)

<br>

## 16. ⏱️ _Debounce_ and _Throttle_ in JavaScript: Control When Your Functions Fire

- **✅ Stop your functions from going wild.**
- **✅ Prevent Laggy UIs**
- **✅ Optimize Expensive Computations, Master efficient event handling**

### 🧠 Simple Analogy: Timing the Talkers

Imagine someone mashing the talk button in a group call.

- **Debounce:** Only let them speak if they stop pressing it for 3 full seconds.
- **Throttle:** Let them speak once every 3 seconds, no matter how often they mash.

That’s how you **manage excessive events in the browser**—keeping things responsive without overreacting.

### 🧪 Example 1: Debounce – Wait Until the User Stops Typing

```javascript
function searchQuery() {
  console.log("Searching...");
}

function debounce(func, delay) {
  let timeout;
  return (...args) => {
    clearTimeout(timeout);
    timeout = setTimeout(() => func(...args), delay);
  };
}

const optimizedSearch = debounce(searchQuery, 300);
optimizedSearch(); // Only runs if no call happens again within 300ms
```

**💡 Explanation (Clean and Clear):**

- `debounce(func, delay)` wraps your real function (`func`) and adds timing control.
- `let timeout;` stores a reference to the latest scheduled task.
- `clearTimeout(timeout);` **cancels the previous run every time** you trigger the function.
- `setTimeout(..., delay);` starts a new timer that **delays the actual function call**.

**📌 Why it matters:**

- The function only executes if there’s a **pause** in activity (e.g., user stops typing).
- Every keystroke resets the timer—**only the last one counts**.

**🛠 Use debounce for:**

- Search bars
- Auto-saving while typing
- Responsive input validation

### 🧪 Example 2: Throttle – Limit Calls to Once Every X ms

```javascript
function logScrollPosition() {
  console.log("Scrolling...");
}

function throttle(func, limit) {
  let lastCall = 0;
  return (...args) => {
    const now = Date.now();
    if (now - lastCall >= limit) {
      lastCall = now;
      func(...args);
    }
  };
}

const optimizedScroll = throttle(logScrollPosition, 500);
document.addEventListener("scroll", optimizedScroll);
```

**💡 Explanation (Just What You Need):**

- `throttle(func, limit)` ensures your **function can’t run more than once every `limit`** milliseconds.
- `let lastCall = 0;` tracks the last time the function was executed.
- `Date.now()` provides a fresh timestamp on every event.
- `if (now - lastCall >= limit)` checks whether enough time has passed.
- If yes, it updates `lastCall` and runs the function.

**📌 Why it matters:**

- The function runs at regular intervals—even if the event (e.g., scroll) happens constantly.
- This keeps performance stable and avoids overwhelming your app.

**🛠 Use throttle for:**

- Scroll listeners
- Resize events
- Button spam prevention

### ❌ Common Pitfalls and How to Avoid Them

| ⚠️ Mistake                  | ❌ Why It Hurts                    | ✅ What to Do Instead                                                 |
| --------------------------- | ---------------------------------- | --------------------------------------------------------------------- |
| Debouncing scroll events    | Misses frequent updates            | **Use throttle for consistent pacing**                                |
| Forgetting to clear timeout | Triggers unwanted executions       | **Always call** `clearTimeout()` **first**                            |
| Arbitrary timing values     | UI feels laggy or overly sensitive | **Start with** `300ms` **for debounce,** `100–250ms` **for throttle** |

### 🌍 Real-World Use Cases

**Debounce**

- Typing in a search box
- Auto-saving text input
- Validating input after pause

**Throttle**

- Tracking scroll position
- Animating based on scroll
- Rate-limiting frequent API hits

### 🧾 TL;DR

| Technique    | What It Does                                     | Great For                                       |
| ------------ | ------------------------------------------------ | ----------------------------------------------- |
| **Debounce** | Runs only after user stops triggering events     | Live search, input cleanup, smooth UX           |
| **Throttle** | Runs at most once every X ms during rapid events | Scrolling, resizing, rate-limiting interactions |

<br>

## 17. 🎯 Event _Delegation_ in JavaScript: Handle More with Less

- **✅ Reduce Event Listeners**
- **✅ Simplify DOM Management**
- **✅ Support Dynamic Elements with Ease**

### 🧠 Simple Analogy: One Bouncer, Many Guests

Imagine you’re throwing a party. Instead of placing a bouncer next to every guest (inefficient), you place **one at the door** to manage everyone who enters.

Event Delegation is the same—**you attach one event listener to a parent element** and detect which child triggered the event.

### 🧪 Example 1: Simple Click Handling in a List

```html
<ul id="menu">
  <li>Home</li>
  <li>About</li>
  <li>Contact</li>
</ul>
```

```javascript
const menu = document.getElementById("menu");

menu.addEventListener("click", (e) => {
  if (e.target.tagName === "LI") {
    console.log("Clicked:", e.target.textContent);
  }
});
```

**💡 Explanation:**

- The click listener is added to the `<ul>`, not each `<li>`.
- `e.target` identifies the actual element clicked.
- Even if new `<li>` elements are added later, this still works!

### 🧪 Example 2: Medium Use Case – Dynamic Notifications

```html
<div class="notifications">
  <div class="toast">🔔 New email <button class="close">✖</button></div>
  <div class="toast">🔔 Message received <button class="close">✖</button></div>
</div>
```

```javascript
document.querySelector(".notifications").addEventListener("click", (e) => {
  if (e.target.classList.contains("close")) {
    e.target.closest(".toast").remove();
  }
});
```

**💡 Explanation:**

- We listen at the `.notifications` wrapper.
- When a `.close` button is clicked, we find its `.toast` container and remove it.
- The **same listener** can close **any number of toasts**, even ones added dynamically.

### 🧪 Example 3: Input Focus Events with Delegation

```html
<form id="signup-form">
  <input type="text" name="name" placeholder="Name" />
  <input type="email" name="email" placeholder="Email" />
</form>
```

```javascript
document.getElementById("signup-form").addEventListener("focusin", (e) => {
  if (e.target.tagName === "INPUT") {
    e.target.style.borderColor = "blue";
  }
});
```

**💡 Explanation:**

- `focusin` bubbles (unlike `focus`), so we can delegate it!
- We react to all `<input>` elements with one listener.
- Great for styling or validating fields without separate event binding.

### ❌ Common Mistakes to Watch Out For

| Mistake                              | Why It’s a Problem                           | What to Do Instead                        |
| ------------------------------------ | -------------------------------------------- | ----------------------------------------- |
| Using `e.currentTarget`              | Always points to the parent listener element | Use `e.target` to access the actual click |
| Not filtering event targets          | Causes handlers to fire on unrelated clicks  | Use `.matches()` or class/tag checks      |
| Attaching listeners to dynamic items | Won’t work if items are added after load     | Delegate from a stable parent             |

### 🌍 Real-World Use Cases

- Dynamic **to-do lists** with delete buttons
- Reusable **modals** or **tabs**
- Delegated **form validation**
- Managing dropdown or mobile nav **menus**

### 🧾 TL;DR

| Feature              | What It Does                                                       | Why It Helps                                 |
| -------------------- | ------------------------------------------------------------------ | -------------------------------------------- |
| **Event Delegation** | **Listen** once on a **parent**, **react** to all **child** events | Less code, better performance, dynamic-ready |

<br>

## 18. 🎛️ Understanding Event Bubbling and Capturing in JavaScript

- **✅ Master DOM Event Flow**
- **✅ Fix Unexpected Behaviors**
- **✅ Power Up Event Delegation and UI Design**

### 🧠 Simple Analogy: The Escalator and the Crowd

Imagine you're in a shopping mall:

- **Capturing phase:** Security spots trouble from the top floor and starts following a person down the escalator.

- **Target phase:** The person reaches a store—they're now the center of attention.

- **Bubbling phase:** As they move down to the food court, everyone they pass reacts.

In JavaScript, **events follow a similar path**: from the **top of the DOM, down to the target element, then back up again**.

### 🚦 How Event Flow Works in the DOM

1. **Capture Phase (Trickles Down)** The event travels from the root (`<html>`) toward the target element.
2. **Target Phase** The event arrives at the element that was actually interacted with (clicked, focused, etc).
3. **Bubble Phase (Bubbles Up)** The event then moves back up the DOM tree to the document.

By default, **event listeners use the bubbling phase**—but you can tap into capturing by setting `{ capture: true }`.

### 🧪 Example 1: Default Bubbling Behavior

```html
<div id="parent">
  <button id="child">Click Me</button>
</div>
```

```javascript
document.getElementById("parent").addEventListener("click", () => {
  console.log("Parent clicked!");
});

document.getElementById("child").addEventListener("click", () => {
  console.log("Child clicked!");
});
```

**💡 Explanation:**

- Click the button: you'll see 👉 `Child clicked!` 👉 `Parent clicked!`
- The event starts at #child, then **bubbles up** and triggers the parent listener.
- This is the default and is what **event delegation depends on**.

### 🧪 Example 2: Using Capture Phase

```javascript
document.getElementById("parent").addEventListener(
  "click",
  () => {
    console.log("Parent capturing!");
  },
  { capture: true }
);
```

**💡 Explanation:**

- Adding `{ capture: true }` causes the event to be handled **while going down** the DOM tree—before it reaches the target.
- Click the button now and you’ll see: 👉 `Parent capturing!` 👉 `Child clicked!`
- Useful when you want to **intercept or prioritize parent-level logic** before it reaches the child.

### 🧪 Example 3: Stop Event Bubbling

```javascript
document.getElementById("child").addEventListener("click", (e) => {
  e.stopPropagation();
  console.log("Child clicked, bubbling stopped!");
});
```

**💡 Explanation:**

- `e.stopPropagation()` **prevents the event from bubbling** to parent listeners.
- The parent won’t receive the event at all—useful when you need to isolate interactions (like modals or dropdowns).

### ❌ Common Pitfalls

| ⚠️ Mistake                     | Why It’s a Problem                               | Fix it with…                                  |
| ------------------------------ | ------------------------------------------------ | --------------------------------------------- |
| Relying only on bubbling       | Some events don’t bubble (e.g., `blur`, `focus`) | Use **capturing phase** or alternative events |
| Forgetting `stopPropagation()` | Parent logic interferes with child behavior      | Stop the bubble when needed                   |
| Overusing capture              | Can complicate debugging                         | Reserve for critical intercepts               |

### 🌍 Real-World Use Cases

- Event Delegation relies on **bubbling**
- Preventing clicks from closing a **dropdown menu**
- Running parent-level logic **before children receive events**
- Stopping event chains inside **modals or nested UIs**

### 🧾 TL;DR

| Phase     | Direction    | Triggered Listeners                 |
| --------- | ------------ | ----------------------------------- |
| Capturing | Top → Target | Listeners with `{ capture: true }`  |
| Target    | —            | The element that received the event |
| Bubbling  | Target → Top | Default phase for most listeners    |
