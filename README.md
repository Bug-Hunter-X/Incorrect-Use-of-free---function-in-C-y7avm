# Incorrect Use of free() in C
This repository demonstrates a common error in C programming: attempting to free memory allocated on the stack using the `free()` function.  The `free()` function is intended for dynamically allocated memory using `malloc()`, `calloc()`, or similar functions. Using it on stack-allocated variables can lead to crashes or unpredictable behavior.

The `bug.c` file shows the erroneous code. The `bugSolution.c` provides the correct approach, which involves no explicit call to `free()` since stack memory is automatically managed.