# Unhandled Invalid Operator in JavaScript Calculator

This repository demonstrates a common yet subtle error in JavaScript: failing to handle unexpected input in a function. The `operate` function handles basic arithmetic operations (+, -, *, /), but it lacks a robust mechanism for handling invalid operators. This can lead to unexpected behavior or crashes.

## The Bug

The provided JavaScript code implements a simple calculator with functions for addition, subtraction, multiplication, and division. Division by zero is correctly handled with an error. However, if an invalid operator (e.g., '%', '^') is passed to the `operate` function, it returns 'Invalid operator'.  While this handles the invalid operator gracefully, it does not prevent potential issues. A more robust solution would be to throw an error for unknown operators, enhancing error handling and debugging.

## The Solution

The solution introduces enhanced error handling for unexpected operators, throwing a more descriptive error instead of simply returning a string. This allows for better debugging and error reporting.