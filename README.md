# 📝 FAQ Toggle System – JavaScript Practice Project

This is a simple FAQ (Frequently Asked Questions) system built with HTML, CSS, and JavaScript. It allows users to click on a question to toggle the visibility of the corresponding answer. This project was created as a hands-on practice for learning **DOM manipulation**, **event bubbling**, and **event delegation** in JavaScript.

---

## 🚀 Features

- Toggle answers on question click  
- Collapse any open answers when clicking outside  
- Event delegation using a single event listener  
- Efficient handling of dynamic content  
- Clean and minimal HTML structure

---

## 🎯 What I Learned

### 🔹 Event Delegation
Instead of adding individual event listeners to each question, I used a single event listener on the parent `.faq` container. This improves performance and simplifies code:

```js
faq.addEventListener("click", function(e) {
  if (e.target.classList.contains("question")) {
    // toggle logic here
  }
});
```
### 🔹 Event Bubbling
The project demonstrates how events bubble up from child to parent elements. I used e.stopPropagation() to control bubbling when necessary.

### 🔹 DOM Traversal
I practiced navigating the DOM using properties like parentElement and querySelector to find and toggle the correct answer element.

### 🔹 Click Outside Detection
To close any open answers when clicking outside the FAQ, I used a document-level click listener combined with faq.contains(e.target).

```faq-project/
├── index.html
├── styles.css
└── script.js
```
