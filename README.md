# Off-by-One Error in C Array Access

This repository demonstrates a common off-by-one error in C when accessing array elements. The bug involves iterating beyond the valid index range of an array, which can cause unpredictable behavior or program crashes.

## Bug Description
The provided C code attempts to print the elements of an integer array. However, the loop condition `i <= 5` is incorrect.  The valid indices for a 5-element array are 0 to 4. Accessing `arr[5]` is out of bounds, leading to undefined behavior.  This might result in accessing memory that doesn't belong to the array, causing a crash or unexpected output.

## Solution
The corrected code adjusts the loop condition to `i < 5` ensuring that the loop iterates only within the valid bounds of the array.