# 🚀 JavaScript Mastery Course
Welcome to the JavaScript Mastery Course – a hands-on learning experience designed for anyone looking to build a solid foundation in JavaScript and grow into a confident frontend or full-stack developer.

This course takes you from the basics of JavaScript to advanced topics through real-world examples, coding challenges, mini-projects, and guided assignments. Whether you're a beginner or brushing up your skills, you'll find this repo packed with practical lessons and resources to sharpen your JavaScript knowledge.

## 💡 What You’ll Learn
JavaScript Fundamentals: Variables, data types, functions, loops, and conditionals

DOM Manipulation and Events

ES6+ Features (let/const, arrow functions, destructuring, spread/rest, etc.)

Asynchronous JavaScript: Callbacks, Promises, async/await

Working with APIs and Fetch

Local Storage and Browser APIs

Modular JavaScript and Code Organization

Building Projects: To-Do App, Quiz Game, Weather App, etc.

## 📁 Structure
lessons/: Step-by-step JavaScript tutorials

projects/: Real-world mini-projects to practice skills

quizzes/: Topic-based questions and practice exercises

assignments/: Coding tasks and challenges

resources/: Helpful links, documentation, and references

## 🧠 Who This Is For
-Beginners looking to start their JavaScript journey

-Self-taught developers aiming to strengthen their core JS skills

-Frontend learners preparing for frameworks like React or Vue

-Anyone who prefers project-based learning

## ✅ How to Use
1. Clone the repository

2. Start with the lessons/ folder and go through the topics in order

3. After every few lessons, try building the project in the projects/ folder

4. Test your understanding with quizzes and assignments

5. Submit pull requests if you'd like to contribute!

# 🎓 JavaScript Mastery Course (Beginner → Advanced)
## 📦 Module 1: Getting Started with JavaScript (Beginner)

Goal: Understand what JavaScript is, how to run it, and learn the basics.

✅ Topics:
What is JavaScript? (History, Use Cases)

Setting up the environment (Browser, Node.js, VS Code)

Writing your first script (console.log, linking JS to HTML)

Variables: var, let, const

Data types: string, number, boolean, null, undefined

Operators: arithmetic, assignment, comparison, logical

Comments & code structure

🧠 Example:
```js
Copy
Edit
let name = "Sam";
console.log("Hello, " + name);
```
🛠️ Practice Project:
Greeting Card Generator: Ask for user input (prompt), show a custom message on the screen.
---
```js
//MOST PRACTICES IN JS
//1. Control Flow and Functions
//2. Arrays
//3. Objects
//4. DOM
//5. Events
//6. Local Storage
//7. Fetch
//8. Async/Await
//9. Regular Expressions
//10. JSON
//11. Error Handling
```
### 🔹 What is Control Flow?
Control Flow is the order in which individual statements, 
instructions, or function calls are executed or evaluated in a program.

By default, JavaScript executes code from top to bottom, 
left to right, but you can alter the flow using control structures like:

Conditionals (if, else, switch)

Loops (for, while, do...while)

Function calls (function())
## 🧩 Module 2: Control Flow & Functions

✅ Topics:
Conditionals: if, else, switch

Loops: for, while, do while

Functions: declarations, expressions, arrow functions, parameters, return

🧠 Example:
```js
Copy
Edit
function greet(name) {
  return `Hello, ${name}`;
}
console.log(greet("Ada"));
```
---
🛠️ Practice Project:
Guess the Number Game: Random number guessing with limited attempts.
---
## 📦 Module 3: Arrays and Objects

✅ Topics:
Arrays: creation, indexing, push, pop, map, filter, reduce

Objects: properties, methods, nesting

Looping through arrays/objects

🧠 Example:
```js
Copy
Edit
const user = {
  name: "John",
  age: 30,
  greet() {
    console.log(`Hi, I'm ${this.name}`);
  }
};
user.greet();
```
🛠️ Practice Project:
To-Do List App: Add/remove tasks, store tasks in an array.
---
🧠 Module 4: DOM Manipulation (Browser Focus)

✅ Topics:
document.querySelector, getElementById

Changing text, HTML, styles

Event listeners (click, input, submit)

Form handling

🧠 Example:
```js
Copy
Edit
document.querySelector("button").addEventListener("click", () => {
  alert("Button clicked!");
});
```
## 📘 JavaScript Arrays – Full Lesson
🔹 What is an Array?
An array is a special variable that can hold multiple values at once
```js
let fruits = ["apple", "banana", "orange"];
```
Here, fruits is an array that holds three string values.

🔹 Why Use Arrays?
To store lists of items.

To group related data.

To iterate through items using loops.

To efficiently perform operations like add, remove, filter, and sort items.
### 🔹 Creating Arrays
```js
let emptyArray = []; // empty array

