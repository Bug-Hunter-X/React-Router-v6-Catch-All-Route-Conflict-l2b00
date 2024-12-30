# React Router v6 Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other routes, preventing them from being matched correctly.

## Problem
The `App.js` file shows a simple React Router setup.  The catch-all route (`/*`) for the `NotFound` component is always selected despite other paths being available.

## Solution
The `AppSolution.js` file demonstrates the solution, which involves carefully ordering the routes.  By placing the catch-all route last, it only matches if no other routes are matched first.  This ensures the intended routing behavior is maintained.