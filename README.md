# MongoDB $inc Operator Unexpected Behavior
This repository demonstrates an uncommon bug encountered when using the `$inc` operator in MongoDB's `updateOne` method.  The bug arises from providing a string value instead of a numeric value to the `$inc` operator.

## Bug Description
The incorrect use of `$inc` with a string argument can lead to the field not being incremented as expected or other unforeseen behaviors.

## Bug Reproduction
1.  Ensure you have a MongoDB instance running.
2.  Create a collection named `myCollection` with at least one document containing a numeric field named `count`.
3.  Execute the provided JavaScript code in a MongoDB shell or Node.js application.
4. Observe the unexpected behavior in the result.

## Solution
The solution involves ensuring that the value passed to the `$inc` operator is a valid number.