let numbers = [10, 20, 30, 40];

let mixed = ["hello", 42, true, null];
```
You can also use the Array constructor:
```js
let scores = new Array(100, 200, 300);
```
An array can contain objects like this
```js
const people = [
    {name: "Sochima", age: 22},
    {name: "Uzoma", age: 22},
    {name: "Roland", age: 75}
]
```
✅ Accessing Objects in the Array
1. Access the whole object by index:
```js
console.log(people[0]); 
// Output: { name: "Sochima", age: 25 }
```
2. Access a property of an object:
```js
console.log(people[1].name); 
// Output: Uzoma
console.log(people[2].age); 
// Output: 75
```
### 🔁 Loop Through Objects in an Array
You can use loops like for, for...of, or forEach.

Example using forEach:
```js
people.forEach(person => {
  console.log(person.name + " is " + person.age + " years old.");
});
```
🔎 Find an Object by a Property
Use .find() to get the first object matching a condition:
```js
const result = people.find(person => person.name === "Charlie");
console.log(result);
// Output: { name: "Charlie", age: 35 }
```
### 🔁 Filter Multiple Matches
```js
const adults = people.filter(person => person.age >= 30);
console.log(adults);
// Output: [ { name: 'Bob', age: 30 }, { name: 'Charlie', age: 35 } ]
```
🔸 Note: Using square brackets [] is preferred for simplicity and readability.

🔹 Accessing Elements
Use indexing (starting from 0):

```js
let cars = ["Toyota", "BMW", "Tesla"];
console.log(cars[0]); // Toyota
console.log(cars[2]); // Tesla
```
🔹 Changing Values
```js
cars[1] = "Mercedes";
console.log(cars); // ["Toyota", "Mercedes", "Tesla"]
```
🔹 Array Properties
length
Gives the number of elements in the array:
```js
let animals = ["dog", "cat", "rabbit"];
console.log(animals.length); // 3
```
🔹 Array Methods
1. ✅ Adding and Removing
Method	Description
- push()	Add to end
- pop()	Remove from end
- unshift()	Add to start
- shift()	Remove from start

```js
let items = ["pen", "pencil"];
items.push("eraser");      // ["pen", "pencil", "eraser"]
items.pop();               // ["pen", "pencil"]
items.unshift("sharpener"); // ["sharpener", "pen", "pencil"]
items.shift();             // ["pen", "pencil"]
```
2. 🔄 Iterating Arrays
for loop
```js
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```
for...of loop
```js
for (let fruit of fruits) {
  console.log(fruit);
}
forEach()
```
```js
fruits.forEach(function(fruit) {
  console.log(fruit);
});
```
3. 🔍 Searching in Arrays
```js
let nums = [1, 2, 3, 4, 5];

console.log(nums.includes(3)); // true
console.log(nums.indexOf(4)); // 3
```
4. 🔧 Other Useful Methods
Method	Description
- join()	Converts to string with separator
- slice()	Extracts part of the array
- splice()	Adds/removes items at specific index
- concat()	Combines arrays
- reverse()	Reverses the array
- sort()	Sorts elements (lexicographically)
- map()	Returns a new array by applying a function
- filter()	Returns a new array with matching items

🧪 Examples
Example 1: Join
```js
let colors = ["red", "blue", "green"];
console.log(colors.join(", ")); // "red, blue, green"
```
Example 2: Slice
```js
let sliced = colors.slice(0, 2); // ["red", "blue"]
```
Example 3: Splice
```js
colors.splice(1, 1, "yellow"); // removes 1 item at index 1, adds "yellow"
console.log(colors); // ["red", "yellow", "green"]
```
💡 Practice Exercises
1. Create an array of 5 student names and print each one using a for...of loop.
2. Create a number array [10, 20, 30, 40, 50]:
Add 60 to the end.

Remove the first element.

Print the new array.

3. Create an array of prices [100, 200, 300], then use map() to return a new array with a 10% discount applied.
4. Filter out numbers greater than 25 from [10, 25, 30, 5, 40].
## 🧠 Mini Quiz
What does array.length return?

What's the difference between push() and unshift()?

How do you remove the second item in an array?

🎯 Challenge Task
Build a program that:

Asks a user to enter 5 favorite foods using prompt().

Stores them in an array.

Sorts them alphabetically.

Prints the sorted list using alert() or console.log().
---
## 📘 JavaScript Objects – Full Lesson
🔹 What is an Object?
In JavaScript, an object is a data structure that lets you store key-value pairs.

```
let person = {
  name: "Alice",
  age: 25,
  isStudent: true
};
name, age, and isStudent are keys (also called properties).

