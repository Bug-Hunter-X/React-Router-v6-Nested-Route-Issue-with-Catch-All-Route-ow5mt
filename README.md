# React Router v6 Nested Route Bug

This repository demonstrates a bug in React Router v6 where nested routes are not rendering correctly when a catch-all route (`/*`) is present. The catch-all route always matches, preventing other routes from rendering.

## Bug Description
The application uses nested routes.  Despite having specific route paths defined, the catch-all route (`/*`) always renders, preventing access to the nested routes. This occurs even when the URL matches a more specific path.

## Solution
The solution involves restructuring the routes to prioritize specific paths over the catch-all route and correctly applying nested route definitions.  The order and structure of routes within the Routes component is crucial for correct routing behavior in React Router v6.