# React useEffect Hook Missing Cleanup Function

This example demonstrates a common error in React applications: forgetting to include a cleanup function in the useEffect hook.  This can cause memory leaks and unexpected behavior.

## Problem
The `bug.js` file showcases the issue.  The `useEffect` hook logs a message when the component mounts, but lacks a return statement for a cleanup function.  This means that any side effects (e.g., subscriptions, timers) started within the effect will not be properly cleaned up when the component unmounts.

## Solution
The `bugSolution.js` file provides the correct implementation. A return function is added inside the `useEffect` to clean up the side effects.  In this simple example, there are no side effects to clean up but the structure shows how to correctly implement a cleanup function.