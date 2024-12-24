# Kotlin `removeIf` Unexpected Behavior
This example demonstrates an uncommon issue related to modifying a list while iterating over it using the `removeIf` function in Kotlin.  The `removeIf` function removes elements from a mutable list based on a predicate.  However, if the predicate modifies the list's structure during iteration, unexpected results can occur.  This example shows how skipping elements due to the modifications can lead to incorrect outputs.

## How to Reproduce
Run the `bug.kt` file to observe the unexpected behavior. The solution demonstrates a safe approach using an iterator.

## Solution
The solution file `bugSolution.kt` provides a corrected approach to safely remove elements from the list using an iterator, avoiding the concurrent modification issue.