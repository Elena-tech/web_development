# 🎨 Lesson 2: CSS Basics – Styling Your Website 🚀  

## 💡 Mission: Learn How to Style Web Pages Using CSS  
**Objective:** Understand how to apply **CSS rules** to style text, backgrounds, layouts, and more.  

### 🔹 Topics Covered:  
✅ **What is CSS?** (How it works & why we use it)  
✅ **CSS Selectors & Properties**  
✅ **Colors, Fonts, and Text Styling**  
✅ **Box Model (Padding, Borders, Margins)**  
✅ **Adding CSS to an HTML Page**  

---

## 📖 Part 1: What is CSS?  

🎯 **CSS (Cascading Style Sheets) is used to style HTML elements.**  
📌 **CSS allows you to:**  
- Change **colors, fonts, sizes**  
- Modify **spacing (margin, padding, borders)**  
- Control **layouts & positioning**  

🔹 **Example: Changing Text Color & Size**  
```css
h1 {
  color: blue;
  font-size: 32px;
}
```

---

## 📖 Part 2: How to Add CSS to an HTML Page  

### 🔹 **1. Inline CSS (Inside an HTML Tag – Not Recommended)**  
```html
<p style="color: red;">This is a red paragraph.</p>
```

### 🔹 **2. Internal CSS (Inside `<style>` in `<head>`)**  
```html
<head>
  <style>
    p {
      color: green;
    }
  </style>
</head>
```

### 🔹 **3. External CSS (Best Practice – Linking a CSS File)**  
🔹 **Create a separate file** called `styles.css`  
```css
p {
  color: purple;
}
```
🔹 **Link the file in HTML**  
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

🎯 **Bonus:** Try using **all three methods** and see which one is best!  

---

## 📖 Part 3: CSS Selectors & Properties  

🔹 **CSS applies styles using selectors:**  
```css
/* Selects all `<p>` elements */
p {
  color: blue;
}
```

### 🔹 **Types of CSS Selectors**  

#### ✅ **Element Selector (Targets HTML Tags)**  
```css
h1 {
  color: orange;
}
```

#### ✅ **Class Selector (Used for Multiple Elements)**  
```css
.highlight {
  background-color: yellow;
}
```
```html
<p class="highlight">This text is highlighted.</p>
```

#### ✅ **ID Selector (Used for a Single Element)**  
```css
#main-title {
  font-size: 36px;
  color: darkred;
}
```
```html
<h1 id="main-title">Welcome to My Website</h1>
```

#### ✅ **Group Selector (Apply Styles to Multiple Elements at Once)**  
```css
h1, h2, h3 {
  font-family: Arial, sans-serif;
}
```

🎯 **Bonus:** Create a class for **buttons** and style them!  

---

## 📖 Part 4: Colors, Fonts & Backgrounds  

### 🔹 **CSS Colors (Using Names, Hex, RGB, HSL)**  
```css
p {
  color: rgb(255, 0, 0); /* Red */
  background-color: #f4f4f4; /* Light gray */
}
```

### 🔹 **Changing Fonts & Text Size**  
```css
body {
  font-family: 'Arial', sans-serif;
  font-size: 18px;
  text-align: center;
}
```

🎯 **Bonus:** Try using **Google Fonts** in your CSS!  

---

## 📖 Part 5: The CSS Box Model  

🎯 **Every HTML element is a box!**  
📌 **The Box Model consists of:**  
- **Content** (The actual text or image inside)  
- **Padding** (Space inside the border)  
- **Border** (Outline around the element)  
- **Margin** (Space outside the element)  

🔹 **Example:**  
```css
.box {
  width: 200px;
  height: 100px;
  padding: 20px;
  margin: 10px;
  border: 2px solid black;
}
```

🔹 **Visual Representation:**  
```
┌────────── Margin ──────────┐
│  ┌────── Border ──────┐   │
│  │  ┌── Padding ──┐  │   │
│  │  │ Content     │  │   │
│  │  └─────────────┘  │   │
│  └───────────────────┘   │
└──────────────────────────┘
```

🎯 **Bonus:** Try changing the **border styles (`dashed`, `dotted`, `solid`)**!  

---

## 📖 Part 6: Adding Backgrounds & Shadows  

🔹 **Background Image & Color**  
```css
body {
  background-color: lightblue;
  background-image: url('background.jpg');
  background-size: cover;
}
```

🔹 **Adding Box Shadows**  
```css
.card {
  box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.2);
}
```

🎯 **Bonus:** Try creating a **gradient background** using `background: linear-gradient()`!  

---

## 🛠️ Lab Challenge: Create a Styled Web Page  

📌 **Task:** Build a **styled web page** using **CSS rules** you learned.  

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Styled Page</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1 class="title">Welcome to My Website</h1>
  <p>This is a paragraph with some styles.</p>
  <button class="btn">Click Me</button>
</body>
</html>
```

🔹 **CSS (`styles.css`)**
```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: navy;
  text-align: center;
}

.btn {
  background-color: blue;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}
```

🎯 **Bonus:** Make the button **change color when hovered**!  

---

## 🎒 Homework & Next Steps  
✅ **Style a full webpage with fonts, colors, and backgrounds.**  
✅ **Experiment with different box models, borders, and paddings.**  
✅ **Try using Google Fonts and custom background images.**  

📢 **Next Lesson:** **Lesson 3: CSS Layouts – Flexbox & Grid!** 🚀  

---

## 🛠️ Additional Resources  

📌 **CSS Basics (MDN Docs)**  
🔗 [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)  

📌 **CSS Box Model Explained**  
🔗 [https://www.w3schools.com/css/css_boxmodel.asp](https://www.w3schools.com/css/css_boxmodel.asp)  

📌 **CSS Flexbox & Grid Layouts**  
🔗 [https://css-tricks.com/snippets/css/a-guide-to-flexbox/](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)  

---

# 🎉 Lesson Wrap-Up  
✅ We learned **how to apply CSS styles to HTML**.  
✅ We covered **colors, fonts, backgrounds, and box models**.  
✅ We prepared for **CSS Layouts (Flexbox & Grid) in the next lesson**.  
