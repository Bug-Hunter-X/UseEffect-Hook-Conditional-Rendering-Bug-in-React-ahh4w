# React useEffect Hook Conditional Rendering Bug
This repository demonstrates a common bug in React's `useEffect` hook related to conditional rendering. The bug involves an incomplete conditional statement in the `useEffect` hook that prevents the document title from updating when the count is 0.

## Bug Description
The `MyComponent` component uses the `useState` hook to manage a count. The `useEffect` hook is intended to update the document title whenever the count changes. However, the conditional statement `if (count > 0)` within `useEffect` only updates the title when the count is greater than 0, leading to a missing title update when the count is 0.

## Solution
The solution involves modifying the conditional logic within the `useEffect` hook to always update the document title, regardless of the count value. This ensures that the title correctly reflects the current count, even when it is 0.

## How to reproduce the bug
1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe that the document title only updates when the count is greater than 0.