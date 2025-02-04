# Node.js Module Crash Bug

This repository demonstrates a common but subtle bug in Node.js where an unhandled error in a module's exported function causes the entire module to crash, leading to difficulties in debugging.

## Description
The `bug.js` file contains a function that is exported but lacks proper error handling. When this function encounters an error, it crashes the module.  This is particularly problematic in larger applications because the error is not always clearly propagated.

The `bugSolution.js` file shows how to fix the bug using a `try...catch` block.