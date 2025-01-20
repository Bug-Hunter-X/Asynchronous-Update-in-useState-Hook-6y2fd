# Asynchronous Update in React's useState Hook

This example demonstrates a common misconception about the `useState` hook in React.  Because state updates are asynchronous, logging the state value immediately after calling `setCount` will not reflect the updated value. This can lead to unexpected behavior if you rely on the immediate update.

## Bug
The `bug.js` file contains a functional component that increments a counter.  The `console.log` statement inside the `handleClick` function demonstrates the problem: it logs the *previous* count value, not the updated one.

## Solution
The `bugSolution.js` file shows how to correctly handle the asynchronous update.  It demonstrates using useEffect to log the state after the state update is completed. 

## How to Run
1. Clone this repo.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.