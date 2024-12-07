# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The error occurs when attempting to increment a numeric field with a non-numeric value resulting in an unexpected update or an error.

## Bug Description
The provided code snippet shows an attempt to increment the `age` field in a document by the string value '2'.  The `$inc` operator expects a numeric value and will not implicitly convert the string to a number, leading to the age value not being correctly incremented or a potential error.

## Solution
The solution corrects the `$inc` operation by providing a numeric value (e.g., 2) to the operator, thereby correctly incrementing the `age` field.