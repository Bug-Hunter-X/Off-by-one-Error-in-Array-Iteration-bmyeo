# Off-by-One Error in Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over an array. The error occurs when the loop condition allows access to an index that is out of bounds, leading to an `ArrayIndexOutOfBoundsException`.

## Bug Description
The provided Java code iterates through an integer array. However, the loop condition `i <= arr.length` is incorrect.  Arrays are zero-indexed; therefore, the valid index range is 0 to `arr.length - 1`. Accessing `arr[arr.length]` results in an exception.

## Solution
The solution modifies the loop condition to `i < arr.length`, ensuring that the loop terminates before accessing an invalid index.