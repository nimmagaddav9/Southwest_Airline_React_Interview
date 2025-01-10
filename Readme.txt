## Southwest Airlines 

### Introduction questions
- Introduce yourself ?
In past 2 years worked on React migration team where I converted the .net pages to react in united.com 
Frontend is React, backend is Java. Used ATMOS library for CSS styling.
Worked on Forgot password, Forgot MileagePlus number, security questions, Sign-in features, Miles-Pooling, United Club pass,  Recent Activity, dashboard updates and KTN(Known Traveler Number) , Accessibility guidelines features on united.com.
New initiative worked on Miles-Pooling( points you get after traveling), TSA Precheck, Account security and management features, Under18.



- How did it all started, when did you decide you wanted to be frontend developer.
I have started as a UI Engineer and worked as Scrum Master and Release specialist have done more 35+ releases so far.


- What is your primary skill, list your skills in order of proficiency.

React.js, 
Redux-Saga, 
JavaScript, 
JSON, 
Ajax, 
HTML5, 
CSS3, 
Node.JS, 
Rest, 
Visual Studio Code, 
Git/GitHub, TeamCity, 
Postman, 
Confluence, 
Agile, 
UI Analytics (Google Analytics, Quantum Metrics), 
Mobile Web Technologies



- what did you feel about the transition from mobile development into web development.


---
### HTML questions
- What are semantic tags in HTML, what is the importance of using them ?

Semantic tags in HTML are specific HTML elements that describe the meaning and purpose of the content they enclose, rather than just how it looks, 
providing context to both developers and machines like search engines and screen readers, making the web page structure more understandable and accessible; 
essentially, they convey the "semantics" or meaning of the content on a page, going beyond just visual presentation. 

• Examples of semantic tags: <header>, <nav>, <main>, <section>, <article>, <aside>, <footer> 
• Benefits of using semantic tags:
	• Improved accessibility: Screen readers can better interpret the page structure and read content meaningfully. 
	• Better SEO: Search engines can understand the content hierarchy and relevance more accurately, potentially improving search rankings.
	• Code readability: Makes HTML code clearer and easier to maintain for developers.


- What is inline element vs block level elements ?
Every HTML element has a default block-level or inline behavior. 
Paragraphs are block-level elements, which means that they block off a whole line for themselves, 
and images are inline elements, which means they will automatically be placed next to one another on the same line.

- What is `inline-block` ? Why is it used ?
"Inline-block" is a CSS property value used to set the display style of an element, 
allowing it to behave like an inline element (flowing with text) while also enabling the ability to set specific width and height values, similar to a block element
---
### CSS Question
- What are different positions in CSS ?
The position property specifies the type of positioning method used for an element.

There are five different position values:

static: HTML elements are positioned static by default.

relative: An element with position: relative; is positioned relative to its normal position.

fixed: An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. 
The top, right, bottom, and left properties are used to position the element.

absolute: An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

sticky: An element with position: sticky; is positioned based on the user's scroll position.
---
### Javascript Questions
- What is the difference between var, let and const ?

var is function-scoped, while let and const are block-scoped. A block is a section of code contained within curly braces, such as an if statement or for loop.
var and let variables can be reassigned, but const variables cannot.
var variables are initialized with undefined, while let and const variables are not. However, var and let can be declared without being initialized, while const must be initialized during declaration.
var variables are hoisted, meaning they can be accessed before they are declared, but let and const variables are not.


- What is hoisting ?
In JavaScript, hoisting is a behavior where variable and function declarations are moved to the top of their scope before code execution. 

- What is ES6 arrow functions ?
ES6 arrow functions are a concise syntax for writing functions in JavaScript, introduced in the ECMAScript 2015 (ES6) standard, which allows for shorter, 
cleaner code by using the "fat arrow" notation (=>) to define a function without the need for the traditional "function" keyword, 
making them particularly useful for creating anonymous functions and passing functions as arguments to other functions.

- What is self invoking function and why is it useful ? what are some of the useCases ?
A "self-invoking function" (also known as an Immediately Invoked Function Expression - IIFE) is a function that executes automatically as soon as it is defined, 
essentially running its code immediately without needing to be explicitly called;

---
### React Questions
- How do you optimize the React components ?

