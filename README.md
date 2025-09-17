[README.md](https://github.com/user-attachments/files/22386277/README.md)
# React Counter App

A simple counter application built with **React 18** and **Vite**.  
This project demonstrates the use of **functional components** and the **useState hook** for state management.

---

##  Features
- Increase and decrease counter value.
- Prevents counter from going below zero.
- Displays a message when the counter reaches the maximum limit (10).
- Clean UI with basic styling.

---

##  Project Structure
```
react-counter-app/
├── index.html
├── package.json
├── vite.config.js
├── src/
│   ├── App.jsx
│   ├── Counter.jsx
│   ├── main.jsx
│   ├── index.css
│   └── Counter.css
```

---

##  Setup Instructions

### 1. Clone or extract the project
```bash
unzip react-counter-app.zip
cd react-counter-app
```

### 2. Install dependencies
```bash
npm install
```

### 3. Run the development server
```bash
npm run dev
```

You will see an output similar to:
```
VITE v5.2.0  ready in 300 ms

  ➜  Local:   http://localhost:5173/
```

### 4. Open in your browser
Go to [http://localhost:5173/](http://localhost:5173/) to view the app.

---

##  Requirements
- Node.js v16+  
- npm v8+  

---

##  Example Behavior
- Initial counter value = `0`  
- Clicking **Increase** increments the counter until it reaches `10`.  
- Clicking **Decrease** decrements the counter but not below `0`.  
- When the counter hits `10`, it shows:  
  >  You've reached the limit!

---

##  License
This project is for learning purposes. Free to use and modify.
