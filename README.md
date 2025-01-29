# Unexpected Behavior with Negative Input in TypeScript Function

This repository demonstrates an unexpected behavior in a TypeScript function when provided with a negative input. The function `printNumbers` is intended to print numbers from 1 to n. However, when n is negative, it does not throw an error or produce any output, unlike what one might intuitively expect.

## Bug Description
The `printNumbers` function uses a simple for loop.  The loop condition `i <= n` will always be false if n is negative, resulting in zero iterations and no output. This is technically correct, but lacks robust error handling. A more user-friendly approach would be to handle negative inputs gracefully, perhaps by throwing an error or returning a message.

## Solution
The solution includes error handling for negative inputs.  It now explicitly throws an error when a negative value is provided, providing informative feedback to the user.