Memoization:
React.memo:
Use React.memo to wrap functional components and prevent unnecessary re-renders when props haven't changed.
useMemo:
Use useMemo to memoize expensive calculations that depend on specific values, avoiding recalculation on every render.
useCallback:
Use useCallback to memoize callback functions, ensuring they aren't recreated on each render unless their dependencies change.
Code Splitting and Lazy Loading:
React.lazy:
Use React.lazy and Suspense to dynamically import components only when needed, reducing initial bundle size and improving load times.
Webpack/Rollup:
Use bundlers like Webpack or Rollup to split your code into smaller chunks and load them on demand.
List Virtualization:
react-window or react-virtualized: Use libraries like react-window or react-virtualized to render only the visible portion of large lists, improving performance for long lists.
Key Coordination for List Rendering:
key prop: Always provide a unique key prop for each item in a list when using methods like map. This helps React identify items efficiently and optimize re-rendering.
Performance Profiling:
React DevTools Profiler: Use the Profiler in React DevTools to identify components that are causing performance bottlenecks and analyze their render times.
Other Techniques:
Avoid unnecessary state updates:
Update state only when necessary to prevent unnecessary re-renders.
Pure components:
Consider using pure components (React.PureComponent or React.memo) to optimize components that only render when props change.
Use shouldComponentUpdate:
In class components, use shouldComponentUpdate to manually control when a component should re-render.
Batch state updates:
If you're making multiple state updates, consider batching them together to avoid unnecessary re-renders.



- When do you use a functional component ?
In React, you should use a functional component when you need a simple, presentational component that doesn't require complex state management or lifecycle methods, prioritizing readability and ease of use;


- What are the some of the ways a render function can be triggered ?
A render function is typically triggered when there are changes to a component's state or props, 
meaning that any update to the values held within the state or received as props from a parent component 
will cause the render function to re-execute and update the UI accordingly; this is the primary mechanism in frameworks like React. 


- What are pure components ? why do you use them ?
Pure components in React are a specific type of component that optimizes performance by reducing the number of render operations in the application. 
They achieve this by implementing a shallow comparison of props and state within the component, to determine if the component should re-render.

- What happens behind the scenes when shouldComponentUpdate is triggered ?
When shouldComponentUpdate is triggered in a React component, it essentially performs a check to determine whether the component needs to re-render based on the upcoming changes to its props and state; 
if the comparison logic within the method decides a re-render is not necessary, 
it returns false, effectively preventing the component from updating in the DOM, thus optimizing performance by avoiding unnecessary re-renders.


- What are the differences between flux and redux ?
While both Flux and Redux are used for managing application state in front-end development, 
the key difference is that Flux is a design pattern focused on unidirectional data flow, 
while Redux is a concrete JavaScript library that implements the Flux architecture with a single store, 
enforcing immutability and using reducers to handle state updates, making it more structured and predictable than Flux which allows for multiple stores;
---
### Unit testing 
- What is your experience with unit testing ?

Unit testing is a type of testing where individual units or components of software are tested.
In the context of React applications, a unit could be a React component, a helper function, or any other JavaScript module. 
The goal is to verify that each unit of the software performs as designed.

- What all unit testing libraries you have used ?
Jest, Enzyme, React testing library.

---
### Javascript code exercise 
What is the output of below code snippet.

```javascript
var w  = 5;
(function(x){
  alert(w)
  alert(x)
  alert(z)
  alert(y)
  y = 0
  var z = 1
})()

```
ERROR!
5
undefined
undefined
/tmp/nc1tcQYKrl/main.js:9
  console.log(y)
              ^

ReferenceError: y is not defined
    at /tmp/nc1tcQYKrl/main.js:9:15
    at Object.<anonymous> (/tmp/nc1tcQYKrl/main.js:12:3)
    at Module._compile (node:internal/modules/cjs/loader:1565:14)
    at Object..js (node:internal/modules/cjs/loader:1708:10)
    at Module.load (node:internal/modules/cjs/loader:1318:32)
    at Function._load (node:internal/modules/cjs/loader:1128:12)
    at TracingChannel.traceSync (node:diagnostics_channel:322:14)
    at wrapModuleLoad (node:internal/modules/cjs/loader:219:24)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:170:5)
    at node:internal/main/run_main_module:36:49

Node.js v22.12.0

=== Code Exited With Errors ===