"Alice", 25, and true are their values.
```
🔹 Why Use Objects?
To group related data together.

To model real-world things (like a user, product, car).

To allow flexible data access using property names.

To store functions (methods) inside data.

🔹 Creating Objects
Method 1: Object Literal (most common)
```js
let car = {
  brand: "Toyota",
  model: "Corolla",
  year: 2020
};
```
Method 2: Using new Object()
```js
let user = new Object();
user.name = "John";
user.age = 30;
```
🔹 Accessing Object Properties
Dot Notation
```js
console.log(car.brand); // "Toyota"
```
Bracket Notation
```js
console.log(car["model"]); // "Corolla"
```
Use bracket notation when the property name is dynamic or has special characters.

🔹 Updating and Adding Properties
```js
car.year = 2021;           // Update
car.color = "blue";        // Add new
```
🔹 Deleting Properties
```js
delete car.color;
```
🔹 Nested Objects
```js
let student = {
  name: "Lucy",
  grades: {
    math: 90,
    science: 85
  }
};

console.log(student.grades.math); // 90
```
🔹 Objects with Methods
You can store functions in objects:

```js
let user = {
  name: "Mike",
  greet: function () {
    console.log("Hi, I'm " + this.name);
  }
};

user.greet(); // Hi, I'm Mike
```
Use this to refer to the object itself.

🔹 Looping Through an Object
for...in loop
```js
for (let key in car) {
  console.log(key + ": " + car[key]);
}
```
🔹 Object Built-in Methods
Method	Description
Object.keys()	Returns an array of keys
Object.values()	Returns an array of values
Object.entries()	Returns an array of key-value pairs
hasOwnProperty()	Checks if key exists directly on object

```js
let keys = Object.keys(car);     // ["brand", "model", "year"]
let values = Object.values(car); // ["Toyota", "Corolla", 2020]
```
🔹 Object Destructuring
```js
let { brand, model } = car;
console.log(brand); // "Toyota"
```
🔹 Object.freeze() vs Object.seal()
Method	Can Modify Values?	Can Add/Delete?
freeze()	❌ No	❌ No
seal()	✅ Yes	❌ No
```js
Object.freeze(car);
car.brand = "Honda"; // Won't change
```
🧪 Examples
Example 1: Create and Display a Book Object
```js
let book = {
  title: "JS Basics",
  author: "Jane Doe",
  pages: 200
};

console.log(`Book: ${book.title} by ${book.author}`);
```
Example 2: Check if Key Exists
```js
console.log("model" in car); // true
```
🧠 Practice Exercises
1. Create an object movie with keys: title, director, year, and rating.
2. Add a method describe that prints movie info.
3. Loop through the object and print each key and value.
4. Create a nested object profile with keys like name, age, and contact (which itself has email, phone).
🎯 Challenge Task
Create a program that:

Stores a list of users as an array of objects.

Each user object has name, email, and loginCount.

Write a function to:

Add a new user.

Print all user names.

Find user by email.

```js
let users = [];

function addUser(name, email) {
  users.push({ name, email, loginCount: 0 });
}
```
📘 JavaScript DOM (Document Object Model) Lesson
✅ What is the DOM?
DOM stands for Document Object Model.

It is a programming interface for HTML and XML documents.

The DOM represents the document as a tree structure where each node is an object representing a part of the page (elements, attributes, text).

🧱 DOM Tree Example:
```html
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is a paragraph.</p>
  </body>
</html>
```
This is converted into a tree-like structure in JavaScript.

📌 Accessing the DOM
You can use the document object in JS to access and manipulate HTML.
```js
console.log(document.title);   // Shows the title of the page
console.log(document.body);    // Access the body element
```
📍 Selecting Elements
1. getElementById()
```html
<p id="demo">Hello</p>

<script>
  const el = document.getElementById("demo");
  console.log(el.textContent); // Output: Hello
</script>
```
2. getElementsByClassName()
```html
<p class="text">One</p>
<p class="text">Two</p>

<script>
  const texts = document.getElementsByClassName("text");
  console.log(texts[0].textContent); // Output: One
</script>
```
3. getElementsByTagName()
```js
const allParas = document.getElementsByTagName("p");
```
4. querySelector() and querySelectorAll()
```html
<div class="box">Hello</div>
<script>
  const el = document.querySelector(".box"); // First .box
