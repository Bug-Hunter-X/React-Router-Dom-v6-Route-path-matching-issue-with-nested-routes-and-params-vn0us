# React Router Dom v6 Route path matching issue
This repository demonstrates a bug in React Router Dom v6 related to path matching with nested routes and optional parameters.  The issue specifically arises when a path contains dynamic segments with optional parts, causing incorrect matching behavior.

## Problem Description
The problem is that paths with optional parameters in nested routes aren't matched correctly.  If the optional parameter is missing, the route may not be recognized as intended.

## Solution
The solution involves a careful restructuring of routes and potentially the use of route guards or custom logic to handle optional parameters effectively. The `useParams` hook may require specific handling.  Details can be found in `bugSolution.js`.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to paths such as `/users/123` and `/users` to observe the incorrect behavior.