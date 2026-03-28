# JavaScript Task — GitHub Users Viewer

This project focuses on asynchronous programming and dynamic DOM manipulation by fetching real-time data from the GitHub API.

---

## 🎯 Objective
Learn how to fetch data from an external API and display it dynamically on a webpage using Vanilla JavaScript.

---

## 🌐 API Endpoint
**URL:** `https://api.github.com/users`

### 🧠 Data Structure
Each user object in the API response contains:
* `login`: The GitHub username.
* `avatar_url`: The profile image URL.
* `html_url`: The link to the user's GitHub profile.

---

## 💻 Requirements

### 🔹 1. Fetch Data
* Use the `fetch()` API to request data.
* Convert the response into JSON format.

### 🔹 2. Handle Data
* The response is an **Array** of users.
* Use a loop (e.g., `forEach` or `map`) to iterate through the user data.

### 🔹 3. Display Data (DOM)
For each user, create elements to display:
* **Profile Image**
* **Username**
* **Profile Link**

### 🔹 4. UI Structure
* Each user must be wrapped inside a **Card** component.
* **Layout:**
  * `[ Image ]`
  * `Username`
  * `Profile Link`

### 🔹 5. Container
* Create a main container in your HTML file.
* Use JavaScript to append all generated user cards into this container.

---

## ⚠️ Rules
* **No Hardcoding:** All content must be generated from the API data.
* **Vanilla JS:** Use only pure JavaScript (no external libraries like jQuery or React).

---

## ⚡ Bonus Features (Completed)
* **Limit Results:** Display only the first 10 users.
* **Styling:** Implemented Grid/Flexbox for the layout.
* **Interactions:** Added hover effects on cards and links that open in a new tab.
* **Search:** Included a filter to search for specific usernames.

---