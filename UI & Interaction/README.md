# JavaScript Tasks — UI & Interaction

## 🧠 Research Summary

### 1. Interaction Events
Interaction events enable the browser to respond to user actions and input.

- `mouseover` / `mouseout`  
  Triggered when the mouse enters or leaves an element.

- `change`  
  Fired when the value of `<input>`, `<select>`, or `<textarea>` changes (after user commits the change).

- `input`  
  Fired on every value change, providing real-time feedback (ideal for live previews/editors).

---

### 2. UI State Management

The most effective way to manage UI changes is by toggling **CSS classes** instead of modifying styles directly.

**Why this approach:**
- 🎯 **Separation of concerns** → CSS handles design, JavaScript handles behavior
- ⚡ **Performance** → One class change is more efficient than multiple inline style updates
- 🔧 **Maintainability** → Easier to debug and scale

---

### 3. CSS Transitions vs JavaScript Intervals

- ✅ **CSS Transitions**
  - Best for smooth visual changes (color, opacity, transform)
  - Hardware-accelerated
  - Cleaner and more efficient for UI animations

- ⚙️ **setInterval**
  - Used for repeated, time-based logic
  - Suitable for dynamic behaviors (timers, color cycling, custom animations)

---

## 🚀 Practical Tasks

### 🟡 Task 1 — Hover Effect
**Requirement:**
- Change background to yellow
- Make text bold on hover

**Logic:**
- Use `mouseover` to add a highlight class
- Use `mouseout` to remove it
- Ensures automatic return to original state

---

### 🌍 Task 2 — Country Dropdown & Flag
**Requirement:**
- Display a flag based on selected country

**Logic:**
- Listen to `change` event on `<select>`
- Use selected value to update `<img src>`

---

### 👁️ Task 3 — Show / Hide Content
**Requirement:**
- Toggle visibility using a button

**Logic:**
- Use `classList.toggle('hidden')`
- Avoids issues with `style.display`
- Keeps layout logic inside CSS

---

### ✍️ Task 4 — Mini Text Editor
**Requirement:**
- Allow text formatting:
  - Bold
  - Underline
  - Font size
  - Font family

**Logic:**
- **Bold / Underline:** toggle classes using `classList`
- **Font Size / Family:** update dynamically using `input` / `change` events

---

### 🎨 Task 5 — Animated Color Box
**Requirement:**
- Change box color over time

**Logic:**
- Use CSS `transition` for smooth animation
- Use `setInterval` to cycle through colors automatically

---