# React Infinite useEffect Loop

This repository demonstrates a common React bug: an infinite loop caused by an incorrectly used `useEffect` hook.

The `bug.js` file contains the buggy code. The `useEffect` hook logs the count to the console after every render. Since `count` updates in every render, `useEffect` triggers again, creating an infinite loop.

The solution (`bugSolution.js`) correctly uses the functional update pattern and prevents the infinite loop by optimizing the re-renders.