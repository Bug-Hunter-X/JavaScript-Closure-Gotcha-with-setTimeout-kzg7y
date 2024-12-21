# JavaScript Closure Gotcha with setTimeout

This example demonstrates a common pitfall in JavaScript related to closures and the `setTimeout` function.

The issue is that the value of `i` is not captured for each iteration of the loop.  By the time `setTimeout` finally executes, the loop has completed, and `i` has reached its final value of 10.

The solution involves using a closure to capture the value of `i` in each iteration, as shown in `bugSolution.js`.

This is a fundamental concept in JavaScript, so understanding it is crucial for writing correct and reliable code.