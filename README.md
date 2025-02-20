# MongoDB $inc Operator Error: Unexpected Type

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numeric field by a specified value. However, if the value provided is not a number (e.g., a string), the operation will fail silently, resulting in unexpected behavior. 

## Bug

The `bug.js` file contains code that attempts to increment a field with a string value. This leads to an incorrect update, potentially causing data inconsistency.

## Solution

The `bugSolution.js` file demonstrates the correct usage of the `$inc` operator, ensuring that only numeric values are used for incrementing.

## How to Reproduce

1. Clone this repository.
2. Run `bug.js`. Observe the unexpected outcome.
3. Run `bugSolution.js`. Observe the correct increment.
