# React useEffect Infinite Loop

This repository demonstrates a common error in React applications: an infinite loop caused by incorrect usage of the `useEffect` hook.

## Bug Description

The `useEffect` hook in `bug.js` has a dependency array that includes `count`. The effect function updates the `count` state, causing a re-render, triggering the `useEffect` again, and creating an infinite loop. This results in a browser freeze or crash.

## Solution

The solution, provided in `bugSolution.js`, addresses this issue by removing `count` from the dependency array or modifying the logic within the useEffect to correctly manage state updates.