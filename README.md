# Express.js Unhandled Error Example

This repository demonstrates a common error in Express.js applications: insufficient error handling in route handlers.

The `bug.js` file showcases a route that fetches user data from a database. It lacks proper error handling for database errors and cases where the requested user doesn't exist. This can lead to server crashes or unexpected responses to the client.

The `bugSolution.js` file provides a corrected version with comprehensive error handling, ensuring robust and reliable application behavior.

## How to Reproduce the Bug

1. Clone this repository.
2. Run `node bug.js`.
3. Send requests to `/users/:id` with invalid or nonexistent IDs.
4. Observe the server's response and/or console output.

## How to Fix the Bug

Refer to `bugSolution.js` for a corrected implementation that incorporates proper error handling.