# 🌍 Lesson 0: Introduction to the Web & Basic HTML 🚀  

## 💡 Mission: Understand How the Web Works & Create Your First HTML Page!  
**Objective:** Learn how **web pages work**, what **HTML is**, and how to create a **basic web page**.  

### 🔹 Topics Covered:  
✅ **What is the Web?** (How Browsers & Servers Work)  
✅ **What is HTML?** (The Language of the Web)  
✅ **Basic HTML Tags (`<h1>`, `<p>`, `<img>`, `<a>`)**  
✅ **Structuring a Simple Web Page (`<header>`, `<main>`, `<footer>`)**  

---

## 📖 Part 1: What is the Web & How Does it Work?  

### 🎯 **How Websites Work**  
When you visit a website, your browser (Chrome, Firefox, Edge) **sends a request** to a **web server**. The server **sends back an HTML file**, which the browser **displays as a web page**.  

🔹 **Key Components:**  
- **Web Browser** – A program that displays web pages (Chrome, Firefox, Safari)  
- **Web Server** – A computer that stores and delivers websites  
- **HTML (HyperText Markup Language)** – The structure of web pages  
- **CSS (Cascading Style Sheets)** – The styling of web pages  
- **JavaScript** – Adds interactivity to web pages  

---

## 🛠️ Lab Challenge 1: Creating Your First Web Page  

📌 **Task:** Create a basic HTML page and open it in a browser.  

#### 🔹 Step 1: Create an HTML File  
📁 **File Name:** `index.html`  

#### 🔹 Step 2: Add Basic HTML Structure  
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My First Web Page</title>
</head>
<body>
  <h1>Welcome to My Website</h1>
  <p>Hello! This is my first web page.</p>
</body>
</html>
```

#### 🔹 Step 3: Open in a Web Browser  
1️⃣ Save the file as `index.html`  
2️⃣ Open it in **Chrome, Firefox, or Edge**  

🎯 **Bonus:** Change the **text in `<title>`** and **refresh the page**!  

---

## 📖 Part 2: Basic HTML Tags  

### 🔹 **Headings (`<h1>` to `<h6>`)**  
Used to define titles and subheadings.  
```html
<h1>Main Title</h1>
<h2>Subheading</h2>
<h3>Smaller Heading</h3>
```

### 🔹 **Paragraphs (`<p>`)**  
Used for regular text.  
```html
<p>This is a paragraph of text.</p>
```

### 🔹 **Links (`<a>`)**  
Used to **navigate between web pages**.  
```html
<a href="https://www.google.com">Visit Google</a>
```

🎯 **Bonus:** Open links in a **new tab** using `target="_blank"`!  
```html
<a href="https://www.google.com" target="_blank">Visit Google</a>
```

---

## 🛠️ Lab Challenge 2: Adding Text & Links  

📌 **Task:** Add headings, paragraphs, and a clickable link to your web page.  

#### 🔹 Updated HTML File  
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>About Me</title>
</head>
<body>
  <h1>About Me</h1>
  <p>Hi! My name is Alex. I love learning web development.</p>
  <p>Check out my favorite website:</p>
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank">MDN Web Docs</a>
</body>
</html>
```

🎯 **Bonus:** Add an **`<h2>` subheading** under `<h1>`!  

---

## 📖 Part 3: Adding Images & Lists  

### 🔹 **Images (`<img>`)**  
Used to **display pictures** on a webpage.  
```html
<img src="image.jpg" alt="A description of the image">
```

🎯 **Bonus:** Use an **online image URL** instead of `image.jpg`!  
```html
<img src="https://www.example.com/photo.jpg" alt="Example image">
```

### 🔹 **Lists (`<ul>` & `<ol>`)**  
Used to create **bullet points or numbered lists**.  

#### **Unordered List (`<ul>`) – Bullets**  
```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

#### **Ordered List (`<ol>`) – Numbers**  
```html
<ol>
  <li>Step 1: Learn HTML</li>
  <li>Step 2: Learn CSS</li>
  <li>Step 3: Learn JavaScript</li>
</ol>
```

---

## 🛠️ Lab Challenge 3: Adding Images & Lists  

📌 **Task:** Add an image and a list of your **favorite hobbies**.  

#### 🔹 Updated HTML File  
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Hobbies</title>
</head>
<body>
  <h1>My Hobbies</h1>
  <img src="https://www.example.com/myphoto.jpg" alt="Me enjoying my hobby">
  <h2>Things I Love Doing:</h2>
  <ul>
    <li>Playing video games</li>
    <li>Reading books</li>
    <li>Traveling</li>
  </ul>
</body>
</html>
```

🎯 **Bonus:** Add a **`<p>` caption below the image**!  

---

## 🎒 Homework & Next Steps  
✅ **Complete all Lab Challenges (Headings, Links, Lists, and Images).**  
✅ **Change colors & styles using basic CSS (next lesson).**  
✅ **Validate your HTML using [W3C Validator](https://validator.w3.org/).**  

📢 **Next Lesson:** **Lesson 1: HTML Forms & Accessibility – Creating User Input Fields** 🚀  

---

## 🛠️ Additional Resources  

📌 **HTML Basics (MDN Docs)**  
🔗 [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)  

📌 **HTML Tags Reference (W3Schools)**  
🔗 [https://www.w3schools.com/tags/](https://www.w3schools.com/tags/)  

📌 **HTML Validator – Check Your Code**  
🔗 [https://validator.w3.org/](https://validator.w3.org/)  

---

# 🎉 Lesson Wrap-Up  
✅ We created a **basic web page using HTML**.  
✅ We added **headings, paragraphs, links, images, and lists**.  
✅ We prepared for **styling with CSS in future lessons**.  
