# MongoDB Aggregation Pipeline Error: Incorrect $inc usage

This repository demonstrates a common error when using the `$inc` operator in MongoDB aggregation pipelines. The `$inc` operator is designed to increment a field's value, but it must be used within the `$group` stage.  Using it outside of `$group` will lead to an error.

The `bug.js` file shows the erroneous code, while `bugSolution.js` provides the corrected version.

## How to reproduce

1. Clone this repository.
2. Ensure you have a MongoDB instance running.
3. Run `bug.js` (you'll need a suitable collection with data).
4. Observe the error.
5. Run `bugSolution.js` to see the corrected implementation.