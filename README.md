# Unhandled Non-numeric Input in Julia Function

This repository demonstrates a common error in Julia: failing to handle non-numeric input to functions. The `bug.jl` file contains a function that works correctly for numbers but throws an error if given a string or other non-numeric type. The solution in `bugSolution.jl` shows how to address this using type checking and error handling.

## Bug Description
The original function `myfunction` only checks if `x` is greater than 0. It doesn't check if the input `x` is actually a number. If you pass a string or other incompatible type to this function, it will throw a `MethodError`. 

## Solution
The solution incorporates a `try-catch` block to handle potential errors and checks the type of the input using `isa`.  This improved function provides a more robust and reliable way to deal with unexpected input.