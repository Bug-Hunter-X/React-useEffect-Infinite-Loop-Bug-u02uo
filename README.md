# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook causing an infinite render loop. The bug occurs when the `useEffect` hook is missing a dependency array, leading to it running after every render. This example shows the problem and its solution.

## Bug
The `bug.js` file contains the buggy component. The `useEffect` hook logs a message to the console after every render, creating an infinite loop and spamming the console.

## Solution
The `bugSolution.js` file demonstrates the solution. By adding `[count]` as a dependency array to the `useEffect` hook, it only runs when the `count` variable changes.