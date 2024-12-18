# Node.js Server Port Already in Use Error

This repository demonstrates a common error in Node.js applications where the server fails to start because the specified port is already in use.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a solution.

## Description

The issue arises when attempting to bind a Node.js server to a port that's currently occupied by another process (e.g., another server, a different application).  This results in an error preventing the server from starting.

## How to reproduce

1. Clone this repository.
2. Run `node bug.js`.
3. While the server is running, attempt to run `node bug.js` again. You should encounter the error.

## Solution

The `bugSolution.js` file demonstrates several ways to handle this scenario, including using a `try...catch` block and gracefully handling the error.

This issue highlights the importance of error handling and resource management in Node.js applications.