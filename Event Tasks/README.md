# JavaScript Mastery — DOM, Events & Interactive UI

## 🧠 Research Summary

### 1. JavaScript Events & The Event Object
An **event** is a signal that something has happened in the browser (e.g., click, input, scroll). When triggered, the browser creates an **Event Object** containing useful details:

- `event.target` → The element that actually triggered the event (child).
- `event.currentTarget` → The element that the event listener is attached to (parent).
- `event.preventDefault()` → Prevents the default browser behavior (e.g., stopping form submission).

---

### 2. Handling Events (Best Practices)

There are three main ways to handle events:

- ✅ **addEventListener (Recommended)**
  - Supports multiple listeners
  - Gives control over bubbling/capturing
  - Keeps HTML clean

- ⚠️ **DOM Property (`onclick`)**
  - Only allows one function
  - Easily overwritten

- ❌ **Inline (`onclick=""`)**
  - Mixes logic with HTML
  - Hard to maintain

---

### 3. Event Flow: Bubbling vs Capturing

Events propagate through the DOM in two phases:

- **Bubbling (Default)**
  - Event starts at the target element and moves up to parent elements

- **Capturing**
  - Event starts from the top (window) and moves down to the target

- `event.stopPropagation()`
  - Stops the event from continuing to parent elements

---

### 4. Event Delegation

A technique where a **single event listener** is attached to a parent instead of multiple children.

**Benefits:**
- 🚀 Better performance (fewer listeners)
- 🔄 Works with dynamically added elements
- 🧼 Cleaner and more maintainable code

---

## 🚀 Practical Tasks

### Task 1: Smart Button
- Toggle button state
- Change text dynamically
- Use `classList.toggle` for styling

---

### Task 2: Live Input Preview
- Listen to `input` event
- Use `event.target.value`
- Display real-time text in a paragraph

---

### Task 3: Interactive List
- Create dynamic task list
- Use **Event Delegation** on `<ul>`
- Handle item deletion efficiently

---

### Task 4: Color Changer Cards
- Manage active state across multiple elements
- Ensure only one card has the active class at a time

---

### Task 5: Toggle Visibility
- Compare:
  - `style.display`
  - `classList.toggle`
- Show and hide elements dynamically

---

### Task 6: Counter with Styling
- Build a numeric counter
- Update text color based on value:
  - Positive → Green
  - Negative → Red
  - Zero → Default

---