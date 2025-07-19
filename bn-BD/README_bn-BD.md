<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png">
  <h1>শিখুন-ভুলুন-আবার শিখুন জাভাস্ক্রিপ্ট 🔄</h1>
</div>

আপনার **JavaScript দক্ষতা পরীক্ষা করুন**, গুরুত্বপূর্ণ ধারণাগুলি পুনঃজীবিত করুন, অথবা **ইন্টারভিউয়ের জন্য প্রস্তুতি নিন!** 💪 এই **সম্পূর্ণ ডকুমেন্ট গাইড** আপনাকে **JavaScript-এর গভীর বিষয়গুলি পরিষ্কারভাবে শেখাতে** সাহায্য করবে, যেখানে রয়েছে **বিশদ ব্যাখ্যা, একাধিক উদাহরণ, সাধারণ ভুলত্রুটি এবং বাস্তব জীবনের প্রয়োগ**।

আমি এটি নিজের **শিখন ও অবসরে আনন্দের জন্য তৈরি করেছি**, তাই **যদি কোনো ভুল থেকে থাকে, দয়া করে ক্ষমা করবেন**। 😊 আপনি যদি এটি **উপকারী মনে করেন**, তাহলে **⭐️ দিয়ে সাহায্য করুন বা রেফারেন্স দিন**, এটি আমাকে আরও ভালো করতে অনুপ্রেরণা দেবে!

আপনার **প্রোগ্রামিং যাত্রায় শুভকামনা—** নতুন কিছু শিখুন, অনুশীলন করুন, এবং **সেরা JavaScript ডেভেলপার হয়ে উঠুন! 🙏✨ হ্যাপি কোডিং! 🧑‍💻**

<p align="center">
💬 যদি আমার সাথে যোগাযোগ করতে চান, ↩️ <br/>
<a href="https://www.facebook.com/saiefalemon">Facebook</a> | <a href="https://www.linkedin.com/in/saiefalemon">LinkedIn</a> | <a href="https://www.iamsaief.com/">Blog</a>

---

**🗂️ সূচিপত্র:**

