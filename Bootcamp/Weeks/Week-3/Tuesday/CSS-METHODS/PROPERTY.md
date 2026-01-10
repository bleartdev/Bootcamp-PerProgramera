# 📘 CSS Priority (Inline, Internal, External)

This document explains **which type of CSS has priority (takes precedence)**
when multiple styles are applied at the same time in HTML.

---

## 🧱 Types of CSS

### 1️⃣ Inline CSS
- Written directly inside an HTML element
- Used via the `style` attribute

```html
<p style="color: red;">Text</p>
```
**Characteristics:**

- ✅ Has the highest priority  
- Applies the style only to that specific element  

**Disadvantages:**

- Makes the code messy  
- Hard to maintain  
- Not recommended for large projects  

---

### 2️⃣ Internal CSS
- Written inside the HTML document  
- Placed inside the `<style>` tag within `<head>`

```html
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```

**Characteristics:**

- Has higher priority than External CSS  
- Affects only that specific HTML page  
- Suitable for small pages or testing  

**Disadvantages:**

- Cannot be reused across other pages  
- Not suitable for large projects  

---

### 3️⃣ External CSS
- Written in a separate file (`style.css`)  
- Linked to the HTML using `<link>`

```html
<link rel="stylesheet" href="style.css">
```

**Characteristics:**

- Most commonly used in real-world projects  
- Code is well organized  
- ❌ Has the lowest priority  

**Disadvantages:**
- Has lower priority compared to Internal and Inline CSS  
- Depends on the CSS file loading (if the file is missing, styles won’t apply)  
- Small changes require opening an additional file  

---


### 🥇 Priority Order

- From highest to lowest priority:

- 1️⃣ Inline CSS  
- 2️⃣ Internal CSS  
- 3️⃣ External CSS  

➡️ If all three are applied to the same element, **Inline CSS wins**.