</script>
```
```js
const allBoxes = document.querySelectorAll(".box"); // All .box
```
✏️ Modifying Content
1. innerHTML – Change HTML inside an element
```js
document.getElementById("demo").innerHTML = "<b>New Text</b>";
```
2. textContent – Change only the text
```js
document.getElementById("demo").textContent = "Just text";
```
🎨 Changing Styles with JavaScript
```js
const btn = document.getElementById("myBtn");
btn.style.color = "white";
btn.style.backgroundColor = "blue";
```
🎮 Adding Events
1. Using onclick
```html
<button onclick="alert('Clicked!')">Click Me</button>
```
2. Using addEventListener
```js
const btn = document.querySelector("#myBtn");
btn.addEventListener("click", function () {
  alert("Clicked!");
});
```
🛠️ Creating and Appending Elements
```js
const newDiv = document.createElement("div");
newDiv.textContent = "I am new!";
document.body.appendChild(newDiv);
```
❌ Removing Elements
```js
const el = document.getElementById("removeMe");
el.remove(); // Removes the element
```
### 🔄 DOM Practice Examples
🧪 Practice 1: Change Text on Button Click
```html
<p id="text">Hello</p>
<button onclick="changeText()">Click Me</button>

<script>
  function changeText() {
    document.getElementById("text").textContent = "You clicked me!";
  }
</script>
```
🧪 Practice 2: Toggle Background Color
```html
<button id="toggleBtn">Toggle</button>

<script>
  const btn = document.getElementById("toggleBtn");

  btn.addEventListener("click", function () {
    document.body.style.backgroundColor =
      document.body.style.backgroundColor === "yellow" ? "white" : "yellow";
  });
</script>
```
🧪 Practice 3: Add Items to a List
```html
<ul id="list"></ul>
<button onclick="addItem()">Add Item</button>

<script>
  function addItem() {
    const li = document.createElement("li");
    li.textContent = "New Item";
    document.getElementById("list").appendChild(li);
  }
</script>
```
### ✅ DOM Practice Assignments
Create a form with name and age inputs. On clicking a button, show a greeting: “Hello [name], you are [age] years old.”

Make a counter that increases or decreases on button click.

Create a light switch: A button that toggles between black and white background and updates its label (ON/OFF).

Build a Todo List:

Add input and a button

Add each new input to a list below

Make each item removable
---
🧠 Summary
Task	Method
Select by ID	getElementById()
Select by class	getElementsByClassName()
Select one or many	querySelector() / querySelectorAll()
Change content	innerHTML, textContent
Change style	.style.property
Listen to events	.addEventListener()
Create element	document.createElement()
Append element	parent.appendChild()
Remove element	.remove()
---
🛠️ Practice Project:
Interactive Quiz App: Show questions, capture answers, show score.
---
## 🌐 Module 5: Advanced Functions & Scope

✅ Topics:
Scope (global, block, function)

Closures

Higher-order functions

Callback functions

🧠 Example:
```js
Copy
Edit
function multiplier(factor) {
  return function(x) {
    return x * factor;
  };
}
const double = multiplier(2);
console.log(double(5)); // 10
```

🛠️ Practice Project:
Tip Calculator App: Calculates tip based on amount and service quality.
---
⏳ Module 6: Asynchronous JavaScript
Duration: 2 weeks

✅ Topics:
Synchronous vs asynchronous

Callbacks → Promises → async/await

fetch API, JSON parsing

Error handling with try...catch

🧠 Example:
```js
Copy
Edit
async function getData() {
  const res = await fetch("https://jsonplaceholder.typicode.com/posts");
  const data = await res.json();
  console.log(data);
}
getData();
```
🛠️ Practice Project:
Weather App: Fetch weather info using an API and display it.
---
## 🧱 Module 7: Object-Oriented Programming (OOP)

✅ Topics:
Constructor functions and prototypes

ES6 classes, inheritance

Encapsulation and method overriding

🧠 Example:
```js
Copy
Edit
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}
```
🛠️ Practice Project:
Library Book Tracker: Add books, mark as read/unread using classes.
---
## 🔁 Module 8: The Event Loop and Performance
✅ Topics:
Event loop, call stack, task queue

setTimeout, setInterval

Memory leaks and garbage collection

Performance tips

🧠 Example:
```js
Copy
Edit
console.log("Start");
setTimeout(() => console.log("Timeout"), 0);
console.log("End");
```
🛠️ Practice Project:
Typing Speed Test App: Timed app that calculates typing speed and shows result.
---
## 🔌 Module 9: Modules and Tooling

✅ Topics:
ES6 import/export

Webpack, Babel (intro)

Linting with ESLint

NPM and dependency management

🧠 Example:
```js
Copy
Edit
// greet.js
export function greet(name) {
  return `Hello, ${name}`;
}
```
## 🧪 Module 10: Testing and Debugging

✅ Topics:
Debugging with browser dev tools

Writing unit tests using Jest

Console tips: console.table, console.group

---
🧠 Final Capstone Projects
Build one or more of the following using all you've learned:

Issue Tracker App (like GitHub Issues)

Movie Search App with API

Personal Expense Tracker

Mini Kanban Board (Trello-style)



