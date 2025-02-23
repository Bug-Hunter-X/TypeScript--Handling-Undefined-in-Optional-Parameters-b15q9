# TypeScript: Handling Undefined in Optional Parameters

This repository demonstrates a common bug in TypeScript related to handling undefined values in function parameters.

## The Bug
The `greet` function in `bug.ts` attempts to handle null values gracefully. However, it fails to address the scenario where the input `name` is undefined. This results in a runtime error. 

## The Solution
The solution provided in `bugSolution.ts` addresses this by explicitly checking for both `null` and `undefined` using the `typeof` operator. This ensures robust handling of optional parameters or potentially undefined values, preventing runtime errors.

## How to Reproduce
1. Clone this repository.
2. Navigate to the repository's root directory.
3. Compile and run the `bug.ts` file using a TypeScript compiler (tsc) and Node.js (node). Observe the error when calling greet with undefined.
4. Repeat step 3 with `bugSolution.ts`. The improved function should handle the undefined value without errors.