# MongoDB $inc Operator Type Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries.  The `$inc` operator is used to increment a numeric field by a specified value.  However, providing a non-numeric value will result in an error or unexpected behavior.

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the corrected version.

## Bug
The bug arises from passing a string ('1') instead of a number (1) to the `$inc` operator.  MongoDB expects a numeric value for proper incrementation.