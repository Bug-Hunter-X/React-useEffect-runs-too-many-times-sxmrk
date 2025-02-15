# React useEffect Bug

This repository demonstrates a common bug in React's `useEffect` hook where the dependency array is not correctly specified, causing the effect to run more frequently than intended.

## Bug Description
The `useEffect` hook in `bug.js` has an empty dependency array `[]`. This makes the effect run after every render, regardless of changes in state or props. This can lead to performance issues and unexpected behavior.

## Bug Solution
The corrected code in `bugSolution.js` specifies the `count` variable in the dependency array `[count]`. This ensures the effect only runs when the `count` variable changes, fixing the performance issues and resolving the unexpected re-renders.