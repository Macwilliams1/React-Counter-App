import React, { useState } from "react";
import "./Counter.css";

function Counter() {
  const [count, setCount] = useState(0);
  const limit = 10;

  const increase = () => {
    if (count < limit) {
      setCount(count + 1);
    }
  };

  const decrease = () => {
    if (count > 0) {
      setCount(count - 1);
    }
  };

  return (
    <div className="counter-container">
      <h1>Counter App</h1>
      <p className="count-value">{count}</p>
      
      {count === limit && (
        <p className="limit-message">🎉 You've reached the limit!</p>
      )}

      <div className="button-group">
        <button onClick={increase} className="btn increase">Increase</button>
        <button onClick={decrease} className="btn decrease">Decrease</button>
      </div>
    </div>
  );
}

.counter-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 50px;
  font-family: Arial, sans-serif;
}

h1 {
  color: #333;
}

.count-value {
  font-size: 3rem;
  margin: 20px 0;
}

.limit-message {
  color: red;
  font-weight: bold;
  margin-bottom: 10px;
}

.button-group {
  display: flex;
  gap: 15px;
}

.btn {
  padding: 10px 20px;
  font-size: 1rem;
  border-radius: 8px;
  border: none;
  cursor: pointer;
  transition: 0.2s;
}

.increase {
  background-color: #4caf50;
  color: white;
}

.decrease {
  background-color: #f44336;
  color: white;
}

.btn:hover {
  opacity: 0.8;
}

import React from "react";
import Counter from "./Counter";

function App() {
  return (
    <main>
      <Counter />
    </main>
  );
}

export default App;


export default Counter;
