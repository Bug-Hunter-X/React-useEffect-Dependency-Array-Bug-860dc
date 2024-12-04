# React useEffect Dependency Array Bug

This repository demonstrates a common error in React's `useEffect` hook:  incorrectly specifying the dependency array, leading to infinite rendering.

## The Problem

The `bug.js` file contains a component that uses `useEffect` to log the count. However, the dependency array is missing `count`, causing the effect to run after every render, leading to an infinite loop of updates.

## The Solution

The `bugSolution.js` file corrects the issue by including `count` in the dependency array.  This ensures that the effect only runs when the `count` value changes.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the infinite logging in the console (for `bug.js`) and the corrected behavior in `bugSolution.js`.
