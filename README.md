# JavaScript Loose Comparison Pitfalls

This repository demonstrates unexpected behavior in JavaScript's loose comparison (==) operator when dealing with NaN (Not a Number) and the values 0 and -0.

## The Problem

JavaScript's loose comparison can lead to surprising results.  The example code showcases two key issues:

1. **NaN comparison:** NaN is never equal to itself or any other value using loose comparison.  This violates the reflexive property of equality (a == a).
2. **Zero comparison:**  The values 0 and -0 are considered equal by the loose comparison operator.

## Solution

Always use strict equality (===) when comparing values in JavaScript to avoid these pitfalls. Strict equality considers both value and type when determining equality.

The solution file demonstrates how using the strict equality operator resolves these issues.
