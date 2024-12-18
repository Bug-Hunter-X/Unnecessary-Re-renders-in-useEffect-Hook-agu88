# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook. The provided `MyComponent` function uses `useEffect` to log the current count to the console after every render. This is inefficient and can lead to performance issues, especially with complex components. The issue arises from the missing dependency array in the `useEffect` call. 

**To reproduce the bug:** Clone this repository and run the code.  Observe the excessive console logs.

**Solution:** The solution involves fixing the `useEffect` dependency array to only run the effect when the count changes.