# Incorrect use of $inc operator in MongoDB update operation
This example demonstrates an incorrect use of the `$inc` operator in a MongoDB update operation. The `$inc` operator is used to increment or decrement a numeric field by a specified value.  However, if a string is passed as the increment value, it results in unexpected behavior. The solution provides the correct usage of the `$inc` operator.

## Bug
The bug lies in the incorrect usage of `$inc`.  Attempting to increment a numeric field by a string leads to either a silent failure or an error, depending on your MongoDB version and settings.

## Solution
The solution is to pass a number instead of a string as the increment value.