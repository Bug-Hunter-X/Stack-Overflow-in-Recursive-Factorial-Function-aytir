# Stack Overflow in Recursive Factorial Function
This repository demonstrates a common error in recursive functions: stack overflow.  The `bug.hack` file contains a recursive factorial function that will crash for larger inputs due to exceeding the maximum recursion depth.  The `bugSolution.hack` file provides a corrected, iterative version of the factorial function.

## How to reproduce
1. Clone this repository.
2. Compile and run `bug.hack` with a large input (e.g., 1000). You'll observe a stack overflow error.
3. Compile and run `bugSolution.hack`. This will calculate the factorial correctly even for large numbers.

## Solution
The problem with the recursive approach is that each recursive call adds a new stack frame. For large inputs, this leads to a stack overflow. The solution uses iteration to avoid unbounded recursion. 