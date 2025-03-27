---
layout: post
title: Quick React Guide
subtitle: A brief overview of React fundamentals
excerpt_image: https://reactjs.org/logo-og.png
categories: react
tags: [guide, react]
top: 2
---

![banner](https://reactjs.org/logo-og.png)

React is a JavaScript library for building user interfaces. It makes it painless to create interactive UIs with reusable components.

## Introduction

React enables developers to build fast, scalable, and simple user interfaces. Some key features include:

- **Declarative UI**: React makes it easy to design interactive UIs with simple component structures.
- **Component-Based**: Build encapsulated components that manage their state and compose them to make complex UIs.
- **Learn Once, Write Anywhere**: Use React to develop web and mobile applications efficiently.

> React allows you to build encapsulated components that manage their state and update efficiently when data changes.

---

## Core Concepts

### JSX
JSX allows you to write HTML inside JavaScript. Example:

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}!</h1>;
}
```

### Components and Props
React applications are built using components. There are two types:

1. **Functional Components**
2. **Class Components**

Example of a functional component:

```jsx
function Greeting({ name }) {
  return <h1>Hello, {name}!</h1>;
}
```

### State and Lifecycle
State allows components to manage changing data. Example:

```jsx
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}
```

---

## Setting Up a React Project

Follow these steps to get started:

1. Install React:

   ```sh
   npx create-react-app my-app
   cd my-app
   npm start
   ```

2. Start coding:

   ```jsx
   import React from 'react';
   function App() {
     return <h1>Welcome to React!</h1>;
   }
   export default App;
   ```

3. Run the project and see the output in your browser.

---

## React Features Overview

| Feature     | Description |
|------------|------------|
| JSX        | JavaScript syntax extension for writing UI components |
| Components | Reusable and self-contained building blocks |
| Virtual DOM | Efficiently updates the UI without re-rendering the whole DOM |
| Hooks      | Enables functional components to manage state and side effects |

---

## Conclusion

React is a powerful UI library used by developers worldwide. Understanding its core concepts will help you build dynamic, scalable applications efficiently.

For more details, check out the [official React documentation](https://reactjs.org).
