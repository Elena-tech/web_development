# 📝 Lesson 1: HTML Forms & Web Components 🚀  

## 💡 Mission: Learn How to Collect & Process User Input  
**Objective:** Understand how to **create forms, capture user input, and build reusable web components** in HTML.  

### 🔹 Topics Covered:  
✅ **What are Forms?** (Capturing User Input)  
✅ **Basic Form Elements (`<input>`, `<textarea>`, `<select>`)**  
✅ **Form Buttons & Submission**  
✅ **Customizing Forms with CSS**  
✅ **Introduction to Web Components**  

---

## 📖 Part 1: What are HTML Forms?  

🎯 **Forms allow users to enter and submit data on websites.**  
📌 **Common Uses of Forms:**  
- Sign-up pages & login screens  
- Contact forms  
- Search bars  
- Checkout & payment pages  

🔹 **Basic Structure of a Form:**  
```html
<form action="submit.php" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <button type="submit">Submit</button>
</form>
```

🎯 **Bonus:** Change the method to `"GET"` and see the difference!  

---

## 📖 Part 2: HTML Form Elements  

### 🔹 **Text Input Fields (`<input type="text">`)**  
Used for **single-line text input**.  
```html
<label for="username">Username:</label>
<input type="text" id="username" name="username">
```

### 🔹 **Email & Password Fields**  
```html
<label for="email">Email:</label>
<input type="email" id="email" name="email">

<label for="password">Password:</label>
<input type="password" id="password" name="password">
```

### 🔹 **Textarea (Multi-line Input)**  
Used for **long text input** (e.g., comments, descriptions).  
```html
<label for="message">Your Message:</label>
<textarea id="message" name="message" rows="4"></textarea>
```

### 🔹 **Dropdown Select Menu (`<select>`)**  
```html
<label for="country">Choose a Country:</label>
<select id="country" name="country">
  <option value="us">United States</option>
  <option value="uk">United Kingdom</option>
  <option value="jp">Japan</option>
</select>
```

🎯 **Bonus:** Add a `multiple` attribute to allow multiple selections!  

---

## 📖 Part 3: Buttons & Form Submission  

### 🔹 **Submit Button (`<button type="submit">`)**  
```html
<button type="submit">Submit Form</button>
```

### 🔹 **Reset Button (`<button type="reset">`)**  
```html
<button type="reset">Clear Form</button>
```

### 🔹 **Button with JavaScript Action**  
```html
<button type="button" onclick="alert('Button Clicked!')">Click Me</button>
```

🎯 **Bonus:** Try using an `<input type="submit">` instead of `<button>`!  

---

## 📖 Part 4: Styling Forms with CSS  

📌 **Task:** Style a form using **CSS**.  

```css
form {
  width: 300px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
}

input, select, textarea {
  width: 100%;
  margin-bottom: 10px;
  padding: 8px;
}

button {
  background-color: blue;
  color: white;
  padding: 10px;
  border: none;
  cursor: pointer;
}
```

🎯 **Bonus:** Add `:focus` styles to highlight selected input fields!  

---

## 📖 Part 5: Introduction to Web Components  

🎯 **What Are Web Components?**  
Web Components allow you to **create reusable custom elements**.  

🔹 **Example: Creating a Custom Button Component**  
```html
<custom-button>Click Me!</custom-button>

<script>
class CustomButton extends HTMLElement {
  connectedCallback() {
    this.innerHTML = `<button>${this.innerText}</button>`;
  }
}
customElements.define('custom-button', CustomButton);
</script>
```

🎯 **Bonus:** Create a reusable **input field component**!  

---

## 🛠️ Lab Challenge: Create a Complete Contact Form  

📌 **Task:** Build a **styled contact form** that collects **name, email, message**, and has a submit button.  

```html
<form action="submit.php" method="POST">
  <h2>Contact Us</h2>
  
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <label for="message">Message:</label>
  <textarea id="message" name="message" rows="4"></textarea>

  <button type="submit">Send Message</button>
</form>
```

🎯 **Bonus:** Add JavaScript to **validate the form before submission**!  

---

## 🎒 Homework & Next Steps  
✅ **Create your own custom form (e.g., a Sign-Up Form or Feedback Form).**  
✅ **Try styling your form using CSS.**  
✅ **Experiment with Web Components to create reusable buttons or inputs.**  

📢 **Next Lesson:** **Lesson 2: CSS Basics – Styling Your Website!** 🚀  

---

## 🛠️ Additional Resources  

📌 **MDN Docs – HTML Forms**  
🔗 [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)  

📌 **W3Schools – Form Elements & Attributes**  
🔗 [https://www.w3schools.com/html/html_forms.asp](https://www.w3schools.com/html/html_forms.asp)  

📌 **CSS Styling for Forms**  
🔗 [https://www.w3schools.com/css/css_form.asp](https://www.w3schools.com/css/css_form.asp)  

---

# 🎉 Lesson Wrap-Up  
✅ We learned **how to create and customize forms** in HTML.  
✅ We explored **input fields, buttons, dropdowns, and textareas**.  
✅ We introduced **basic form styling & Web Components**.  