- [১. 🧐 JavaScript-এর Truthy বনাম Falsy: কন্ডিশনাল লজিকে মাস্টার হয় এবং গোপন বাগ এড়াও](#১--javascript-এর-truthy-বনাম-falsy-কন্ডিশনাল-লজিকে-মাস্টার-হয়-এবং-গোপন-বাগ-এড়াও)
- [২. 👨‍👩‍👧‍👦 JavaScript-এর Prototypal Inheritance: কিভাবে অবজেক্ট Prototype Chain ব্যবহার করে কাজকর্ম শেয়ার করে](#২--javascript-এর-prototypal-inheritance-কিভাবে-অবজেক্ট-prototype-chain-ব্যবহার-করে-কাজকর্ম-শেয়ার-করে)
- [৩. 📜 JavaScript এ Promises এর ব্যাখ্যাঃ .then(), .catch(), ও async/await দিয়ে অ্যাসিনক্রোনাস লজিক হ্যান্ডল করা](#৩--javascript-এ-promises-এর-ব্যাখ্যাঃ-then-catch-ও-asyncawait-দিয়ে-অ্যাসিনক্রোনাস-লজিক-হ্যান্ডল-করা)
- [4. 🎭 উদাহরণ সহ Closures এর ব্যাখ্যা: JavaScript এ Function Scope আনলক করা এবং Private State সংরক্ষণ করা](#4--উদাহরণ-সহ-closures-এর-ব্যাখ্যা-javascript-এ-function-scope-আনলক-করা-এবং-private-state-সংরক্ষণ-করা)
- [৫. 🔄 জাভাস্ক্রিপ্টের Event Loop ও অ্যাসিনক্রোনাস ব্যাবহার](#৫--জাভাস্ক্রিপ্টের-event-loop-ও-অ্যাসিনক্রোনাস-ব্যাবহার)
- [৬. 🔥 `this` কেন বিভ্রান্তিকর (এবং কীভাবে দক্ষভাবে ব্যবহার করবেন)](#৬--this-কেন-বিভ্রান্তিকর-এবং-কীভাবে-দক্ষভাবে-ব্যবহার-করবেন)
- [৭. 💡 `call`, `apply`, এবং `bind` ব্যবহার করে ফাংশনের শক্তিশালী নিয়ন্ত্রণ](#৭--call-apply-এবং-bind-ব্যবহার-করে-ফাংশনের-শক্তিশালী-নিয়ন্ত্রণ)
- [৮. 🚀 `map`, `filter`, এবং `reduce` সহজ ভাষায় ব্যাখ্যা](#৮--map-filter-এবং-reduce-সহজ-ভাষায়-ব্যাখ্যা)
- [৯. ⏳ `setTimeout` এবং `setInterval` কীভাবে কাজ করে (এবং কেন গুরুত্বপূর্ণ)](#৯--settimeout-এবং-setinterval-কীভাবে-কাজ-করে-এবং-কেন-গুরুত্বপূর্ণ)
- [১০. 🔄 `async` এবং `await`: অ্যাসিনক্রোনাস কোড সহজ করে তোলার সবচেয়ে ভালো উপায়](#১০--async-এবং-await-অ্যাসিনক্রোনাস-কোড-সহজ-করে-তোলার-সবচেয়ে-ভালো-উপায়)
- [১১. 📦 `JSON` এবং `localStorage` ব্যবহার করে ডাটা সংরক্ষণ করা](#১১--json-এবং-localstorage-ব্যবহার-করে-ডাটা-সংরক্ষণ-করা)
- [১২. 🏗️ ES6 Classes: Object-Oriented JavaScript সহজ করার সবচেয়ে ভালো উপায়](#১২-️-es6-classes-object-oriented-javascript-সহজ-করার-সবচেয়ে-ভালো-উপায়)
- [১৩. 🔟 🚨 কেন JavaScript-এ `"use strict"` ব্যবহার করা উচিত (এবং কীভাবে এটি কোডকে নিরাপদ করে)](#১৩---কেন-javascript-এ-use-strict-ব্যবহার-করা-উচিত-এবং-কীভাবে-এটি-কোডকে-নিরাপদ-করে)
- [১৪. 🛡️ JavaScript-এর `try...catch`: ত্রুটি হ্যান্ডলিংয়ের গোপন অস্ত্র](#১৪-️-javascript-এর-trycatch-ত্রুটি-হ্যান্ডলিংয়ের-গোপন-অস্ত্র)
- [১৫. 🔑 `Object.keys()`, `Object.values()`, এবং `Object.entries()` ব্যবহার করে ডাটা বের করা](#১৫--objectkeys-objectvalues-এবং-objectentries-ব্যবহার-করে-ডাটা-বের-করা)
- [১৬. ⏱️ জাভাস্ক্রিপ্টে _ডিবাউন্স_ এবং _থ্রটল_: কিভাবে ফাংশনের সময় ঠিকমতো নিয়ন্ত্রণ করবেন](#১৬-️-জাভাস্ক্রিপ্টে-ডিবাউন্স-এবং-থ্রটল-কিভাবে-ফাংশনের-সময়-ঠিকমতো-নিয়ন্ত্রণ-করবেন)
- [১৭. 🎯 জাভাস্ক্রিপ্টে ইভেন্ট _ডেলিগেশন_ : কম দিয়ে বেশি ইভেন্ট হ্যান্ডল করুন](#১৭--জাভাস্ক্রিপ্টে-ইভেন্ট-ডেলিগেশন--কম-দিয়ে-বেশি-ইভেন্ট-হ্যান্ডল-করুন)
- [১৮. 🎛️ ইভেন্ট _বাবলিং_ এবং _ক্যাপচারিং_ জাভাস্ক্রিপ্টে: কীভাবে ইভেন্ট প্রবাহ কাজ করে](#১৮-️-ইভেন্ট-বাবলিং-এবং-ক্যাপচারিং-জাভাস্ক্রিপ্টে-কীভাবে-ইভেন্ট-প্রবাহ-কাজ-করে)
- [১৯. 🧠 জাভাস্ক্রিপ্টে মেমোরি ম্যানেজমেন্ট: লিক বন্ধ করুন, অ্যাপ অপটিমাইজ করুন](#১৯--জাভাস্ক্রিপ্টে-মেমোরি-ম্যানেজমেন্ট-লিক-বন্ধ-করুন-অ্যাপ-অপটিমাইজ-করুন)
- [২০. ⛓️ জাভাস্ক্রিপ্টে ব্লকিং বনাম নন-ব্লকিং কোড কীভাবে কাজ করে](#২০-️-জাভাস্ক্রিপ্টে-ব্লকিং-বনাম-নন-ব্লকিং-কোড-কীভাবে-কাজ-করে)
- [২১. 🧪 টেস্টযোগ্য জাভাস্ক্রিপ্ট লেখা: পিওর ফাংশন এবং সাইড ইফেক্ট](#২১--টেস্টযোগ্য-জাভাস্ক্রিপ্ট-লেখা-পিওর-ফাংশন-এবং-সাইড-ইফেক্ট)

---

## ১. 🧐 JavaScript-এর Truthy বনাম Falsy: কন্ডিশনাল লজিকে মাস্টার হয় এবং গোপন বাগ এড়াও

**🛠️ পরিচিতি**

JavaScript-এ, প্রতিটি মান হয় **truthy** না হয় **falsy** যখন তা Boolean কনটেক্সটে যাচাই করা হয়—যেমন `if` স্টেটমেন্ট বা লজিকাল কন্ডিশনে।

এই classification নির্ধারণ করে তোমার অ্যাপ কীভাবে ডিসিশন নেয়, ডেটা ফিল্টার করে, আর expression যাচাই করে।

Truthy আর falsy কী তা ভালোভাবে বোঝা গেলে কোড হবে আরও পরিষ্কার আর বাগবিহীন।

### 💡 সহজ উদাহরণ: খালি কাগজ বনাম ভর্তি ফোল্ডার

ধরো primitive মান মানে একটা কাগজ — সেটা হয় খালি (falsy) বা লেখা ভর্তি (truthy)।

অন্যদিকে, object মানে একটা ফোল্ডার। ফোল্ডারের ভেতরে যদি খালি কাগজও থাকে (`new Boolean(false)`), ফোল্ডারটা যেহেতু আছে, সেটা truthy ধরা হয়।

### 📝 উদাহরণ (সহজ): স্ট্রিং চেক করা

```javascript
const name = "Saief";

if (name) {
  console.log("Valid name");
} else {
  console.log("Name is missing");
}
```

**💬 ব্যাখ্যা:**

- স্ট্রিং `"Saief"` truthy কারণ এটা খালি না। কিন্তু যদি `name = ""` হয়, তাহলে সেটা falsy হবে এবং `else` ব্লক চলবে।

### 📝 উদাহরণ (জটিল): অবজেক্ট র‍্যাপার বোঝা

```javascript
const flag = new Boolean(false);

if (flag) {
  console.log("This still runs!");
}
```

**💬 ব্যাখ্যা:**

- `false` ভিতরে থাকলেও, `flag` একটি object, আর সব object truthy।
- এটা অনেক সময় বিভ্রান্ত করে, বিশেষ করে টাইপ coercion আর Boolean লজিকে অবজেক্ট র‍্যাপার মেশালে।

### 🧪 প্রিমিটিভ টাইপ: Truthy বনাম Falsy চিট শিট

| 🧱 টাইপ     | 🧪 উদাহরণ                   | ✅ Boolean কনটেক্সটে আচরণ    |
| ----------- | --------------------------- | ---------------------------- |
| `undefined` | `undefined`                 | Falsy                        |
| `null`      | `null`                      | Falsy                        |
| `boolean`   | `true`, `false`             | `true` truthy, `false` falsy |
| `number`    | `42`, `0`, `NaN`            | `0` আর `NaN` falsy           |
| `string`    | `"Hello"`, `""`             | `""` falsy                   |
| `symbol`    | `Symbol("id")`              | সবসময় truthy                 |
| `BigInt`    | `BigInt(1234)`, `BigInt(0)` | `BigInt(0)` falsy            |

### 🧪 রেফারেন্স টাইপ সবসময় Truthy

| 💡 টাইপ            | 📝 উদাহরণ             | ⚡ আচরণ      |
| ------------------ | --------------------- | ------------ |
| Array              | `[]`, `[1,2,3]`       | সবসময় truthy |
| Object             | `{}`, `{ name: "A" }` | সবসময় truthy |
| Function           | `function() {}`       | সবসময় truthy |
| Constructor Object | `new Boolean(false)`  | সবসময় truthy |

> ভেতরে যা-ই থাকুক না কেন—রেফারেন্স যদি মেমোরিতে থাকে, সেটা truthy।

### ❌ সাধারণ ভুল

| ❌ ভুল                        | 😵 কেন বিভ্রান্তিকর                             | ✅ সমাধান                                   |
| ----------------------------- | ----------------------------------------------- | ------------------------------------------- |
| `new Boolean(false)` truthy   | দেখতে falsy মনে হয়, কিন্তু object হিসেবে truthy | প্রিমিটিভ র‍্যাপ না করাই ভালো               |
| `""`, `0`, `NaN` কে valid ধরা | কন্ডিশনে সাইলেন্টলি ফেল করে                     | স্পষ্টভাবে চেক করো                          |
| `==` ব্যবহার                  | টাইপ coercion ঘটায়                              | `===` ব্যবহার করো strict comparison এর জন্য |

### 🌍 বাস্তব উদাহরণ

- React-এ conditional rendering

```jsx
{
  user && <WelcomeScreen />;
}
```

- Short-circuit evaluation

```javascript
const theme = customTheme || "light";
```

- ফর্ম ভ্যালিডেশন

```javascript
if (!email) showError("Email is required");
```

### 🧾 সংক্ষিপ্ত রেফারেন্স

| 🧩 টাইপ                                        | ✅ Truthy? | ⚠️ Falsy? | 🔎 মন্তব্য                    |
| ---------------------------------------------- | ---------- | --------- | ----------------------------- |
| `""`, `0`, `NaN`, `null`, `undefined`, `false` | ❌ না      | ✅ হ্যাঁ  | কন্ডিশনে false হিসেবে বিবেচিত |
| সব object (`{}`, `[]`, function, constructor)  | ✅ হ্যাঁ   | ❌ না     | সবসময় truthy                  |
| `new Boolean(false)` এর মত র‍্যাপ করা মান      | ✅ হ্যাঁ   | ❌ না     | object হওয়ার কারণে truthy     |

<br>

## ২. 👨‍👩‍👧‍👦 JavaScript-এর Prototypal Inheritance: কিভাবে অবজেক্ট Prototype Chain ব্যবহার করে কাজকর্ম শেয়ার করে

**🛠️ পরিচিতি**

JavaScript-এ **prototypal inheritance** ব্যবহার হয় object গুলোর মধ্যে property আর method শেয়ার করার জন্য। Java বা C++ এর মতো ক্লাসভিত্তিক ভাষায় এক ক্লাস আরেকটা ক্লাসকে extend করে, কিন্তু JavaScript-এ object গুলো সরাসরি অন্য object থেকে inherit করতে পারে।

এই পদ্ধতিতে ডেভেলপাররা **কম মেমোরি খরচে**, **reusable** এবং **extendable** কোড লিখতে পারে, কারণ common method গুলো instance-এ না রেখে prototype-এ রাখা যায়।

Prototype কীভাবে কাজ করে সেটা জানা দরকার ভালো কোড, behavior extend করা আর inheritance-জনিত bug ধরার জন্য।

### 💡 সহজ উদাহরণ: পারিবারিক রেসিপি বই

ধরো প্রতিটা JavaScript object এর একটা নিজস্ব রেসিপি বই আছে। যদি সেখানে কোনো রেসিপি (method) না থাকে, তাহলে সে তার বাবা-মায়ের কাছে জিজ্ঞাসা করে। না পেলে তারা আবার তাদের মা-বাবাকে জিজ্ঞেস করে। শেষ পর্যন্ত যদি কেউ না পায়, তাহলে সেটা মেনে নেয়।

এই রেসিপি খোঁজার চেইনটাই JavaScript-এর **prototype chain**—object গুলো একে অপরের কাছ থেকে উত্তর খোঁজে।

### 📝 উদাহরণ ও 💬 ব্যাখ্যা

#### 🐶 উদাহরণ ১: Dog ক্লাস এবং bark মেথড

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
pet.bark(); // Woof I am Mara
```

**💬 ব্যাখ্যা:**

- `Dog` হলো constructor ক্লাস।
- `bark()` method ক্লাসের ভিতরে না, বরং `Dog.prototype`-এ রাখা হয়েছে।
- ফলে সব instance একই method শেয়ার করে, মেমোরি কম খরচ হয়।
- যখন `pet.bark()` কল করা হয়, JavaScript প্রথমে `pet`-এ খোঁজে, না পেলে `Dog.prototype`-এ গিয়ে method খুঁজে পায়।

#### 📢 উদাহরণ ২: `String.prototype`-এ shout method যোগ করা

```js
String.prototype.shout = function () {
  return this.toUpperCase() + "!!!";
};

console.log("hello".shout()); // HELLO!!!
```

**💬 ব্যাখ্যা:**

- `shout()` method টা `String.prototype`-এ যোগ করা হয়েছে, তাই সব string এটা পাবে।
- এমনকি string literal `"hello"` ও `.shout()` কল করতে পারে কারণ JavaScript একে অস্থায়ীভাবে `String` object বানিয়ে ফেলে।

> Built-in টাইপের prototype extend করা শক্তিশালী হলেও, সাবধানে করতে হয় না হলে global behavior নষ্ট হতে পারে।

#### 📦 উদাহরণ ৩: `Array.prototype`-এ firstElement যোগ করা

```js
Array.prototype.firstElement = function () {
  return this.length > 0 ? this[0] : undefined;
};

console.log([1, 2, 3].firstElement()); // 1
```

**💬 ব্যাখ্যা:**

- এই `firstElement()` method সব array-তেই থাকবে।
- এটা শেয়ারড, কপি করা নয়, তাই পারফরম্যান্স ভালো থাকে।
- যেকোনো array থেকে প্রথম item বের করার জন্য এটা এখন একটা শর্টকাট।

#### 🧠 উদাহরণ ৪: `Object.prototype` এ keysCount (সতর্ক থাকো)

```js
Object.prototype.keysCount = function () {
  return Object.keys(this).length;
};

console.log({ name: "Alice", age: 25 }.keysCount()); // 2
```

**💬 ব্যাখ্যা:**

- সব object এই method পেয়ে যাবে কারণ এটা `Object.prototype`-এ রাখা হয়েছে।

> এটা শক্তিশালী হলেও অনেক সময় সমস্যা করতে পারে—loop এ extra method দেখা যাবে বা অন্য লাইব্রেরির সঙ্গে conflict হতে পারে।

> - প্রোডাকশন অ্যাপে `Object.prototype` এ পরিবর্তন না করাই ভালো, যদি না পুরো environment এর ওপর তোমার নিয়ন্ত্রণ থাকে।

### 🌍 বাস্তব ব্যবহার

- **Instance গুলোর মাঝে common utility method শেয়ার করা** (যেমন form validator)
- **Framework বা লাইব্রেরি extend করা** (যেমন `.shout()`)
- **কম মেমোরিতে object modeling** (যেমন game logic বা DOM wrapper)
- **পুরনো browser এ polyfill লেখা** (যেমন `Array.prototype.includes`)

### ❌ সাধারণ ভুল

| ❌ ভুল                           | ⚠️ সমস্যা কেন হয়                                           | ✅ কী করা উচিত                                      |
| -------------------------------- | ---------------------------------------------------------- | --------------------------------------------------- |
| `Object.prototype` পরিবর্তন করা  | loop বা থার্ড পার্টি টুল ভেঙে যেতে পারে                    | utility wrapper বা scoped prototype extend করো      |
| constructor এর ভেতর method রাখা  | প্রতিটা instance আলাদা করে method কপি পায়                  | `.prototype`-এ রাখো                                 |
| `class` মানেই prototype নেই ভাবা | class syntax-ও আন্ডার দ্যা হুড prototype chain ব্যবহার করে | এটাকে prototype chain এর syntactic sugar হিসেবে ধরো |
| inheritance resolution না বোঝা   | bug ধরতে সমস্যা হয়                                         | `console.log(obj.__proto__)` দিয়ে চেইন দেখো         |

### 🧾 সংক্ষিপ্ত রেফারেন্স

| 🧩 ফিচার                      | 💡 মানে কী                                    | 🔧 কেন দরকার                                  |
| ----------------------------- | --------------------------------------------- | --------------------------------------------- |
| **Prototypal Inheritance**    | object তার prototype chain থেকে behavior নেয়  | মেমোরি বাঁচে, logic reuse করা যায়             |
| `.prototype` ব্যবহার          | instance গুলোর জন্য method শেয়ার করে          | constructor-এ method কপি হওয়া বন্ধ হয়         |
| **Built-in prototype extend** | array, string ইত্যাদিতে কাস্টম method যোগ করা | সাবধানে করতে হবে, না হলে global scope নষ্ট হয় |

<br>

আপনার দেওয়া মার্কডাউন কন্টেন্টটির সহজ সরল বাংলায় অনুবাদ নিচে দেওয়া হলো, যেখানে টপিক রিলেটেড টার্ম/কীওয়ার্ড গুলোর বাংলা অনুবাদ করার প্রয়োজন নেই এবং কোনো অংশ বাদ দেওয়া হয়নি।

## ৩. 📜 JavaScript এ Promises এর ব্যাখ্যাঃ .then(), .catch(), ও async/await দিয়ে অ্যাসিনক্রোনাস লজিক হ্যান্ডল করা

**🛠️ ভূমিকা**

**Promise** হলো একটি অবজেক্ট যা asynchronous operation-এর ফলাফলকে উপস্থাপন করে — হয় সফলতা অথবা ব্যর্থতা। কোড চালানো এবং তাৎক্ষণিকভাবে ফলাফল ফেরানোর পরিবর্তে, Promise আপনাকে এমন ফলাফলগুলি পরিচালনা করতে দেয় যা **পরে** আসে (যেমন একটি সার্ভার থেকে ডেটা)।

এগুলো পুরোনো callback-ভিত্তিক প্যাটার্নগুলোর (callback-based patterns) তুলনায় async logic ডিল করার জন্য একটি পরিচ্ছন্ন, আরও সুসংগঠিত উপায় প্রদান করে। আধুনিক JavaScript ডেভেলপমেন্টের জন্য, বিশেষ করে React বা API-ভিত্তিক অ্যাপস-এ, Promises বোঝাটা non-negotiable।

### 💡 সহজ উদাহরনঃ (রেস্টুরেন্ট রিজার্ভেশন)

একটি ডিনার রিজার্ভেশন করার কথা ভাবুন:

- **আপনি (consumer)** রেস্টুরেন্টে ফোন করেন।
- **তারা (producer)** একটি টেবিল প্রস্তুত করে।
- যদি সবকিছু ঠিকঠাক চলে, তারা **বুকিং নিশ্চিত করে (resolve)**।
- যদি অতিরিক্ত বুকিং হয়ে যায় বা তারা গোলমাল করে, তারা **এটি বাতিল করে (reject)**।

আপনি কাউন্টারে বসে অপেক্ষা করেন না। পরিবর্তে, আপনি **নিশ্চিতকরণের উপর বিশ্বাস রাখেন** এবং যখন প্রস্তুত হন তখন উপস্থিত হন। এভাবেই একটি Promise কাজ করে — **এটি নিশ্চিত করে যে অবশেষে কিছু ঘটবেই**, এবং আপনার কোড সেই অনুযায়ী প্রতিক্রিয়া জানাতে পারে।

### 🔹 Promise এর অবস্থাগুলো

একটি Promise এর **3টি অবস্থা** থাকতে পারে:

| **State (অবস্থা)** | **Description (বর্ণনা)**                    |
| ------------------ | ------------------------------------------- |
| **Pending**        | অপারেশনটি এখনও চলছে।                        |
| **Fulfilled**      | অপারেশন সফলভাবে সম্পন্ন হয়েছে (`resolve`)। |
| **Rejected**       | অপারেশন ব্যর্থ হয়েছে (`reject`)।           |

### 📝 উদাহরণ এবং 💬 ব্যাখ্যা

#### ✅ উদাহরণ ১: একটি Promise তৈরি করা

```js
const myPromise = new Promise((resolve, reject) => {
  const success = true;

  setTimeout(() => {
    if (success) {
      resolve("✅ Data received!");
    } else {
      reject("❌ Something went wrong.");
    }
  }, 1500);
});
```

**💬 ব্যাখ্যা:**

- `new Promise()` দুটি প্যারামিটার সহ একটি ফাংশন নেয়: `resolve` এবং `reject`।
- এই ফাংশনটি (যা executor নামে পরিচিত) অবিলম্বে চলে।
- 1500ms পরে, এটি `success` ফ্ল্যাগের উপর ভিত্তি করে `resolve()` অথবা `reject()` কল করে।
- Promise একটি `pending` অবস্থা থেকে শুরু হয়, তারপর `fulfilled` বা `rejected` অবস্থায় চলে যায়।

#### ✅ উদাহরণ ২: `.then()` এবং `.catch()` ব্যবহার করা

```js
myPromise.then((message) => console.log("Success:", message)).catch((error) => console.log("Failure:", error));
```

**💬 ব্যাখ্যা:**

- `.then()` চলে যদি Promise সফলভাবে resolve হয়।
- `.catch()` চলে যদি এটি reject হয়।
- এই chaining সফলতা/ব্যর্থতা পাশাপাশি হ্যান্ডেল করা সহজ করে তোলে।
- আপনি `.finally()` ব্যবহার করতে পারেন, ফলাফল যাই হোক না কেন এই ব্লকের কোডটি চলবে।

#### ✅ উদাহরণ ৩: Async/Await – পরিষ্কার সিনট্যাক্স

```js
async function fetchData() {
  try {
    const response = await fetch("https://jsonplaceholder.typicode.com/posts");
    if (!response.ok) throw new Error(`HTTP status: ${response.status}`);
    const data = await response.json();
    console.log("Fetched:", data);
  } catch (error) {
    console.error("Error:", error.message);
  }
}
fetchData();
```

**💬 ব্যাখ্যা:**

- `async function` আপনাকে `await` ব্যবহার করতে দেয়, promise resolve না হওয়া পর্যন্ত এক্সিকিউশন থামিয়ে রাখার জন্য।
- যদি এটি ব্যর্থ হয়, নিয়ন্ত্রণ `catch` ব্লকে চলে যায়।
- এই প্যাটার্নটি **synchronous** মনে হয়, কিন্তু এটি আন্ডার দ্য হুড **asynchronous behavior** হ্যান্ডেল করে।
- এটি সাধারণত **React hooks, data fetching, এবং form handling**-এ ব্যবহৃত হয়।

### 🌍 বাস্তব উদাহরণ

- REST APIs বা GraphQL থেকে ডেটা আনা।
- ব্রাউজারে `FileReader` ব্যবহার করে ফাইল পড়া।
- ব্যবহারকারীর authentication বা form submission হ্যান্ডেল করা।
- অ্যানিমেশন এবং ট্রানজিশন যা asynchronously সম্পন্ন হয়।
- React এর `useEffect()` প্রায়শই Promise বা `async/await` ব্যবহার করে async logic কে wraps করে।

### ❌ সাধারণ ভুল

| ❌ ভুল                                      | 😵 সমস্যা কেন হয়               | ✅ সমাধান                                                       |
| ------------------------------------------- | ------------------------------ | --------------------------------------------------------------- |
| একটি promise return করতে ভুলে যাওয়া        | চেইনে অনির্দিষ্ট আচরণ দেখা দেয় | সর্বদা promise বা ফলাফল return দিন                              |
| `async` এবং `.then()` মেশানো                | অগোছালো নেস্টেড কোড তৈরি করে   | `.then()` অথবা `await` এর মধ্যে যেকোনো একটি বেছে নিন, উভয়ই নয় |
| Unhandled rejections (আনহ্যান্ডেলড রিজেকশন) | নীরবে এরর ফ্লো ভেঙে দেয়        | সর্বদা `.catch()` বা `try...catch` ব্যবহার করুন                 |
| `async` এর বাইরে `await` ব্যবহার করা        | সিনট্যাক্স এরর সৃষ্টি করে      | প্যারেন্ট ফাংশনটিকে `async` করুন                                |

### 🧾 সংক্ষেপে

| 🎯 ধারণা               | 💡 বর্ণনা                                                    | ⚡ টিপস                                                 |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------- |
| `Promise`              | ভবিষ্যতের সফলতা বা ব্যর্থতাকে উপস্থাপন করে                   | async operations পরিষ্কারভাবে হ্যান্ডেল করতে ব্যবহৃত হয় |
| `.then()` / `.catch()` | ফলাফল এবং ত্রুটির জন্য হ্যান্ডলারগুলিকে শৃঙ্খলিত (chain) করে | চেইনিং এবং লজিক বিভাজনের জন্য দারুণ                     |
| `async/await`          | Promise এর সাথে কাজ করার জন্য সিনট্যাক্স সুগার               | async flows-এ কোড রিডেবিলিটি উন্নত করে                  |
| States (অবস্থা)        | `pending`, `fulfilled`, `rejected`                           | আপনার কোড কখন এবং কীভাবে এক্সিকিউট হয় তা জানুন          |

<br>

## 4. 🎭 উদাহরণ সহ Closures এর ব্যাখ্যা: JavaScript এ Function Scope আনলক করা এবং Private State সংরক্ষণ করা

**🛠️ ভূমিকা**

একটি closure গঠিত হয় যখন একটি ফাংশন তার বাইরের scope এর ভেরিয়েবলগুলিকে "মনে রাখে", এমনকি বাইরের ফাংশনটি এক্সিকিউশন শেষ করার পরেও। এটি JavaScript এর সবচেয়ে শক্তিশালী বৈশিষ্ট্যগুলির মধ্যে একটি, যা **data encapsulation**, **function factories**, এবং **persistent state** এর মতো প্যাটার্নগুলিকে সক্ষম করে।

Closures সর্বত্র রয়েছে — **event handlers** থেকে শুরু করে **loops**, **timers**, এবং **React hooks** পর্যন্ত। আপনি সাধারণ টুল তৈরি করুন বা জটিল অ্যাপস স্কেল করুন না কেন, closures সম্পর্কে একটি পরিষ্কার ধারণা আপনাকে অনুমানযোগ্য এবং testable কোড লিখতে সাহায্য করে।

### 💡 সহজ উদাহরণ: পিকনিক বাস্কেট

কল্পনা করুন আপনি পিকনিকে যাচ্ছেন:

- আপনি আপনার **স্যান্ডউইচ, পানি, এবং অন্যান্য জিনিস** প্যাক করেন।
- বাড়ি থেকে বহু মাইল দূরেও, আপনার **বাস্কেট** আপনি যা প্যাক করেছেন তার **সবকিছু বহন করে**।
- Closures একইভাবে কাজ করে: একটি ফাংশন তার original scope থেকে ভেরিয়েবল সহ ভ্রমণ করে — **এমনকি সেই scope চলে যাওয়ার পরেও**।

### 📝 উদাহরণ এবং 💬 ব্যাখ্যা

#### ✅ উদাহরণ ১: ডেটা গোপনীয়তা

```javascript
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

**💬 ব্যাখ্যা:**

- `count` হলো `createCounter()` এর ভিতরের একটি local variable।
- রিটার্ন করা inner function closures এর মাধ্যমে `count` এ অ্যাক্সেস বজায় রাখে।
- `createCounter()` ইতিমধ্যে চললেও, `count` সচল থাকে।
- ✅ এটি global variables ব্যবহার না করেই একটি private, persistent state তৈরি করে।

#### ✅ উদাহরণ ২ঃ ফাংশন ফ্যাক্টরি

```javascript
function multiplier(x) {
  return function (num) {
    return num * x;
  };
}

const double = multiplier(2);
console.log(double(5)); // 10
```

**💬 ব্যাখ্যা:**

- রিটার্ন করা ফাংশন `x` কে মনে রাখা হয়।
- `multiplier()` এর প্রতিটি কল একটি ফাংশন ফেরত দেয় যার নিজস্ব closed-over `x` আছে।
- এই প্যাটার্নটি **custom utilities, configurable handlers, বা dynamic calculations** তৈরি করার জন্য দরকারী।

#### ✅ উদাহরণ ৩ঃ ইভেন্ট হ্যান্ডলিং

```javascript
(function () {
  let clickCount = 0;

  document.getElementById("myButton").addEventListener("click", function () {
    clickCount++;
    console.log(`Clicked ${clickCount} times`);
  });
})();
```

**💬 ব্যাখ্যা:**

- anonymous outer function একবার চলে এবং `clickCount` সেট করে।
- event handler `clickCount` কে “closes over” করে এবং প্রতিটি ক্লিকে এটি আপডেট করে।
- বাইরের ফাংশনটি অনেক আগে শেষ হয়ে গেলেও, handler এখনও `clickCount` কে মনে রাখে এবং modify করে।

#### ⏱️ উদাহরণ ৪ঃ Closure সহ কাউন্টডাউন টাইমার

```javascript
function startCountdown(seconds) {
  let remaining = seconds;

  const intervalId = setInterval(() => {
    if (remaining === 0) {
      console.log("⏰ Time's up!");
      clearInterval(intervalId);
    } else {
      console.log(`🕒 ${remaining} seconds left`);
      remaining--;
    }
  }, 1000);
}

startCountdown(5);
```

**💬 ব্যাখ্যা:**

- `startCountdown()` ফাংশনটি একটি private `remaining` ভেরিয়েবল ইনিশিয়ালাইজ (initialize) করে।
- `setInterval()` এর ভিতরের inner function একটি **closure** তৈরি করে এবং `remaining` এ অ্যাক্সেস বজায় রাখে।
- `startCountdown()` এক্সিকিউশন শেষ করার পরেও, interval প্রতি সেকেন্ডে `remaining` কে modify এবং read করতে থাকে।
- একবার এটি শূন্যে পৌঁছালে, cycle বন্ধ করার জন্য interval টিকে ক্লিয়ার করা হয়।

> ✅ এটি closures এর একটি নিখুঁত উদাহরণ যা timed logic (যেমন countdowns, game loops, বা auto-refresh behaviors) কে global scope দূষিত না করেই শক্তিশালী করে।

### 🌍 বাস্তব প্রয়োগ

- **React hooks** (যেমন, useState, useEffect)
- ইনপুট বা স্ক্রলের জন্য **Debounce/throttle functions**
- **Custom event handlers** যা context বজায় রাখে
- **Currying এবং function factories**
- **Async operations** যা persistent data সহ কাজ করে

### ❌ সাধারণ ভুল

| ❌ ভুল                                            | ⚠️ সমস্যা                                         | ✅ পরিবর্তে কি করবেন                                                   |
| ------------------------------------------------- | ------------------------------------------------- | ---------------------------------------------------------------------- |
| closures এর ভিতরে loop variable এর উপর নির্ভর করা | সমস্ত callback চূড়ান্ত loop value রেফারেন্স করে  | প্রতিটি iteration এর জন্য মান ক্যাপচার করতে `let` বা IIFE ব্যবহার করুন |
| ভুলবশত internal state উন্মুক্ত করা                | encapsulation ভেঙে দেয় এবং বাগ তৈরি করে          | শুধুমাত্র প্রয়োজনীয় interface functions রিটার্ন করুন                 |
| উপলব্ধি না করা যে closure মেমরি সচল রাখে          | কর্মক্ষমতার সমস্যা বা stale data এর কারণ হতে পারে | যখন আর প্রয়োজন নেই তখন রেফারেন্সগুলি পরিষ্কার করুন                    |

### 🧾 সংক্ষেপে

| 🧩 ধারণা             | 🔎 বর্ণনা                                      | 💡 কেন এটি গুরুত্বপূর্ণ                                         |
| -------------------- | ---------------------------------------------- | --------------------------------------------------------------- |
| **Closure**          | ফাংশন যা outer scope এ অ্যাক্সেস ধরে রাখে      | private state এবং persistent logic সক্ষম করে                    |
| **Data Privacy**     | ভেরিয়েবলগুলিকে global access থেকে লুকানো রাখে | নিরাপদ এবং পরিষ্কার কোড লিখতে সাহায্য করে                       |
| **Function Factory** | মনে রাখা context সহ নতুন ফাংশন ফেরত দেয়       | পুনরায় ব্যবহারযোগ্য utilities এবং configurations এর জন্য দারুণ |

<br>

## ৫. 🔄 জাভাস্ক্রিপ্টের Event Loop ও অ্যাসিনক্রোনাস ব্যাবহার

জাভাস্ক্রিপ্ট **সিঙ্গেল-থ্রেডেড**, অর্থাৎ এটি **এক সময়ে একটিমাত্র কাজ করে**। তবে এটি **Event Loop ব্যবহার করে অ্যাসিনক্রোনাস কাজ দক্ষতার সাথে পরিচালনা করতে পারে**, যা **কোনো কাজ ব্লক না করে অ্যাপ্লিকেশনকে রেসপন্সিভ রাখে**।

### 🧐 কিভাবে Event Loop কাজ করে?

#### 1️⃣ Main Thread

- JavaScript **সিঙ্ক্রোনাস কোড লাইন বাই লাইন এক্সিকিউট** করে।
- সাধারণ **গাণিতিক কাজ, ফাংশন কল, ভেরিয়েবল এসাইনমেন্ট** তাৎক্ষণিকভাবে কার্যকর হয়।

#### 2️⃣ Asynchronous Tasks

- **ফেচ অপারেশন (API কল), ইউজার ইনপুট, ফাইল রিডিং** ইত্যাদি **অ্যাসিনক্রোনাস কাজ** JavaScript ব্লক না করেই চালাতে পারে।
- এসব কাজ **Web APIs-এ ডেলিগেট করা হয়** (যেমন `setTimeout`, `fetch()`, `addEventListener()`)।
- অ্যাসিনক্রোনাস কাজ চলাকালীন, **JavaScript অন্য কোড এক্সিকিউট করা চালিয়ে যেতে পারে**।

#### 3️⃣ Callback Queue

- **যখন একটি অ্যাসিনক্রোনাস কাজ সম্পন্ন হয়**, তার **কলব্যাক ফাংশন কলব্যাক কিউতে রাখা হয়**।
- **কলব্যাক কিউ** এমন ফাংশনগুলোর তালিকা সংরক্ষণ করে, যেগুলো **চালানোর জন্য অপেক্ষমাণ**।

#### 4️⃣ Event Loop

- **Event Loop** ধারাবাহিকভাবে **চেক করে**:
- **Call Stack খালি আছে কিনা।**
- **Callback Queue-তে কোনো কাজ অপেক্ষমাণ আছে কিনা।**
- যদি Call Stack খালি থাকে, **Event Loop কলব্যাক কিউ থেকে পরবর্তী কাজ নিয়ে এক্সিকিউট করে।**

### ⏱️ Web APIs ও setTimeout()

**🔹 setTimeout() এর কাজের ধরন**

1. JavaScript `setTimeout(callback, delay)` **কল করলে**, এটি **Web API-তে ডেলিগেট করা হয়**।
2. **JavaScript মূল থ্রেডে অন্য কাজ চালিয়ে যেতে পারে**, সেটি ব্লক হয় না।
3. **নির্দিষ্ট সময় (delay) শেষে, Web API Callback Queue**-তে কলব্যাক পাঠায়। 4.** Call Stack খালি হলে Event Loop কলব্যাকটিকে এক্সিকিউট করে।**

**📝 Example: setTimeout()**

```js
console.log("Start");

setTimeout(() => {
  console.log("Timeout callback");
}, 1000);

console.log("End");

// আউটপুট:
// "Start"
// "End"
// (১ সেকেন্ড পরে) "Timeout callback"
```

**💡 Explanation:**

- `"Start"` এবং `"End"` **তাৎক্ষণিকভাবে এক্সিকিউট হয়**।
- `setTimeout()` **একটি অ্যাসিনক্রোনাস অপারেশন**, যা Web API-তে পাঠানো হয়।
- **১ সেকেন্ড পরে, `setTimeout()`** এর কলব্যাক **Callback Queue-তে যায়**।
- **Call Stack খালি থাকলে**, Event Loop কলব্যাকটিকে এক্সিকিউট করে।

### 🤝 Microtask Queue ও Promises Execution

Promises অ্যাসিনক্রোনাস কাজ আরও দক্ষতার সাথে পরিচালনা করতে **Microtask Queue** ব্যবহার করে, যা **Callback Queue-র চেয়ে বেশি প্রাধান্য পায়**।

**🔹 কিভাবে Promises কাজ করে?**

- **Promise হলো ভবিষ্যতের জন্য সংরক্ষিত একটি ভ্যালু** (যেমন API থেকে ডাটা আনার জন্য অপেক্ষা)।
- যখন **Promise `resolve()` বা `reject()` হয়**, তার `.then()` বা `.catch()` **Microtask Queue-তে পাঠানো হয়**।
- **Event Loop প্রথমে Microtask Queue চেক করে**, তারপর Callback Queue-তে যায়।

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

// আউটপুট:
// "Fetching data..."
// (১ সেকেন্ড পরে) "Data fetched"
```

**💡 Explanation:**

- `fetchData()` **ফাংশন একটি Promise রিটার্ন করে**, যা **অ্যাসিনক্রোনাস অপারেশন**।
- `.then()` Promise **Resolve হলে চালিত হবে**।
- Meanwhile, **JavaScript Fetching data...** এক্সিকিউট করতে থাকে।
- **১ সেকেন্ড পরে**, Promise **Resolve হলে** **`.then()` Microtask Queue-তে যায়**।
- **Microtask Queue-এর কাজ Call Stack খালি হলে প্রথমেই চালিত হয়**।

**🔁 সারসংক্ষেপ**

- ✅ JavaScript সিঙ্গেল-থ্রেডেড, তবে Event Loop অ্যাসিনক্রোনাস কাজ পরিচালনা করে।
- ✅ setTimeout() Callback Queue ব্যবহার করে, কিন্তু Promises Microtask Queue ব্যবহার করে (যা প্রথমে প্রসেস হয়)।
- ✅ Event Loop নিশ্চিত করে যে JavaScript ব্লক না হয় এবং সিস্টেম সর্বদা রেসপন্সিভ থাকে।

<br>

## ৬. 🔥 `this` কেন বিভ্রান্তিকর (এবং কীভাবে দক্ষভাবে ব্যবহার করবেন)

- ✅ Implicit vs. Explicit Binding
- ✅ Arrow Function এবং Lexical `this`
- ✅ সাধারণ ভুলত্রুটি ও তা ঠিক করার উপায়

### 💡 সহজ উদাহরণ: একজন ব্যক্তিগত সহকারী যার অনেক মালিক আছে

ধরুন একজন সহকারী বিভিন্ন মালিকের জন্য কাজ করেন। কখনও তিনি বুঝতে পারেন কার জন্য কাজ করছেন, আবার কখনও বিভ্রান্ত হন। ঠিক JavaScript-এ `this` ও তাই—এটি যেভাবে এবং কোথায় ফাংশন কল করা হয়, তার উপর নির্ভর করে ভিন্ন ভিন্ন অবজেক্টকে নির্দেশ করে।

### 🔍 this ব্যবহারের প্রক্রিয়া

**📝 উদাহরণ ১: this ব্যবহার করে Object-এর Method কল করা (Implicit Binding)**

```javascript
const person = {
  name: "Alice",
  greet() {
    console.log(`Hello, my name is ${this.name}`);
  },
};

person.greet(); // আউটপুট: Hello, my name is Alice
```

**💡 ব্যাখ্যা:** `this` এখানে `person` অবজেক্টকে নির্দেশ করছে কারণ এটি `greet()` মেথডের ভিতরে ব্যবহৃত হয়েছে।

**📝 উদাহরণ ২: `call`, `apply`, এবং `bind` ব্যবহার করে `this` নির্ধারণ (Explicit Binding)**

```javascript
function sayHello() {
  console.log(`Hello, my name is ${this.name}`);
}

const user = { name: "John" };

sayHello.call(user); // আউটপুট: Hello, my name is John
```

**💡 ব্যাখ্যা:** `.call()` ব্যবহার করে ব্যক্তিগতভাবে `this` নির্ধারণ করা হয়েছে, যাতে এটি `user` অবজেক্টকে নির্দেশ করে।

**📌 সাধারণ ভুল:** Event Listener-এ `this` ভুলভাবে ব্যবহার করলে `undefined` হয়ে যেতে পারে!

**📝 উদাহরণ ৩: Arrow Function ও Lexical this**

```javascript
const student = {
  name: "Emma",
  subjects: ["Math", "Science"],
  showSubjects() {
    this.subjects.forEach((subject) => console.log(`${this.name} studies ${subject}`));
  },
};

student.showSubjects();
// আউটপুট: Emma studies Math
// Emma studies Science
```

**💡 ব্যাখ্যা:** Arrow Function-এর নিজস্ব `this` নেই, তাই এটি চারপাশের স্কোপ থেকে `this` গ্রহণ করে।

### 📌 বাস্তব জীবনের প্রয়োগ

- **Callback ফাংশনের `this` ঠিকমতো ব্যবহারের সমস্যা সমাধান**
- **React-এ ইভেন্ট হ্যান্ডলিংয়ের সময় `this` ঠিক রাখা**
- **Class-এর মেথডে `this` ভুলভাবে ব্যবহারের সমস্যা দূর করা**

<br>

## ৭. 💡 `call`, `apply`, এবং `bind` ব্যবহার করে ফাংশনের শক্তিশালী নিয়ন্ত্রণ

- ✅ এক অবজেক্ট থেকে অন্য অবজেক্টে মেথড ধার নেওয়া
- ✅ তাদের মধ্যে পার্থক্য কীভাবে কাজ করে
- ✅ বাস্তব জীবনের প্রয়োগ

### 💡 সহজ উদাহরণ: অন্যের গাড়ি ধার নেওয়া

- `call` আপনাকে তৎক্ষণাৎ গাড়ি চালানোর অনুমতি দেয়।
- `apply` একই কাজ করে, কিন্তু আর্গুমেন্টের তালিকা একটি অ্যারে আকারে পাঠায়।
- `bind` আপনাকে গাড়ির চাবি দেয়, তবে আপনি পরে চালাতে পারবেন।

### 🔍 এদের কার্যপ্রক্রিয়া

**📝 উদাহরণ ১: `call` ব্যবহার করে অবজেক্টের কন্ট্যাক্সে/প্রসঙ্গ নির্ধারণ করা**

```javascript
const person1 = { name: "Alice" };
const person2 = { name: "Bob" };

function introduce(age) {
  console.log(`Hi, I'm ${this.name} and I'm ${age} years old.`);
}

introduce.call(person1, 25); // আউটপুট: Hi, I'm Alice and I'm 25 years old.
introduce.call(person2, 30); // আউটপুট: Hi, I'm Bob and I'm 30 years old.
```

**💡 ব্যাখ্যা:** `call()` তাৎক্ষণিকভাবে ফাংশন কল করে এবং `this` নির্ধারণ করে।

**📝 উদাহরণ ২: `apply` ব্যবহার করে অ্যারে-আকারে আর্গুমেন্ট পাস করা**

```javascript
introduce.apply(person1, [25]); // আউটপুট: Hi, I'm Alice and I'm 25 years old.
introduce.apply(person2, [30]); // আউটপুট: Hi, I'm Bob and I'm 30 years old.
```

**💡 ব্যাখ্যা:** `apply()` `call()`-এর মতোই কাজ করে, তবে আর্গুমেন্ট অ্যারে আকারে পাঠায়।

**📝 উদাহরণ ৩: `bind` ব্যবহার করে নতুন ফাংশন তৈরি করা**

```javascript
const boundFunction = introduce.bind(person1, 28);
boundFunction(); // আউটপুট: Hi, I'm Alice and I'm 28 years old.
```

**💡 ব্যাখ্যা:** `bind()` তাৎক্ষণিকভাবে ফাংশন কল করে না, বরং একটি নতুন ফাংশন তৈরি করে যা পরবর্তীতে ব্যবহার করা যায়।

### 📌 বাস্তব জীবনের প্রয়োগ

- Event Listener-এ `this` ঠিকমতো নির্ধারণ করা
- অবজেক্টের সাথে মেথড শেয়ার করা
- React-এর ফাংশন কম্পোনেন্টে `this` ঠিক রাখা

<br>

## ৮. 🚀 `map`, `filter`, এবং `reduce` সহজ ভাষায় ব্যাখ্যা

- ✅ অ্যারের উপাদান পরিবর্তন করা (`map`)
- ✅ নির্দিষ্ট মান অনুযায়ী ফিল্টার করা (`filter`)
- ✅ একটি নির্দিষ্ট ফলাফল তৈরির জন্য রিডিউস করা (`reduce`)

### 💡 সহজ উদাহরণ: জামা কাপড় গোছানো

- `map` → প্রতিটি জামা ইস্ত্রি করা (পরিবর্তন করা)।
- `filter` → পুরনো বা ছেঁড়া জামা আলাদা করা (নির্দিষ্ট কিছু বাদ দেওয়া)।
- `reduce` → সব জামা ভাঁজ করে ব্যাগে ঢুকানো (একটি নির্দিষ্ট রূপে পরিণত করা)।

### 🔍 `map`, `filter`, এবং `reduce` কীভাবে কাজ করে

**📝 উদাহরণ ১: map ব্যবহার করে প্রতিটি উপাদানের মান পরিবর্তন করা**

```javascript
const numbers = [1, 2, 3, 4, 5];

const doubled = numbers.map((n) => n * 2);
console.log(doubled); // আউটপুট: [2, 4, 6, 8, 10]
```

**💡 ব্যাখ্যা:** `map()` প্রতিটি উপাদান পরিবর্তন করে একটি নতুন অ্যারে তৈরি করে। এখানে প্রতিটি সংখ্যা দ্বিগুণ করা হয়েছে।

**📌 বাস্তব জীবনের প্রয়োগ:**

- একটি অ্যারে থেকে নতুন ফরম্যাটে ডাটা তৈরি করা
- ব্যবহারকারীর নামগুলোর প্রথম অক্ষর বড় হাতের করা
- ই-কমার্স ওয়েবসাইটে পণ্যের মূল্য পরিবর্তন করা

**📝 উদাহরণ ২: `filter` ব্যবহার করে নির্দিষ্ট উপাদান আলাদা করা**

```javascript
const ages = [12, 20, 17, 25, 30];

const adults = ages.filter((age) => age >= 18);
console.log(adults); // আউটপুট: [20, 25, 30]
```

**💡 ব্যাখ্যা:** `filter()` শুধুমাত্র নির্দিষ্ট শর্ত পূরণ করা উপাদান সংরক্ষণ করে। এখানে ১৮ বছরের কম বয়সী সবাই বাদ দেওয়া হয়েছে।

**📌 বাস্তব জীবনের প্রয়োগ:**

- শুধু নির্দিষ্ট বিভাগ অনুযায়ী পণ্য দেখানো
- ব্যবহারকারীদের মধ্যে শুধু নির্দিষ্ট বয়সের ব্যক্তিদের আলাদা করা
- একটি তালিকা থেকে শুধুমাত্র সক্রিয় সদস্যদের বের করা

**📝 উদাহরণ ৩: `reduce` ব্যবহার করে সব উপাদান একত্রিত করা**

```javascript
const prices = [10, 20, 30, 40];

const totalPrice = prices.reduce((total, price) => total + price, 0);
console.log(totalPrice); // আউটপুট: 100
```

**💡 ব্যাখ্যা:** `reduce()` প্রত্যেকটি উপাদানকে একত্রিত করে একটি নির্দিষ্ট ফলাফল তৈরি করে। এখানে সমস্ত সংখ্যাকে যোগ করে একটি মোট যোগফল তৈরি করা হয়েছে।

**📌 বাস্তব জীবনের প্রয়োগ:**

- শপিং কার্টের মোট মূল্য নির্ধারণ করা
- ব্যবহারকারীদের মধ্যে মোট ব্যয় যোগ করা
- স্ট্যাটিস্টিক্যাল বিশ্লেষণ তৈরি করা

### ⚠️ সাধারণ ভুল ও তা সংশোধনের উপায়

**❌ ভুল:** `map`, `filter`, এবং `reduce` ব্যবহার করে মূল অ্যারে পরিবর্তন করার চেষ্টা করা

**✅ সঠিক:** এগুলো সব সময় নতুন অ্যারে তৈরি করে, তাই মূল অ্যারে অপরিবর্তিত থাকে

**❌ ভুল:** `reduce()`-এর প্রারম্ভিক মান সেট না করা

**✅ সঠিক:** যদি শুরুতে কোনো মান সেট না করা হয়, তাহলে প্রথম উপাদানকে ডিফল্ট মান হিসেবে ধরে

<br>

## ৯. ⏳ `setTimeout` এবং `setInterval` কীভাবে কাজ করে (এবং কেন গুরুত্বপূর্ণ)

- **✅ সঠিকভাবে টাইমার সেট করা**
- **✅ Web API ও বিলম্বিত এক্সিকিউশন বোঝা**
- **✅ `clearTimeout` এবং `clearInterval` ব্যবহার করে টাইমার বন্ধ করা**

**💡 সহজ উদাহরণ: অ্যালার্ম ঘড়ি বনাম পুনরাবৃত্ত বিজ্ঞপ্তি**

- `setTimeout` কাজ করে **একবার নির্দিষ্ট সময়ে**—যেমন একটি **অ্যালার্ম** যা একবার বাজে।
- `setInterval` কাজ করে **বারবার নির্দিষ্ট বিরতিতে**—যেমন **নোটিফিকেশন** যা প্রতি এক মিনিটে পপ আপ হয়।

### 🔍 কীভাবে `setTimeout` এবং `setInterval` কাজ করে

**📝 উদাহরণ ১: `setTimeout` ব্যবহার করে বিলম্বিত ফাংশন কল করা**

```javascript
setTimeout(() => console.log("২ সেকেন্ড পরে হ্যালো!"), 2000);
```

**💡 ব্যাখ্যা:** `setTimeout()` ২ সেকেন্ড অপেক্ষা করে, তারপর ফাংশন চালায়।

**📝 উদাহরণ ২: `setInterval` ব্যবহার করে পুনরাবৃত্ত কাজ করা**

```javascript
let counter = 0;

const interval = setInterval(() => {
  counter++;
  console.log(`Count: ${counter}`);
  if (counter === 5) clearInterval(interval); // ৫ বার পরে বন্ধ হবে
}, 1000);
```

**💡 ব্যাখ্যা:** `setInterval()` প্রতি ১ সেকেন্ডে ফাংশন চালায়, যতক্ষণ না `counter` ৫ হয়।

### 📌 বাস্তব জীবনের প্রয়োগ

- কাউন্টডাউন টাইমার (যেমন ফ্ল্যাশ সেল, নিলাম)
- স্বয়ংক্রিয় নোটিফিকেশন (যেমন লাইভ স্পোর্টস স্কোর)
- ডাটা রিফ্রেশিং (যেমন অনলাইন চ্যাট মেসেজ লোড করা)

<br>

## ১০. 🔄 `async` এবং `await`: অ্যাসিনক্রোনাস কোড সহজ করে তোলার সবচেয়ে ভালো উপায়

- **✅ Callback Hell থেকে মুক্তি পাওয়া**
- **✅ পরিষ্কার, মেইনটেইনেবল অ্যাসিনক্রোনাস কোড লেখা**
- **✅ Error Handling করা `try...catch` দিয়ে**

### 💡 সহজ উদাহরণ: রেস্টুরেন্টে খাবার অর্ডার করা

আপনি রেস্টুরেন্টে খাবার (**Promise**) অর্ডার করেন, তারপর অপেক্ষা করেন (`await`) খাবার পরিবেশনের জন্য।

### 🔍 অ্যাসিনক্রোনাস আচরণ বোঝা

**📝 উদাহরণ ১: `async` এবং `await` এর বেসিক ব্যবহার**

```javascript
async function fetchData() {
  let response = await fetch("https://jsonplaceholder.typicode.com/todos/1");
  let data = await response.json();
  console.log(data);
}

fetchData();
```

**💡 ব্যাখ্যা:** `await` এক্সিকিউশন থামিয়ে দেয় যতক্ষণ না ডাটা ফেচ সম্পন্ন হয়, যাতে আমরা ডাটা ব্যবহার করতে পারি।

**📝 উদাহরণ ২: `try...catch` ব্যবহার করে অ্যাসিনক্রোনাস কোডের ত্রুটি হ্যান্ডল করা**

```javascript
async function fetchUserData() {
  try {
    let response = await fetch("https://invalid-url.com");
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.log("ডাটা আনতে সমস্যা:", error.message);
  }
}

fetchUserData();
```

**💡 ব্যাখ্যা:** যদি API রিকোয়েস্ট ব্যর্থ হয়, `catch` ত্রুটি হ্যান্ডল করে, স্ক্রিপ্ট ভেঙে ফেলার পরিবর্তে।

### 📌 বাস্তব জীবনের প্রয়োগ

- **API থেকে ডাটা ফেচ করা** (যেমন ইউজার প্রোফাইল লোড করা)
- **Authentication Flow পরিচালনা করা** (যেমন লগইন)
- **অ্যানিমেশন সম্পন্ন হওয়ার জন্য অপেক্ষা করা**

<br>

## ১১. 📦 `JSON` এবং `localStorage` ব্যবহার করে ডাটা সংরক্ষণ করা

- **✅ সঠিকভাবে ডাটা সংরক্ষণ ও পুনরুদ্ধার করা**
- **✅ Object-কে String-এ কনভার্ট করা**
- **✅ Persistent Data সংরক্ষণ করা**

### 💡 সহজ উদাহরণ: নোটবুকে তথ্য লেখা ও পরে পড়া

`localStorage` **একটি নোটবুকের মতো**, যেখানে আপনি তথ্য লিখতে পারেন এবং পরে তা ফিরে পেতে পারেন—even ব্রাউজার বন্ধ হলেও।

### 🔍 কীভাবে ডাটা সংরক্ষণ ও পুনরুদ্ধার করা যায়

**📝 উদাহরণ ১: `localStorage` ব্যবহার করে ডাটা স্টোর ও রিট্রিভ করা**

```javascript
const user = { name: "Alice", age: 25 };

localStorage.setItem("user", JSON.stringify(user));
const retrievedUser = JSON.parse(localStorage.getItem("user"));

console.log(retrievedUser.name); // আউটপুট: Alice
```

**💡 ব্যাখ্যা:** **`localStorage` শুধুমাত্র String সংরক্ষণ করতে পারে**, তাই আমরা `JSON.stringify()` ব্যবহার করে Object কে String-এ কনভার্ট করি, এবং `JSON.parse()` ব্যবহার করে পুনরুদ্ধার করি।

**📝 উদাহরণ ২: `localStorage` থেকে নির্দিষ্ট ডাটা মুছে ফেলা**

```javascript
localStorage.removeItem("user"); // নির্দিষ্ট ডাটা মুছে ফেলবে
localStorage.clear(); // সব সংরক্ষিত ডাটা মুছে ফেলবে
```

**💡 ব্যাখ্যা:** **`removeItem()` নির্দিষ্ট ডাটা ডিলিট করে**, আর **`clear()` `localStorage`-এর সব কিছু মুছে ফেলে**।

### 📌 বাস্তব জীবনের প্রয়োগ

- **ইউজার প্রিফারেন্স সংরক্ষণ করা** (যেমন Dark Mode, ভাষার সেটিংস)
- **Shopping Cart Data সংরক্ষণ করা** (ই-কমার্স ওয়েবসাইটে)
- **Form Input সংরক্ষণ করা** (যেমন অটো-ফিল করা Contact Form)

<br>

## ১২. 🏗️ ES6 Classes: Object-Oriented JavaScript সহজ করার সবচেয়ে ভালো উপায়

- ✅ Reusable Object Template তৈরি করা
- ✅ Constructor এবং Methods ব্যবহার করা
- ✅ Inheritance (বংশানুক্রমিক বৈশিষ্ট্য) যোগ করা

### 💡 সহজ উদাহরণ: খেলনার কারখানা

একটি কারখানা **নির্দিষ্ট কাঠামো অনুযায়ী খেলনা তৈরি করে**। JavaScript-এ **Classes একইভাবে কাজ করে—একটি সাধারণ কাঠামো থেকে নতুন অবজেক্ট তৈরি করতে সাহায্য করে**।

### 🔍 JavaScript-এ Class কীভাবে কাজ করে

**📝 উদাহরণ ১: Class ডিফাইন ও ব্যবহার করা**

```javascript
class Toy {
  constructor(name, price) {
    this.name = name;
    this.price = price;
  }
  display() {
    console.log(`${this.name} এর দাম $${this.price}`);
  }
}

const toyCar = new Toy("গাড়ি", ১০);
toyCar.display(); // আউটপুট: গাড়ি এর দাম $10
```

**💡 ব্যাখ্যা:** Toy ক্লাস **একটি সাধারণ কাঠামো প্রদান করে**, যা থেকে আমরা **অনেক খেলনা অবজেক্ট তৈরি করতে পারি**।

**📝 উদাহরণ ২ঃ অন্য ক্লাস থেকে বৈশিষ্ট্য ইনহেরিট করা**

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

**💡 ব্যাখ্যা:** `Vehicle` ক্লাসকে `Car` ক্লাস ইনহেরিট করেছে, মানে সকল গাড়িগুলো এখন স্বয়ংক্রিয়ভাবে `type` প্রোপার্টিটি পেয়ে যাবে।

### 📌 বাস্তব জীবনের প্রয়োগ

- **গেম ক্যারেক্টার তৈরি করা** (যেমন RPG গেমে প্লেয়ার স্ট্যাটস)
- **React UI কম্পোনেন্ট তৈরি করা**
- **ইউজার প্রোফাইল মডেল তৈরি করা** (যেমন এডমিনিস্ট্রেটর, এডিটর, ভিউয়ার রোলগুলো)

<br>

## ১৩. 🔟 🚨 কেন JavaScript-এ `"use strict"` ব্যবহার করা উচিত (এবং কীভাবে এটি কোডকে নিরাপদ করে)

- **✅ কমন ভুল প্রতিরোধ করা**
- **✅ ভালো কোডিং অভ্যাস তৈরি করা**
- **✅ অপ্রত্যাশিত ভুল ধরতে সাহায্য করা**

### 💡 সহজ উদাহরণ: কঠোর নিয়ম অনুসরণকারী শিক্ষক

একজন শিক্ষক **সকল শিক্ষার্থীকে সঠিক নিয়ম অনুসরণ করতে বাধ্য করেন**, যাতে তারা **ভুল না করে**। JavaScript-এ `"use strict"` **একইভাবে কাজ করে—ভুলভাবে লেখা কোডকে ধরতে সাহায্য করে**।

### 🔍 `"use strict"` কীভাবে কাজ করে

**📝 উদাহরণ ১: অঘোষিত ভেরিয়েবল ব্যবহার করলে ত্রুটি পাওয়া**

```javascript
"use strict";

x = 10; // ত্রুটি! `x` ঘোষণা করা হয়নি
```

**💡 ব্যাখ্যা:** `"use strict"` **কোডে ভুল ধরতে সাহায্য করে**, যাতে আমরা **অঘোষিত ভেরিয়েবল ব্যবহার করতে না পারি**।

**📝 উদাহরণ ২: অবজেক্টের পরিবর্তন আটকানো**

```javascript
"use strict";

const person = Object.freeze({ name: "Alice" });

person.name = "Bob"; // ত্রুটি! অবজেক্ট পরিবর্তন করা যাবে না
```

**💡 ব্যাখ্যা:** `"use strict"` **নিরাপত্তা নিশ্চিত করে**, যাতে অবজেক্ট ফ্রিজ থাকলে তা পরিবর্তন করা না যায়।

### 📌 বাস্তব জীবনের প্রয়োগ

- **প্রোডাকশন কোড নিরাপদ রাখা**
- **ত্রুটি দ্রুত খুঁজে বের করা**
- **বৈধ ভেরিয়েবল ও ফাংশন ব্যবহার নিশ্চিত করা**

<br>

## ১৪. 🛡️ JavaScript-এর `try...catch`: ত্রুটি হ্যান্ডলিংয়ের গোপন অস্ত্র

- **✅ প্রত্যাশিত ত্রুটি হ্যান্ডল করা**
- **✅ ব্যবহারকারীর অভিজ্ঞতা উন্নত করা**
- **✅ কোডকে সহজে ডিবাগ করা**

### 💡 সহজ উদাহরণ: নিরাপত্তা জাল

যদি আপনি **একটি উঁচু বিল্ডিং থেকে লাফ দেন**, তাহলে **নিরাপত্তা জাল আপনাকে থেকে রক্ষা করবে**। JavaScript-এ `try...catch` **একইভাবে কাজ করে—যদি কোনো ত্রুটি ঘটে, এটি সেটিকে ধরতে সাহায্য করে**।

### 🔍 `try...catch` কীভাবে কাজ করে

**📝 উদাহরণ ১: সাধারণ ত্রুটি ধরতে `try...catch` ব্যবহার**

```javascript
try {
  let result = 5 / 0;
  console.log(result);
} catch (error) {
  console.log("ত্রুটি ঘটেছে:", error.message);
}
```

**💡 ব্যাখ্যা:** `try...catch` **ত্রুটির জন্য কোড ব্লক পরীক্ষা করে**, এবং **ত্রুটি থাকলে তা সুন্দরভাবে হ্যান্ডল করে**।

**📝 উদাহরণ ২: API থেকে ডাটা ফেচ করার সময় ত্রুটি হ্যান্ডলিং**

```javascript
async function fetchData() {
  try {
    let response = await fetch("https://invalid-url.com");
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.log("ডাটা আনতে সমস্যা:", error.message);
  }
}

fetchData();
```

**💡 ব্যাখ্যা:** যদি API রিকোয়েস্ট ব্যর্থ হয়, `catch` **ত্রুটি হ্যান্ডল করে, যাতে স্ক্রিপ্ট ভেঙে না যায়**।

### 📌 বাস্তব জীবনের প্রয়োগ

- ব্যবহারকারীর ইনপুট ভ্যালিডেট করা
- API ত্রুটি হ্যান্ডল করা
- ব্যবহারকারীকে সুন্দরভাবে ত্রুটি দেখানো

## ১৫. 🔑 `Object.keys()`, `Object.values()`, এবং `Object.entries()` ব্যবহার করে ডাটা বের করা

- **✅ অবজেক্ট থেকে তথ্য সহজে বের করা**
- **✅ অবজেক্টকে অ্যারে-তে রূপান্তর করা**
- **✅ অবজেক্টের উপর লুপ চালানো সহজ করা**

### 💡 সহজ উদাহরণ: একটি আলমারি/লকার সংগঠিত করা

একটি আলমারিতে অনেক দরজা (properties) থাকে—কখনো দরজার নাম দরকার হয়, কখনো ভিতরের জিনিস। JavaScript-এ `Object.keys()`, `Object.values()` এবং `Object.entries()` **একসাথে এই কাজগুলো করতে পারে**।

### 🔍 অবজেক্ট থেকে তথ্য বের করা

**📝 উদাহরণ ১: অবজেক্টের কী (properties) বের করা**

```javascript
const person = { name: "Alice", age: 25 };

console.log(Object.keys(person)); // ["name", "age"]
```

**💡 ব্যাখ্যা:** `Object.keys()` অবজেক্টের সব **properties-এর নামকে অ্যারে আকারে দেয়**।

**📝 উদাহরণ ২: অবজেক্টের ভ্যালুগুলো বের করা**

```javascript
console.log(Object.values(person)); // ["Alice", 25]
```

**💡 ব্যাখ্যা:** `Object.values()` অবজেক্টের **ভ্যালুগুলো অ্যারে আকারে দেয়**।

**📝 উদাহরণ ৩: কী এবং ভ্যালু একসাথে বের করা**

```javascript
console.log(Object.entries(person)); // [["name", "Alice"], ["age", 25]]
```

**💡 ব্যাখ্যা:** `Object.entries()` একসাথে **কী এবং ভ্যালু অ্যারে হিসেবে দেয়**।

### 📌 বাস্তব জীবনের প্রয়োগ

- **অবজেক্টকে অ্যারে-তে রূপান্তর করা** (ডাটাবেস কুয়েরির জন্য দরকারি)
- **ডাটা ফিল্টার করা ও সাজানো** (যেমন ইউজারের প্রোফাইল সাজানো)
- **API থেকে ফেচ করা ডাটা পরিচালনা করা** (এপের জটিল সেটিংস হ্যান্ডল করা)

<br>

## ১৬. ⏱️ জাভাস্ক্রিপ্টে _ডিবাউন্স_ এবং _থ্রটল_: কিভাবে ফাংশনের সময় ঠিকমতো নিয়ন্ত্রণ করবেন

- **✅ আপনার ফাংশনকে অপ্রয়োজনীয় বারবার চলা থেকে থামান**
- **✅ ল্যাগি ইউআই বন্ধ করুন**
- **✅ দামী হিসাব-নিকাশ অপ্টিমাইজ করুন, স্মার্ট ইভেন্ট হ্যান্ডলিং শিখুন**

### 🧠 সহজ উদাহরণ: কথা বলার সময় ঠিক রাখা

ভাবুন কেউ গ্রুপ কলে বারবার মাইকের বোতাম চাপছে।

- **Debounce (ডিবাউন্স):** তাকে শুধু তখনই কথা বলতে দেব যখন সে ৩ সেকেন্ড ধরে বোতাম না চাপবে।
- **Throttle (থ্রটল):** তাকে প্রতি ৩ সেকেন্ডে একবার করে কথা বলতে দেব, যতবারই সে চাপ দিক না কেন।

এইভাবেই আপনি **ব্রাউজারে অনেক বেশি ইভেন্ট আসা নিয়ন্ত্রণ** করতে পারেন—ইউআইকে স্মার্ট এবং ফাস্ট রাখবেন।

### 🧪 উদাহরণ ১: Debounce – ইউজার টাইপ করা বন্ধ না করলে কিছু করো না

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
optimizedSearch(); // এটা তখনই চলবে যখন ৩০০মিলিসেকেন্ডের মধ্যে আবার না কল করা হয়
```

**💡 সহজ ব্যাখ্যা:**

- `debounce(func, delay)` আপনার আসল ফাংশনটা প্যাক করে এবং সময়ের উপর নিয়ন্ত্রণ রাখে।
- `let timeout;` আগের নির্ধারিত টাইমার মনে রাখে।
- `clearTimeout(timeout);` আগের টাইমার বাতিল করে দেয়।
- `setTimeout(..., delay);` নতুন একটা টাইমার শুরু করে যা ফাংশন চালাতে দেরি করে।

**📌 কেন এটা দরকার:**

- ফাংশনটা তখনই চলে যখন ইউজার কিছুক্ষণ কিছু না করে (যেমন টাইপ বন্ধ করে)।
- প্রতিটা টাইপ নতুন করে টাইমার চালু করে—**শেষটাই শুধু কাজে লাগে**।

**🛠 ডিবাউন্স ব্যবহার করুন যখন:**

- সার্চ বক্সে টাইপিং হয়
- টাইপ করার সময় অটো-সেভ দরকার
- ইউজার ইনপুট রেসপন্সিভ রাখতে হয়

### 🧪 উদাহরণ ২: Throttle – প্রতি নির্দিষ্ট সময় পর পরই শুধু চলবে

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

**💡 সহজ ব্যাখ্যা:**

- `throttle(func, limit)` নিশ্চিত করে যে আপনার ফাংশন নির্দিষ্ট সময়ের আগে বারবার চলবে না।
- `let lastCall = 0;` শেষ বার কবে ফাংশন চলেছিল সেটা মনে রাখে।
- `Date.now()` ইভেন্টের সময় বের করে।
- `if (now - lastCall >= limit)` দেখে ঠিক সময় পার হয়েছে কিনা।

**📌 কেন এটা দরকার:**

- এমনকি যদি ইভেন্ট (যেমন স্ক্রল) বারবার হয়, তবুও ফাংশনটা ঠিক সময় পর পর চলে।
- এর ফলে পারফর্মেন্স ভালো থাকে এবং অ্যাপ স্লো হয় না।

**🛠 থ্রটল ব্যবহার করুন যখন:**

- স্ক্রল লিসেনার দরকার
- রিসাইজ ইভেন্ট আছে
- বারবার বাটনে চাপা ঠেকাতে হয়

### ❌ কিছু সাধারণ ভুল এবং এড়িয়ে চলার উপায়

| ⚠️ ভুল                  | ❌ সমস্যা                        | ✅ সঠিক পদ্ধতি                                                           |
| ----------------------- | -------------------------------- | ------------------------------------------------------------------------ |
| স্ক্রল ইভেন্টে ডিবাউন্স | অনেক আপডেট মিস হয়                | **থ্রটল ব্যবহার করুন যাতে নিয়মিত আপডেট পাওয়া যায়**                       |
| clearTimeout না দেওয়া   | অপ্রয়োজনীয় এক্সিকিউশন হয়         | **প্রথমে অবশ্যই** `clearTimeout()` **ব্যবহার করুন**                      |
| টাইমিং ভুলভাবে নির্ধারণ | ইউআই ল্যাগি বা অতিসেন্সিটিভ লাগে | **ডিবাউন্সের জন্য** `300ms`, **থ্রটলের জন্য** `100–250ms` দিয়ে শুরু করুন |

### 🌍 বাস্তব জীবনের কিছু ব্যবহার

**ডিবাউন্স**

- সার্চ বক্সে টাইপ করা
- ইনপুট অটো-সেভ করা
- ইউজার থামলে ইনপুট যাচাই করা

**থ্রটল**

- স্ক্রল পজিশন ট্র্যাক করা
- স্ক্রল বেইসড অ্যানিমেশন
- অনেক API কল কমিয়ে আনা

### 🧾 সংক্ষেপে

| টেকনিক       | কী করে                                         | কোথায় ভালোভাবে কাজ করে                      |
| ------------ | ---------------------------------------------- | ------------------------------------------- |
| **Debounce** | ইউজার ইভেন্ট থামালে ফাংশন চালায়                | লাইভ সার্চ, ইনপুট ক্লিনআপ, স্মুথ ইউআই       |
| **Throttle** | অনেক ইভেন্টেও নির্দিষ্ট সময় পর পরই ফাংশন চালায় | স্ক্রল, রিসাইজ, রেট-লিমিট করা ইন্টারঅ্যাকশন |

<br>

## ১৭. 🎯 জাভাস্ক্রিপ্টে ইভেন্ট _ডেলিগেশন_ : কম দিয়ে বেশি ইভেন্ট হ্যান্ডল করুন

- **✅ ইভেন্ট লিসেনার কমান**
- **✅ DOM ম্যানেজমেন্ট সহজ করুন**
- **✅ ডাইনামিক এলিমেন্ট সহজেই সাপোর্ট করুন**

### 🧠 সহজ উদাহরণ: একজন বাউন্সার, অনেক অতিথি

ভাবুন আপনি একটা পার্টি দিচ্ছেন। প্রতিটা অতিথির পাশে বাউন্সার না বসিয়ে **দরজার পাশে একজন রাখলেন**, সে-ই সবাইকে দেখবে।

Event Delegation ঠিক তাই—**একটা parent element-এ একটা ইভেন্ট লিসেনার বসান** আর চেক করুন কোন child ইভেন্ট ট্রিগার করেছে।

### 🧪 উদাহরণ ১: তালিকায় ক্লিক হ্যান্ডলিং

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

**💡 ব্যাখ্যা:**

- ক্লিক লিসেনার `<li>` তে না বসিয়ে `<ul>` তে বসানো হয়েছে।
- `e.target` বলে দেয় ঠিক কোন এলিমেন্টে ক্লিক হয়েছে।
- নতুন `<li>` এলিমেন্ট এলেও এটা কাজ করবে!

### 🧪 উদাহরণ ২: ডাইনামিক নোটিফিকেশন ম্যানেজমেন্ট

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

**💡 ব্যাখ্যা:**

- আমরা `.notifications` কনটেইনারে লিসেনার বসিয়েছি।
- যদি `.close` বাটনে ক্লিক হয়, তাহলে তার কাছের `.toast` মুছে ফেলা হয়।
- **একটাই লিসেনার** দিয়ে যেকোনো **সংখ্যক toast** হ্যান্ডল করা যায়—even যদি পরে যোগ হয়।

### 🧪 উদাহরণ ৩: ইনপুট ফোকাস ইভেন্ট ডেলিগেশনের মাধ্যমে

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

**💡 ব্যাখ্যা:**

- `focusin` ইভেন্ট bubble করে (কিন্তু `focus` করে না), তাই এটা delegate করা যায়।
- সব `<input>` এর জন্য একটাই লিসেনার যথেষ্ট।
- styling বা validation করার জন্য আলাদা করে লিসেনার বসাতে হয় না।

### ❌ কিছু সাধারণ ভুল এবং এড়ানোর উপায়

| ভুল                                  | সমস্যা                                  | সঠিক করণীয়                                   |
| ------------------------------------ | --------------------------------------- | -------------------------------------------- |
| `e.currentTarget` ব্যবহার করা        | এটা সবসময় parent এলিমেন্টকেই দেখায়      | `e.target` ব্যবহার করুন সঠিক এলিমেন্ট ধরতে   |
| ইভেন্ট টার্গেট না ফিল্টার করা        | অপ্রাসঙ্গিক ক্লিকেও ফাংশন চলে যেতে পারে | `.matches()` বা ক্লাস/ট্যাগ চেক ব্যবহার করুন |
| ডাইনামিক আইটেমে সরাসরি লিসেনার বসানো | নতুন আইটেমে ইভেন্ট কাজ করবে না          | parent এলিমেন্ট থেকে delegate করুন           |

### 🌍 বাস্তব জীবনের কিছু ব্যবহার

- ডাইনামিক **টুডু লিস্ট** এ delete বাটন
- রিইউজেবল **মোডাল** বা **ট্যাব**
- ডেলিগেটেড **ফর্ম validation**
- ড্রপডাউন বা মোবাইল নেভ **মেনু** ম্যানেজ করা

### 🧾 সংক্ষেপে

| ফিচার                | কী করে                                                          | উপকারিতা                                |
| -------------------- | --------------------------------------------------------------- | --------------------------------------- |
| **Event Delegation** | **parent এলিমেন্টে শুনে**, সব **child ইভেন্টে প্রতিক্রিয়া দেয়** | কম কোড, ভালো পারফর্মেন্স, ডাইনামিক রেডি |

<br>

## ১৮. 🎛️ ইভেন্ট _বাবলিং_ এবং _ক্যাপচারিং_ জাভাস্ক্রিপ্টে: কীভাবে ইভেন্ট প্রবাহ কাজ করে

- **✅ DOM ইভেন্ট ফ্লো ভালোভাবে বুঝুন**
- **✅ অপ্রত্যাশিত আচরণ ঠিক করুন**
- **✅ ইভেন্ট ডেলিগেশন ও UI ডিজাইনে দক্ষতা বাড়ান**

### 🧠 সহজ উদাহরণ: এসকেলেটর আর ভিড়

ধরুন আপনি শপিং মলে আছেন:

- **Capturing phase:** উপরের তলা থেকে নিরাপত্তাকর্মী কাউকে সন্দেহ করছে এবং নিচে নামছে তাকে অনুসরণ করে।

- **Target phase:** সেই ব্যক্তি একটি দোকানে পৌঁছায়—এখন সে কেন্দ্রে।

- **Bubbling phase:** সে যখন ফুড কোর্টে নামছে, তখন সবাই তাকে দেখে প্রতিক্রিয়া দিচ্ছে।

জাভাস্ক্রিপ্টেও **ইভেন্ট এমনভাবেই চলে**: DOM-এর **সর্বোচ্চ স্তর থেকে টার্গেট এলিমেন্টে, তারপর আবার উপরে ফিরে যায়।**

### 🚦 DOM-এ ইভেন্ট ফ্লো কিভাবে কাজ করে

1. **Capture Phase (নিচে নামে):** ইভেন্ট `<html>` থেকে শুরু হয়ে টার্গেট এলিমেন্টের দিকে যায়।
2. **Target Phase:** ইভেন্ট আসল যেই এলিমেন্টে ইউজার ক্লিক করেছে, সেখানে পৌঁছায়।
3. **Bubble Phase (উপরে উঠে):** ইভেন্ট DOM ট্রি ধরে আবার উপরের দিকে ফিরে যায়।

ডিফল্টভাবে, **ইভেন্ট লিসেনার বাবলিং ফেজ ব্যবহার করে**—তবে `{ capture: true }` সেট করে ক্যাপচারিং ফেজও ব্যবহার করা যায়।

### 🧪 উদাহরণ ১: ডিফল্ট বাবলিং আচরণ

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

**💡 ব্যাখ্যা:**

- বাটনে ক্লিক করলে দেখবেন 👉 `Child clicked!` তারপর 👉 `Parent clicked!`
- ইভেন্ট #child এ শুরু হয়, তারপর **বাবল হয়ে** parent এ পৌঁছে।
- এটাই ডিফল্ট আচরণ এবং **ইভেন্ট ডেলিগেশনের ভিত্তি।**

### 🧪 উদাহরণ ২: ক্যাপচার ফেজ ব্যবহার

```javascript
document.getElementById("parent").addEventListener(
  "click",
  () => {
    console.log("Parent capturing!");
  },
  { capture: true }
);
```

**💡 ব্যাখ্যা:**

- `{ capture: true }` দিলে ইভেন্ট **নিচে নামার সময়** parent এ হ্যান্ডল হয়—টার্গেটে পৌঁছানোর আগে।
- এখন বাটনে ক্লিক করলে দেখবেন: 👉 `Parent capturing!` তারপর 👉 `Child clicked!`
- যখন আপনি চাই parent লজিক আগে চলুক—তখন এটা খুব কাজের।

### 🧪 উদাহরণ ৩: ইভেন্ট বাবলিং থামানো

```javascript
document.getElementById("child").addEventListener("click", (e) => {
  e.stopPropagation();
  console.log("Child clicked, bubbling stopped!");
});
```

**💡 ব্যাখ্যা:**

- `e.stopPropagation()` **ইভেন্টকে উপরে উঠতে দেয় না**।
- parent আর ইভেন্ট পাবে না—modals বা dropdown-এর মত isolate দরকার হলে এটা দরকার।

### ❌ কিছু সাধারণ ভুল

| ⚠️ ভুল                       | সমস্যা                                         | সমাধান                                             |
| ---------------------------- | ---------------------------------------------- | -------------------------------------------------- |
| শুধু বাবলিং এর উপর নির্ভর    | কিছু ইভেন্ট (যেমন `blur`, `focus`) বাবল করে না | **ক্যাপচার ফেজ** ব্যবহার করুন বা বিকল্প ইভেন্ট নিন |
| `stopPropagation()` না দেওয়া | parent লজিক child এর উপর প্রভাব ফেলে           | প্রয়োজনে বাবলিং বন্ধ করুন                         |
| বেশি ক্যাপচার ব্যবহার করা    | ডিবাগ করা কঠিন হয়ে পড়ে                         | কেবল গুরুত্বপূর্ণ ইন্টারসেপ্টে ব্যবহার করুন        |

### 🌍 বাস্তব জীবনের কিছু ব্যবহার

- **ইভেন্ট ডেলিগেশন** বাবলিংয়ের উপর কাজ করে
- **ড্রপডাউন মেনু** বন্ধ হওয়া ঠেকানো
- **প্যারেন্ট লজিক** আগে চালানো
- **মোডাল বা নেস্টেড UI** এর মধ্যে ইভেন্ট চেইন থামানো

### 🧾 সংক্ষেপে

| ফেজ       | দিক            | কোন লিসেনার ট্রিগার হয়                  |
| --------- | -------------- | --------------------------------------- |
| Capturing | উপরে → টার্গেট | `{ capture: true }` সহ লিসেনার          |
| Target    | —              | টার্গেট এলিমেন্টেই ইভেন্ট পড়ে           |
| Bubbling  | টার্গেট → উপরে | ডিফল্টভাবে প্রায় সব লিসেনার এই ফেজে চলে |

<br>

## ১৯. 🧠 জাভাস্ক্রিপ্টে মেমোরি ম্যানেজমেন্ট: লিক বন্ধ করুন, অ্যাপ অপটিমাইজ করুন

- **✅ Garbage Collector কীভাবে কাজ করে বুঝুন**
- **✅ লুকানো মেমোরি লিক এড়িয়ে চলুন**
- **✅ আপনার অ্যাপ রাখুন হালকা ও দ্রুত**

### 🧠 সহজ উদাহরণ: মেমোরি মানে কাজের ডেস্ক

ভাবুন আপনার অ্যাপ একটা ডেস্কে কাজ করছে। সে ফাইল (অবজেক্ট) খোলে, কাগজ জমায় (ভ্যারিয়েবল), ফোল্ডার রাখে (DOM এলিমেন্ট)। কিন্তু যদি **সেগুলো কখনো পরিষ্কার না করে**, ডেস্ক এলোমেলো হয়ে যায় — এবং অ্যাপ ধীর হয়ে পড়ে।

জাভাস্ক্রিপ্টের মেমোরি মডেল অপ্রয়োজনীয় জিনিস সরিয়ে দেয় (যেমন আবর্জনা ফেলা), কিন্তু আপনাকেই জানতে হবে **কোন জিনিসগুলো জ্যাম তৈরি করছে** এবং কীভাবে সেটা পরিষ্কার রাখবেন।

### 🧪 উদাহরণ ১: জাভাস্ক্রিপ্ট মেমোরির লাইফসাইকেল

```javascript
function createUser() {
  const user = {
    name: "Saief",
    skills: ["React", "TypeScript"],
  };
  return user;
}

const newUser = createUser();
```

**💡 ব্যাখ্যা:**

- `user` মেমোরিতে তৈরি হয় যখন ফাংশন চলে।
- যখন এটা `newUser` এ দেওয়া হয়, তখনও এটা অ্যাক্সেসযোগ্য থাকে।
- সব রেফারেন্স মুছে গেলে, **garbage collector** এটা সরিয়ে ফেলবে।

### 🔍 কীভাবে মেমোরি লিক হয়?

মেমোরি লিক হয় যখন **অপ্রয়োজনীয় ডেটা** এখনও **মেমোরিতে রয়ে যায়**, যা অ্যাপকে ভারী করে তোলে। সাধারণ কারণগুলো:

- ❗ ভুলে যাওয়া timer বা interval
- ❗ DOM থেকে সরানো এলিমেন্ট
- ❗ পুরনো ডেটা ধরে রাখা closure
- ❗ কখনো না মুছে ফেলা global variables

### 🧪 উদাহরণ ২: `setInterval` দিয়ে লিক

```javascript
function startCounter() {
  setInterval(() => {
    console.log("Running forever...");
  }, 1000);
}
```

**💡 কী হচ্ছে:**

- এই `setInterval` **চিরকাল চলে**, আর তার closure সবকিছুর রেফারেন্স ধরে রাখে।
- `startCounter()` শেষ হলেও, মেমোরি আটকে থাকে।
- **🔧 সমাধান:** দরকার শেষে `clearInterval()` দিয়ে বন্ধ করুন।

### 🧪 উদাহরণ ৩: Detached DOM Nodes

```javascript
const container = document.getElementById("list");
let tempDiv = document.createElement("div");
tempDiv.textContent = "Temp";
container.appendChild(tempDiv);
container.removeChild(tempDiv); // পরিষ্কার মনে হচ্ছে, তাই তো?
```

**💡 সমস্যা:**

- আপনার কোড যদি `tempDiv`-এর রেফারেন্স ধরে রাখে (ভ্যারিয়েবল বা ইভেন্ট লিসেনার), তাহলে ব্রাউজার এটা মুছবে না।
- **🔧 সমাধান:** রেফারেন্স `null` করে দিন এবং ইভেন্ট লিসেনার সরান।

### ✅ পরিচ্ছন্ন মেমোরির জন্য ভালো অভ্যাস

- 🧹 `let` বা `const` দিয়ে স্পষ্ট স্কোপ ব্যবহার করুন
- 🧹 DOM এলিমেন্ট সরালে ইভেন্ট লিসেনারও সরান
- 🧹 `setInterval`, `setTimeout` ক্লিয়ার করুন
- 🧹 গ্লোবাল ভ্যারিয়েবল এড়িয়ে চলুন
- 🧹 দীর্ঘস্থায়ী ক্লোজার থেকে সাবধান থাকুন (বিশেষ করে SPA-তে)

### ❌ সাধারণ ভুল

| ভুল                                | কী সমস্যা হয়                   | কী করবেন                                     |
| ---------------------------------- | ------------------------------ | -------------------------------------------- |
| DOM সরিয়ে ফেলার পরও রেফারেন্স রাখা | এলিমেন্ট garbage collect হয় না | `null` করুন, `removeEventListener()` দিন     |
| `setInterval` বন্ধ না করা          | ফাংশন চিরকাল মেমোরিতে থেকে যায় | সবসময় `clearInterval()` ব্যবহার করুন         |
| বড় `closure` রাখা                  | অজান্তে বড় ডেটা আটকে পড়ে       | শুধুমাত্র দরকারি জিনিস রাখুন ক্লোজারে        |
| থার্ড-পার্টি লাইব্রেরির লিক        | হিডেন লিসেনার বা ক্যাশ জমা হয়  | DevTools দিয়ে চেক করুন, আনমাউন্টে ক্লিন করুন |

### 🧾 সংক্ষেপে

| টার্ম                  | মানে                                     | টিপস                                       |
| ---------------------- | ---------------------------------------- | ------------------------------------------ |
| **Garbage Collection** | অ্যাক্সেসহীন মেমোরি নিজে নিজে সরিয়ে ফেলা | ব্যাকগ্রাউন্ডে চলে, কিন্তু সবসময় নিখুঁত নয় |
| **Memory Leak**        | ডেটা দরকার নেই, তবু মেমোরিতে থেকে যাচ্ছে | বেশি রেফারেন্স থাকার কারণেই হয়             |
| **Reference**          | ভ্যারিয়েবল বা ক্লোজার যা ডেটা ধরে রাখে   | `null` করুন বা ক্লিনআপ ফাংশন ব্যবহার করুন  |

<br>

## ২০. ⛓️ জাভাস্ক্রিপ্টে ব্লকিং বনাম নন-ব্লকিং কোড কীভাবে কাজ করে

- **✅ সিঙ্ক্রোনাস এবং অ্যাসিঙ্ক্রোনাস এক্সিকিউশন বোঝা**
- **✅ UI হ্যাং বা ল্যাগ হওয়া ঠেকানো**
- **✅ স্মুথ ও স্কেলেবল কোড লেখা শিখুন**

### 🧠 সহজ উদাহরণ: এক লেনে হেঁটে যাওয়া বনাম মাল্টিটাস্কিং

ধরুন কেউ একটার পর একটা কাজ করছে:

- **ব্লকিং কোড** মানে লাইনে দাঁড়িয়ে থাকা - আপনি সামনে থাকা ব্যক্তি শেষ না করা পর্যন্ত নড়তে পারবেন না।

- **নন-ব্লকিং কোড** মানে কফির জন্য লাইনে দাঁড়িয়ে বন্ধুকে টেক্সট পাঠানো - অন্য কাজও আপনি একসাথে করে যেতে পারেন।

জাভাস্ক্রিপ্ট ডিফল্টভাবে **একটি থ্রেড** এ চলে। কিন্তু তার **ইভেন্ট লুপ** এর কারণে অ্যাসিঙ্ক্রোনাস কাজগুলি হ্যান্ডেল করতে পারে, UI ফ্রিজ না করেই।

### 🧪 উদাহরণ ১: ব্লকিং কোড (সিঙ্ক্রোনাস)

```javascript
console.log("Start");

function heavyTask() {
  for (let i = 0; i < 1e9; i++) {}
}

heavyTask();
console.log("End");
```

**💡 ব্যাখ্যা:**

- `heavyTask()` সম্পন্ন না হওয়া পর্যন্ত অন্য কিছু চলবে না।
- `console.log("End")` চলবে তখনই, যখন `heavyTask` শেষ হবে।
- 🛑 পুরো থ্রেড ব্লক হয়ে থাকে-UI, রেসপন্স সব থেমে যায়।

**📌 সাধারণত হয় যখন:**

- বড় লুপ বা কম্পিউটেশন করা হয়
- সিঙ্ক ফাইল পড়া হয়
- বড় JSON পার্সিং বা রেগুলার এক্সপ্রেশন

### 🧪 উদাহরণ ২: নন-ব্লকিং কোড (অ্যাসিঙ্ক্রোনাস)

```javascript
console.log("Start");

setTimeout(() => {
  console.log("Async Task");
}, 1000);

console.log("End");
```

**💡 ব্যাখ্যা:**

- `setTimeout()` ইভেন্ট লুপের মাধ্যমে ভবিষ্যতের জন্য শিডিউল হয়।
- `console.log("End")` তৎক্ষণাৎ চলে, কোনো অপেক্ষা ছাড়াই।
- ✅ এর ফলে অ্যাপ অন্য কোড চালাতে পারে, অপেক্ষা না করেই।

**📌 সাধারণ অ্যাসিঙ্ক্রোনাস প্যাটার্ন:**

- `setTimeout` / `setInterval`
- `Promise` / `async-await`
- `fetch` বা অন্যান্য I/O অপারেশন

### 🔄 ইভেন্ট লুপ কীভাবে সাহায্য করে

জাভাস্ক্রিপ্ট ব্যবহার করে:

- **Call Stack:** কোন ফাংশন চলছে তা ট্র্যাক করে
- **Web APIs:** অ্যাসিঙ্ক ফাংশন বাইরে পাঠায় (যেমন `setTimeout`, `fetch`)
- **Callback Queue:** যে টাস্ক গুলো অপেক্ষা করছে
- **Event Loop:** স্ট্যাক খালি হলে কিউ থেকে টাস্ক চালায়

✅ এই সিস্টেমের ফলে জাভাস্ক্রিপ্ট **এক থ্রেডে** থেকেও "মাল্টিটাস্ক"-এর মতো আচরণ করতে পারে।

### 🧪 উদাহরণ ৩: ব্লকিং আর নন-ব্লকিং একসাথে

```javascript
console.log("Start");

setTimeout(() => {
  console.log("Delayed task");
}, 0);

for (let i = 0; i < 1e9; i++) {}

console.log("End");
```

**💡 ব্যাখ্যা:**

- 0ms delay দিলেও, লুপ শেষ না হওয়া পর্যন্ত `setTimeout` চলবে না।
- প্রমাণ: **ব্লকিং কোড ইভেন্ট কিউ আটকে দেয়**, যতক্ষণ না কল স্ট্যাক খালি হয়।
- মনে রাখুন: অ্যাসিঙ্ক কাজ করতে হবে **ব্লকিং ছাড়াই**, নয়তো লাভ নেই।

### ❌ সাধারণ ভুল

| ভুল                                      | কী সমস্যা হয়                        | কী করবেন                                       |
| ---------------------------------------- | ----------------------------------- | ---------------------------------------------- |
| বড় সিঙ্ক কোড UI-তে রাখলে                 | বাটন ফ্রিজ করে, ইউজার ল্যাগ ফিল করে | Web worker বা ছোট অ্যাসিঙ্ক অংশে ভাগ করুন      |
| `setTimeout(..., 0)` কে ইনস্ট্যান্ট ভাবা | স্ট্যাক ব্যস্ত থাকলে দেরি হয়        | গুরুত্বপূর্ণ কোড হালকা ও দ্রুত রাখুন           |
| API ডেটা সিঙ্ক লুপে আনলে                 | ডেটা না আসা পর্যন্ত UI আটকে থাকে    | `fetch`, `Promise`, `async-await` ব্যবহার করুন |

### 🌍 বাস্তব ব্যবহার

- ডেটা ফেচ করার সময় UI রেসপন্সিভ রাখা
- ব্যাকএন্ড রিকুয়েস্ট প্রসেসিং চলাকালীন অ্যানিমেশন দেখানো
- নন-ব্লকিং ফর্ম ভ্যালিডেশন
- SPA-তে Lazy Loading

### 🧾 সংক্ষেপে

| টাইপ                     | আচরণ                            | কখন ব্যবহার করবেন                              |
| ------------------------ | ------------------------------- | ---------------------------------------------- |
| **Blocking (Sync)**      | প্রতিটি ধাপে অপেক্ষা করে        | ছোট ও দ্রুত টাস্কের জন্য ভালো                  |
| **Non-Blocking (Async)** | অপেক্ষার সময়েও থ্রেড ফাঁকা থাকে | নেটওয়ার্ক, টাইমার বা স্মুথ UI-র জন্য অপরিহার্য |

<br>

## ২১. 🧪 টেস্টযোগ্য জাভাস্ক্রিপ্ট লেখা: পিওর ফাংশন এবং সাইড ইফেক্ট

- **✅ বাগ ধরা সহজ হয়**
- **✅ ইউনিট টেস্ট সহজ হয়**
- **✅ আপনার লজিক থাকে পরিষ্কার ও স্কেলযোগ্য**

### 🧠 সহজ উদাহরণ: ল্যাব বনাম রান্নাঘর

একটা **পিওর ফাংশন** মানে কেমিস্ট্রির পরীক্ষাগার - একই উপাদান, একই ফলাফল, কোনো ঝামেলা নেই।

একটা **সাইড ইফেক্টযুক্ত ফাংশন** মানে রান্না করা - পেঁয়াজ কাটতেই চোখে জল, সস ছিটকে পড়ে, আর ফায়ার অ্যালার্ম বেজে উঠে।

যদি আপনি ক্লিন আউটপুট চান, তাহলে **লজিক রাখুন ল্যাবের ভেতর**। সাইড ইফেক্ট লাগলে আলাদা করে রাখুন।

### 📦 পিওর ফাংশন কী?

```javascript
function add(a, b) {
  return a + b;
}
```

**💡 ব্যাখ্যা:**

- ইনপুট নেয় → আউটপুট দেয়
- বাইরের ভ্যারিয়েবল, DOM বা স্টেট পরিবর্তন করে না
- কোনো চমক নেই শুধুই গাণিতিক হিসাব
- 🔍 টেস্ট করা সহজ: একই ইনপুটে সবসময় একই রেজাল্ট

### ⚡ সাইড ইফেক্ট কী?

```javascript
let count = 0;

function increment() {
  count += 1;
  console.log("Current count:", count);
}
```

**💡 ব্যাখ্যা:**

- `count` (গ্লোবাল স্টেট) পরিবর্তন করছে
- কনসোলে লগ প্রিন্ট করছে
- ⚠️ টেস্ট করা কঠিন, কারণ আউটপুট নির্ভর করে বাইরের ভ্যারিয়েবল বা স্কোপের উপর

### 🔧 উদাহরণ: টেস্টযোগ্য কোডে রিফ্যাক্টর করা

**আগে - টেস্ট করা কঠিন**

```javascript
function saveName(name) {
  localStorage.setItem("user", name); // সরাসরি সাইড ইফেক্ট
}
```

**পরে - লজিক আগে, সাইড ইফেক্ট পরে**

```javascript
function getSavePayload(name) {
  return { key: "user", value: name }; // পিওর ফাংশন
}

function saveToStorage(payload) {
  localStorage.setItem(payload.key, payload.value); // সাইড ইফেক্ট আলাদা
}
```

**💡 কেন এটা গুরুত্বপূর্ণ:**

- `getSavePayload()` প্রেডিক্টেবল ও টেস্টযোগ্য
- আপনি `saveToStorage()` মক করতে পারেন ইন্টিগ্রেশন টেস্টে
- ব্যবসায়িক লজিক আর "ঝামেলাপূর্ণ" কাজ আলাদা থাকে

### 🧪 উদাহরণ: পিওর ফাংশনের টেস্টিং

```javascript
function calculateDiscount(price, percent) {
  return price - price * (percent / 100);
}
// টেস্ট কেস
console.log(calculateDiscount(100, 20)); // ✅ সবসময় ৮০ রিটার্ন করে
```

- ✅ কোনো লগ নেই
- ✅ DOM-এ কিছু করে না
- ✅ একমাত্র ইনপুট → আউটপুট = টেস্টিংওএর জন্য ভালো

### ❌ সাধারণ ভুল

| 🚩 সমস্যা                       | 😵 কেন খারাপ              | ✅ কী করবেন                          |
| ------------------------------- | ------------------------- | ------------------------------------ |
| UI লজিক ও ব্যবসায়িক লজিক মেশানো | ইউনিট টেস্ট কঠিন করে তোলে | লজিকগুলো আলাদা হেল্পার ফাংশনে রাখুন  |
| ফাংশনের ভিতরে লগিং বা মিউটেশন   | টেস্ট রেজাল্ট গুলিয়ে ফেলে | লগ আলাদা রাখুন, লজিক ক্লিন রাখুন     |
| গ্লোবাল ভ্যারিয়েবল ব্যবহার      | আচরণ অনির্দেশ্য হয়ে পড়ে   | দরকারি সব ইনপুট প্যারামিটার দিয়ে দিন |

### 🌍 বাস্তব ব্যবহার

- ইউটিলিটি ফাংশন (হিসাব, ভ্যালিডেশন, ফরম্যাটিং)
- Redux রিডিউসার বা ফাংশনাল পাইপলাইন
- ফাইন্যান্স বা ফর্মের লজিক
- ফ্রেমওয়ার্ক কম্পোনেন্ট যেখানে লজিক ও ইফেক্ট আলাদা

### 🧾 সংক্ষেপে

| 🔹 কনসেপ্ট      | 🔎 এর মানে                                | 💡 কেন গুরুত্বপূর্ণ                                  |
| --------------- | ----------------------------------------- | ---------------------------------------------------- |
| **পিওর ফাংশন**  | কোনো সাইড ইফেক্ট নেই, প্রেডিক্টেবল আউটপুট | সহজে টেস্ট, ডিবাগ ও পুনর্ব্যবহারযোগ্য                |
| **সাইড ইফেক্ট** | ফাংশনের বাইরে কিছু পরিবর্তন (DOM, state)  | আর্কিটেকচার ক্লিন রাখতে ও টেস্ট সহজ করতে আলাদা রাখুন |
