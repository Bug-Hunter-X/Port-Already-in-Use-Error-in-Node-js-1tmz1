# Node.js Port Already in Use Error

This repository demonstrates a common error in Node.js development: attempting to start a server on a port that is already in use.  The `bug.js` file contains the problematic code, while `bugSolution.js` provides a solution.

## Problem

The `bug.js` file creates a simple HTTP server using the `http` module. If you attempt to run this file while another process is already using port 8080, the server will fail to start and throw an error.

## Solution

The `bugSolution.js` file demonstrates how to handle this error gracefully using the `'error'` event listener of the `http.Server` object.