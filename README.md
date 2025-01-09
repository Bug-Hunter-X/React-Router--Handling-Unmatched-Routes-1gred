# React Router Unmatched Route Bug

This repository demonstrates a common bug in React Router v6 and its solution.

## Bug Description

The application uses `react-router-dom` v6.  It has routes for '/' and '/about'.  If a user navigates to a non-existent route (e.g., '/invalid'), React Router v6 defaults to rendering nothing.  This can lead to unexpected blank screens.

## Solution

The solution involves adding a catch-all route using `*` to handle all unmatched paths. This provides a graceful fallback, preventing blank screens and handling potential errors.  A fallback component will display on invalid route paths. 