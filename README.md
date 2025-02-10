# Unhandled Request in Express.js
This repository demonstrates a common error in Express.js applications where requests are received but the server fails to send a response, leading to hanging requests. The issue stems from a missing `res.send()` or `res.json()` call within the request handler.

## Bug
The `bug.js` file shows an Express.js server that logs an incoming request to the console but doesn't actually send a response to the client. This results in the client waiting indefinitely for a response.

## Solution
The `bugSolution.js` file fixes the bug by adding `res.send()` to the request handler, sending a simple 'Hello, world!' response to the client.