# 📐 Lesson 3: CSS Layouts – Flexbox & Grid 🚀  

## 💡 Mission: Learn How to Create Responsive Layouts Using CSS  
**Objective:** Understand how to use **CSS Flexbox & Grid** to build **modern, responsive page layouts**.  

### 🔹 Topics Covered:  
✅ **Introduction to CSS Layouts**  
✅ **Flexbox Basics (Aligning & Spacing Elements)**  
✅ **CSS Grid Basics (Creating Grid-Based Layouts)**  
✅ **Responsive Design with Media Queries**  
✅ **Combining Flexbox & Grid for Best Results**  

---

## 📖 Part 1: Introduction to CSS Layouts  

🎯 **CSS provides multiple ways to arrange elements on a page.**  

📌 **Common Layout Techniques:**  
✅ **Floats & Inline-Block (Old methods – rarely used now)**  
✅ **Flexbox (Best for one-dimensional layouts like menus & cards)**  
✅ **CSS Grid (Best for complex, two-dimensional layouts like full web pages)**  

🔹 **Example: Old Method Using Floats (❌ Outdated)**  
```css
.container {
  width: 100%;
}

.left {
  float: left;
  width: 50%;
}

.right {
  float: right;
  width: 50%;
}
```
🎯 **Better Alternative:** Use **Flexbox** or **Grid!**  

---

## 📖 Part 2: Introduction to Flexbox  

🎯 **Flexbox makes it easy to align, distribute, and space elements inside a container.**  

🔹 **Basic Flexbox Example:**  
```css
.container {
  display: flex;
}
```

🔹 **HTML Structure:**  
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

🔹 **CSS: Basic Flexbox Layout**  
```css
.container {
  display: flex;
  justify-content: space-between;
}

.box {
  width: 100px;
  height: 100px;
  background-color: lightblue;
  text-align: center;
  line-height: 100px;
}
```

🎯 **Bonus:** Try using `justify-content: center;`  

---

## 📖 Part 3: Flexbox Properties  

### 🔹 **1. `display: flex;` (Enables Flexbox)**  
Applies **Flexbox behavior** to a container.  
```css
.container {
  display: flex;
}
```

### 🔹 **2. `justify-content` (Horizontal Alignment)**  
```css
justify-content: flex-start;   /* Default */
justify-content: center;       /* Center elements */
justify-content: space-between; /* Even spacing */
justify-content: space-around; /* Spacing with margins */
```

### 🔹 **3. `align-items` (Vertical Alignment)**  
```css
align-items: flex-start;   /* Align to the top */
align-items: center;       /* Center elements */
align-items: flex-end;     /* Align to the bottom */
```

### 🔹 **4. `flex-wrap` (Wrap Elements Instead of Squishing)**  
```css
flex-wrap: wrap; /* Allow wrapping to new lines */
```

🎯 **Bonus:** Try setting `flex-direction: column;`  

---

## 📖 Part 4: Introduction to CSS Grid  

🎯 **CSS Grid is great for building full-page layouts!**  

🔹 **Basic Grid Example:**  
```css
.container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
}
```

🔹 **HTML Structure:**  
```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

🔹 **CSS: Basic Grid Layout**  
```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}

.item {
  background-color: lightcoral;
  padding: 20px;
  text-align: center;
}
```

🎯 **Bonus:** Try using `grid-template-rows: repeat(2, 100px);`  

---

## 📖 Part 5: Grid Properties  

### 🔹 **1. `grid-template-columns` & `grid-template-rows`**  
Defines the number of columns and rows.  
```css
grid-template-columns: 200px 200px; /* Two equal columns */
grid-template-columns: 1fr 2fr 1fr; /* Flexible columns */
grid-template-rows: 100px 200px;    /* Two rows with different heights */
```

### 🔹 **2. `gap` (Spacing Between Grid Items)**  
```css
gap: 20px; /* Adds spacing between items */
```

### 🔹 **3. `grid-column` & `grid-row` (Merging Grid Items)**  
```css
grid-column: span 2; /* Makes an item take two columns */
grid-row: span 2; /* Makes an item take two rows */
```

🎯 **Bonus:** Try setting `place-items: center;`  

---

## 📖 Part 6: Responsive Design with Media Queries  

🎯 **Make layouts responsive by using media queries.**  

🔹 **Example: Changing Layout for Mobile Screens**  
```css
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

🎯 **Bonus:** Try setting different `grid-template-columns` for mobile.  

---

## 🛠️ Lab Challenge: Create a Responsive Two-Column Layout  

📌 **Task:** Build a **responsive two-column layout** using **Flexbox** or **Grid**.  

🔹 **HTML Structure:**  
```html
<div class="container">
  <div class="left">Left Column</div>
  <div class="right">Right Column</div>
</div>
```

🔹 **CSS (Flexbox Version):**  
```css
.container {
  display: flex;
  gap: 20px;
}

.left, .right {
  flex: 1;
  padding: 20px;
  background-color: lightgray;
}

/* Responsive Design */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

🎯 **Bonus:** Try the **Grid version** of the same layout!  

---

## 🎒 Homework & Next Steps  
✅ **Practice with Flexbox & Grid layouts.**  
✅ **Build a simple page layout using Flexbox.**  
✅ **Try making a full website layout using Grid.**  

📢 **Next Lesson:** **Lesson 4: Responsive Web Design & Mobile Optimization!** 📱  

---

## 🛠️ Additional Resources  

📌 **CSS Flexbox Guide (CSS-Tricks)**  
🔗 [https://css-tricks.com/snippets/css/a-guide-to-flexbox/](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)  

📌 **CSS Grid Guide (MDN Docs)**  
🔗 [https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)  

📌 **CSS Responsive Design (W3Schools)**  
🔗 [https://www.w3schools.com/css/css_rwd_intro.asp](https://www.w3schools.com/css/css_rwd_intro.asp)  

---

# 🎉 Lesson Wrap-Up  
✅ We learned **how to use Flexbox & Grid for layouts**.  
✅ We covered **alignments, spacing, and responsive design**.  
✅ We prepared for **making fully responsive websites in the next lesson**.  
