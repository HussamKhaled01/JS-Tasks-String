# 🚀 JavaScript — Web Storage Tasks

---

## 🟢 Task 1 — Save Simple Data

### 🎯 Objective
Implement basic data persistence using `localStorage`.

### 💻 Requirements
- Create an input field for user input
- Add a button labeled **"Save Name"**

### ✅ Expected Outcome
- Store the entered name in `localStorage`
- Retrieve and display the stored name on the page

---

## 🟡 Task 2 — Store Object Data

### 🎯 Objective
Work with structured data using JSON in `localStorage`.

### 💻 Requirements
Create a form that includes:
- Name field
- Email field

### ✅ Expected Outcome
- Store the form data as a JavaScript object in `localStorage`
- Use `JSON.stringify()` when saving data
- Use `JSON.parse()` when retrieving data
- Display the stored data on the page
- Ensure data persists after page reload

---

## 🔴 Final Task — Search System with Storage

### 🎯 Objective
Build a dynamic search system that utilizes `localStorage` for data persistence and state management.

---

### 🧩 Step 1 — Data Initialization

users = [
  { name: "Ahmad" },
  { name: "Ali" },
  { name: "Sara" },
  { name: "Lana" }
]

---

### 🧩 Step 2 — Data Storage
Persist the users array in `localStorage` using `JSON.stringify()` to ensure structured data is stored correctly.

---

### 🧩 Step 3 — User Interface
Design and implement:
- A search input field for user interaction
- A results container to display filtered data dynamically

---

### 🧩 Step 4 — Search Functionality

#### ✅ Expected Outcome
- Capture user input in real-time (e.g., using `input` event)
- Filter the stored users based on the search query
- Dynamically render matching results in the UI

---

### 🧩 Step 5 — Persistent Search State

#### ✅ Expected Outcome
- Store the last search query in `localStorage`
- On page reload:
  - Restore the previous search value in the input field
  - Automatically display the corresponding filtered results

---

## ⚡ Bonus Enhancements (Optional)

- Display a **"No results found"** message when no matches are returned
- Implement case-insensitive search for better usability
- Add functionality to delete users from both the UI and `localStorage`