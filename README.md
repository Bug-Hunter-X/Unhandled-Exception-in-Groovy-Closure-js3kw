# Unhandled Exception in Groovy Closure

This repository demonstrates a common issue in Groovy where an exception thrown within a closure is not properly handled by the surrounding method.  The `bug.groovy` file showcases this problem, while `bugSolution.groovy` provides a corrected version.

The problem arises because the exception thrown inside the closure propagates up the call stack and is not caught by `methodWithClosure`.

The solution involves adding a `try-catch` block within `methodWithClosure` to handle potential exceptions from the closure.