# Express.js Route Handler Bug: Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when dealing with user input.  The provided code attempts to retrieve a user from an array based on a user ID from the request parameters, but fails to handle cases where the ID is invalid (e.g., not a number).  This can lead to unexpected errors or crashes.

The `bug.js` file contains the erroneous code.  The `bugSolution.js` file provides a corrected version that includes robust error handling.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `node bug.js` and try accessing the route with an invalid ID (e.g., `/users/abc`).
4. Observe the error.
5. Run `node bugSolution.js` and try accessing the same route. The improved error handling will prevent the crash and return a more informative response.