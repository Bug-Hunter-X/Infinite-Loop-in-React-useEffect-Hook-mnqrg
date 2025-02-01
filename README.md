# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook:  an infinite loop caused by missing dependencies. The `useEffect` hook, without a dependency array, runs after every render, causing a continuous update cycle. This example shows the problem and its solution.

## Bug
The `bug.js` file contains a component that uses `useEffect` without specifying a dependency array. This leads to infinite re-renders.

## Solution
The `bugSolution.js` file demonstrates the correct usage of the `useEffect` hook with the dependency array `[count]`.  The effect now only runs when the `count` state variable changes.