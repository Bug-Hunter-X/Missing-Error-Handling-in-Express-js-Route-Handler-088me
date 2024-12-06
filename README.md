# Express.js Route Handler Error

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  The `bug.js` file contains the flawed code, while `bugSolution.js` provides a corrected version.

The bug occurs when a user ID is passed that is not a valid integer.  The code attempts to convert the ID to an integer using `parseInt()`, but if the conversion fails (resulting in NaN), the code crashes without appropriate error handling.  This leads to a poor user experience and potential application instability.

The solution adds robust error handling to gracefully manage such scenarios, returning appropriate HTTP status codes and user-friendly messages.