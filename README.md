# Swift Array Map Function Unexpected Behavior

This repository demonstrates a common, yet subtle, error that can occur when using the `map` function with arrays in Swift. The error arises from misunderstanding how `map` transforms the original array.

## The Bug

The `bug.swift` file contains code that attempts to double the values in an array using the `map` function.  While the code appears correct, it doesn't account for potential issues that might arise. The subtle error relates to how the original array is not affected by the `map` function. 

## The Solution

The `bugSolution.swift` file demonstrates the corrected approach.  A common mistake is to attempt to modify the original array in place.  The `map` function returns a *new* array with transformed elements, leaving the original array unchanged.