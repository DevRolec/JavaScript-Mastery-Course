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



