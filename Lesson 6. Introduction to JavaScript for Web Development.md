# 🛠️ Lesson 6: Introduction to JavaScript for Web Development 🚀  

## 💡 Mission: Learn How JavaScript Makes Web Pages Interactive  
**Objective:** Understand JavaScript fundamentals, how it interacts with HTML & CSS, and how to add dynamic functionality to web pages.  

### 🔹 Topics Covered:  
✅ **What is JavaScript & Why Use It?**  
✅ **Variables & Data Types**  
✅ **Functions & Events**  
✅ **Manipulating the DOM (Updating Web Page Content Dynamically)**  
✅ **Handling User Input & Basic Form Validation**  

---

## 📖 Part 1: What is JavaScript?  

🎯 **JavaScript is a programming language that adds interactivity to websites.**  

📌 **What Can JavaScript Do?**  
✅ Change **text, colors, and styles dynamically**  
✅ Respond to **user actions (clicks, key presses, scrolls, form submissions)**  
✅ Fetch data from **APIs** and update the page without reloading  

🔹 **Example: Changing Text Using JavaScript**  
```html
<p id="text">Hello, world!</p>
<button onclick="changeText()">Click Me</button>

<script>
  function changeText() {
    document.getElementById("text").innerText = "JavaScript is awesome!";
  }
</script>
```

🎯 **Bonus:** Try using `console.log("Hello, JavaScript!")` in the browser console!  

---

## 📖 Part 2: JavaScript Basics (Variables & Data Types)  

🎯 **JavaScript uses variables to store data.**  

🔹 **Declaring Variables in JavaScript**  
```js
let name = "Alice";  // String
const age = 25;  // Number
let isStudent = true;  // Boolean
```

🔹 **Using Variables**  
```js
console.log(`My name is ${name} and I am ${age} years old.`);
```

🎯 **Bonus:** Try declaring variables using `var` and `const`!  

---

## 📖 Part 3: Functions & Event Listeners  

🎯 **Functions let you write reusable blocks of code.**  

🔹 **Basic Function Example**  
```js
function greet() {
  console.log("Hello, world!");
}

greet(); // Calls the function
```

🔹 **Handling Button Clicks**  
```html
<button id="myButton">Click Me</button>

<script>
  document.getElementById("myButton").addEventListener("click", function() {
    alert("Button clicked!");
  });
</script>
```

🎯 **Bonus:** Try using `prompt()` to get user input and `alert()` to display it!  

---

## 📖 Part 4: Changing HTML & CSS with JavaScript  

🎯 **JavaScript can modify HTML elements and CSS styles dynamically.**  

🔹 **Changing Text Content**  
```html
<p id="message">Hello!</p>
<button onclick="changeMessage()">Change Text</button>

<script>
  function changeMessage() {
    document.getElementById("message").innerText = "JavaScript is fun!";
  }
</script>
```

🔹 **Changing CSS Styles**  
```html
<p id="styledText">This text will change color.</p>
<button onclick="changeColor()">Change Color</button>

<script>
  function changeColor() {
    document.getElementById("styledText").style.color = "red";
  }
</script>
```

🎯 **Bonus:** Add a button that changes the **background color**!  

---

## 📖 Part 5: Handling User Input  

🎯 **JavaScript allows real-time user interaction.**  

🔹 **Reading User Input & Displaying It**  
```html
<input type="text" id="username" placeholder="Enter your name">
<button onclick="displayUsername()">Submit</button>
<p id="output"></p>

<script>
  function displayUsername() {
    let username = document.getElementById("username").value;
    document.getElementById("output").innerText = `Hello, ${username}!`;
  }
</script>
```

🎯 **Bonus:** Clear the input field after submission!  

---

## 📖 Part 6: Form Validation with JavaScript  

🎯 **Validate forms before submission to prevent errors.**  

🔹 **Example: Check if Fields are Empty**  
```html
<form id="loginForm">
  <input type="text" id="username" placeholder="Username">
  <input type="password" id="password" placeholder="Password">
  <button type="submit">Login</button>
  <p id="error-message" style="color: red;"></p>
</form>

<script>
  document.getElementById("loginForm").addEventListener("submit", function(event) {
    event.preventDefault();
    
    let username = document.getElementById("username").value;
    let password = document.getElementById("password").value;
    let errorMessage = document.getElementById("error-message");

    if (username === "" || password === "") {
      errorMessage.innerText = "All fields are required!";
    } else {
      errorMessage.innerText = "";
      alert("Login successful!");
    }
  });
</script>
```

🎯 **Bonus:** Add password length validation!  

---

## 🛠️ Lab Challenge: Build an Interactive To-Do List  

📌 **Task:** Create a **To-Do List** where users can **add, mark as complete, and remove tasks**.  

🔹 **Example HTML**  
```html
<input type="text" id="taskInput" placeholder="New Task">
<button onclick="addTask()">Add Task</button>
<ul id="taskList"></ul>
```

🔹 **JavaScript for To-Do List**  
```js
function addTask() {
  let taskInput = document.getElementById("taskInput");
  let taskList = document.getElementById("taskList");

  if (taskInput.value !== "") {
    let li = document.createElement("li");
    li.innerText = taskInput.value;

    let completeButton = document.createElement("button");
    completeButton.innerText = "✔";
    completeButton.addEventListener("click", function() {
      li.style.textDecoration = "line-through";
    });

    let removeButton = document.createElement("button");
    removeButton.innerText = "❌";
    removeButton.addEventListener("click", function() {
      taskList.removeChild(li);
    });

    li.appendChild(completeButton);
    li.appendChild(removeButton);
    taskList.appendChild(li);
    taskInput.value = "";
  }
}
```

🎯 **Bonus:** Store tasks in **localStorage** so they persist after page reload!  

---

## 🎒 Homework & Next Steps  
✅ **Create a webpage that responds to button clicks and user input.**  
✅ **Modify the To-Do List to allow editing tasks.**  
✅ **Try using `localStorage` to save data between page reloads.**  

📢 **Next Lesson:** **Lesson 7: CSS Animations & Transitions!** 🎨🚀  

---

## 🛠️ Additional Resources  

📌 **JavaScript Basics (MDN Docs)**  
🔗 [https://developer.mozilla.org/en-US/docs/Web/JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)  

📌 **JavaScript DOM Manipulation (MDN Docs)**  
🔗 [https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)  

📌 **Form Validation in JavaScript**  
🔗 [https://www.w3schools.com/js/js_validation.asp](https://www.w3schools.com/js/js_validation.asp)  

---

# 🎉 Lesson Wrap-Up  
✅ We learned **JavaScript fundamentals (variables, functions, events).**  
✅ We explored **DOM manipulation (updating HTML & CSS dynamically).**  
✅ We built an **interactive To-Do List using JavaScript!**  
