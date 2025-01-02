# React Native: Handling Null or Undefined Property Access

This repository demonstrates a common error in React Native: attempting to access a property of an object that is null or undefined. The `bug.js` file shows the problematic code, and `bugSolution.js` provides the solution.

The error typically occurs when working with asynchronous data fetching or when components render before data is fully loaded.  Proper error handling is crucial to prevent crashes and provide a better user experience.

## How to reproduce the bug

1. Clone this repository.
2. Run `npm install`.
3. Run the app. You will likely encounter an error similar to:
   `TypeError: Cannot read properties of undefined (reading 'name')`

## Solution

The solution involves using optional chaining and nullish coalescing operators to safely access the properties and provide a default value if the object or property is null or undefined.