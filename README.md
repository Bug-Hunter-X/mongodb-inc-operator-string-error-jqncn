# MongoDB $inc operator error: using string instead of number
This example demonstrates an error that occurs when using the MongoDB `$inc` operator with a string value instead of a numeric value. The `$inc` operator is designed to increment or decrement numeric fields in MongoDB documents.  Using a string will lead to an error because MongoDB cannot perform the increment operation on a non-numeric type.

## Bug
The bug lies in how the `$inc` operator is used.  Incorrectly providing a string value to the `$inc` operator will cause the update operation to fail. 

## Solution
The solution is to ensure that the value provided to `$inc` is a number.  The corrected code uses a numeric value for the increment, resulting in the expected behavior.