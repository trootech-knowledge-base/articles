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

2nd paragraph. *Functional Components*, **Class Components**, and `JSX`. Itemized lists look like:

  * Declarative UI
  * Component-Based
  * Learn Once, Write Anywhere

Note that --- not considering the asterisk --- the actual text content starts at 4-columns in.

> React allows you to build encapsulated components.
>
> They manage their own state and update efficiently when data changes.

Use 3 dashes for an em-dash. Use 2 dashes for ranges (ex., "React versions 16--18"). Three dots ... will be converted to an ellipsis.


An h2 header
------------

Here's a numbered list of core React concepts:

 1. Components and Props
 2. State and Lifecycle
 3. Handling Events
 4. Conditional Rendering

Note again how the actual text starts at 4 columns in (4 characters from the left side). Here's a code sample:

    function Welcome(props) {
        return <h1>Hello, {props.name}</h1>;
    }

As you probably guessed, indented 4 spaces. By the way, instead of indenting the block, you can use delimited blocks, if you like:

~~~jsx
function App() {
    return (
        <div>
            <h1>Welcome to React</h1>
        </div>
    );
}
~~~

(which makes copying & pasting easier). You can optionally mark the delimited block for syntax highlighting:

~~~javascript
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
~~~


### An h3 header ###

Now a nested list:

 1. First, install React:

      * `npm install react`
      * `npm install react-dom`

 2. Create a new project:

      ```bash
      npx create-react-app my-app
      cd my-app
      npm start
      ```

 3. Start coding!

    Follow these steps:

        import React from 'react';
        function App() {
            return <h1>Hello React!</h1>;
        }

    Export the component and use it in your project.

Here's a link to [React Docs](https://reactjs.org), to a [local component](local-component.html), and to a [section heading in the current doc](#an-h2-header). Here's a footnote [^1].

[^1]: React was originally created by Facebook.

Tables can look like this:

Feature        | Description
------------- | -------------------------
JSX           | JavaScript syntax extension
Components    | Reusable UI elements
Virtual DOM   | Efficient rendering
Hooks         | State & lifecycle without classes

Table: React core features.

(The above is the caption for the table.)

A horizontal rule follows.

***

Here's a definition list:

JSX
  : A syntax extension that lets you write HTML in JavaScript.

State
  : A component’s memory in React.

Props
  : Arguments passed to React components.

Again, text is indented 4 spaces. (Put a blank line between each term and its definition to spread things out more.)

Here's a "line block" (note how whitespace is honored):

| React is
|   a powerful
| library for UI development.

and images can be specified like so:

![React Logo](https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg "React Framework")

Inline math equation: $f(x) = x^2$. Display math should get its own line like so:

$$y = mx + b$$

And note that you can backslash-escape any punctuation characters which you wish to be displayed literally, ex.: \`code\`, \*React\*, etc.
