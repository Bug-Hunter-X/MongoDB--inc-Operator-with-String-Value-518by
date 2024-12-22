# MongoDB $inc Operator with String Value
This repository demonstrates an uncommon error related to the MongoDB `$inc` operator when used incorrectly with a string value instead of a number.

The `bug.js` file contains the code with the error. The `bugSolution.js` file demonstrates the correct usage of the `$inc` operator.

## Bug Description
The `$inc` operator in MongoDB is designed to increment a numerical field by a specified value. Attempting to use the `$inc` operator with a string value will result in an error because MongoDB expects a number for the increment.

## Solution
Ensure that the value you pass to the `$inc` operator is a numerical value (integer or float), not a string.