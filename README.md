# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling for invalid input. Specifically, the code attempts to parse a user ID from a route parameter as an integer without validating whether the parameter is actually a number.  This can lead to unexpected behavior or crashes.

## Bug
The `bug.js` file contains the erroneous code.  It attempts to find a user based on their ID, but doesn't handle cases where the ID is not a valid integer.

## Solution
The `bugSolution.js` file provides a corrected version. It includes input validation to ensure the user ID is a number before attempting to parse it and handle cases where no user is found.