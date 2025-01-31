# React Router Dom Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The catch-all route is intended to handle any path that doesn't match other defined routes. However, in this example, it's incorrectly capturing all routes, including valid ones.

## Problem

The `App.js` file contains a simple React Router setup. Despite having routes defined for `/` and `/about`, the catch-all route (`/*`) always renders, resulting in the 'Not Found' component being displayed.

## Solution

The `AppSolution.js` file provides a corrected version.  The issue is resolved by carefully ordering routes. The catch all route must be placed at the end after other routes to work as intended