# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common error in React 19 involving the `useEffect` hook.  The issue arises when an effect runs after every render due to a missing or incorrect dependency array.

## Bug Description
The provided `MyComponent` uses `useEffect` without a dependency array.  This causes the effect to re-run every time the component re-renders, creating an infinite loop of re-renders and console logs. In React 18 and earlier this could lead to performance issues, in React 19 it will likely cause an error or crash.