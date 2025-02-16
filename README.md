# Lua Nil Arithmetic Bug

This repository demonstrates a subtle bug related to how Lua handles `nil` values in arithmetic expressions and conditional statements.

The `foo` function attempts to add two numbers, but it doesn't explicitly handle cases where either `a` or `b` is `nil`.  Lua's implicit type coercion can produce unexpected `nil` results when performing arithmetic operations that involve `nil` operands.

The solution shows how to improve the function to handle `nil` values gracefully, ensuring that the function returns the expected result in all cases.

## Bug

The `bug.lua` file contains the buggy version of the code.

## Solution

The `bugSolution.lua` file provides the corrected version of the function that addresses the `nil` handling issue.