# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by missing dependencies in the dependency array.

## The Bug
The `bug.js` file contains a component that uses the `useEffect` hook to log the current count to the console. However, the dependency array is missing, causing the effect to run after every render, triggering another render, and creating an infinite loop. 

## The Solution
The `bugSolution.js` file shows the corrected code with the `count` variable added to the dependency array. This ensures the effect only runs when the `count` value changes.