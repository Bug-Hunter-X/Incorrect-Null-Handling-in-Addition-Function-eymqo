# Incorrect Null Handling in Addition Function

This repository demonstrates a common JavaScript bug related to incorrect null handling in a simple addition function. The function `foo` is designed to add two numbers, but it incorrectly treats any nullish value (null or undefined) as null and returns null. This behavior is not ideal, as it does not handle other falsy values like 0 or "".

## Bug

The `bug.js` file contains the buggy function.  The function returns `null` if either `a` or `b` is `null`, even if the other value is a valid number.

## Solution

The `bugSolution.js` file provides a corrected version of the function. The improved function checks explicitly for null and undefined, allowing other falsy values to be processed correctly.  This makes the function more robust and reliable.