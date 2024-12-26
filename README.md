# React useEffect Hook with Incorrect Dependency Array

This repository demonstrates a common error in React applications involving the `useEffect` hook and its dependency array.  The provided `bug.js` file shows an example where the dependency array is incorrectly set to empty (`[]`), preventing the effect from running whenever the relevant state changes.

The correct implementation, provided in `bugSolution.js`, demonstrates the proper use of the dependency array to ensure the effect runs only when the `count` state changes.

## Bug:
The initial code includes an empty dependency array in the useEffect hook. This means the effect runs only when the component mounts. Even though the count variable changes, the effect doesn't re-run.