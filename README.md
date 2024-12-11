# Tcl Proc Return Value Bug
This example demonstrates a common error in Tcl where the return value of a procedure is not handled correctly.  The `badproc` procedure is intended to return 1, but the calling code doesn't use the result.

## Bug
The issue lies in how the `badproc` procedure is called. The return value of 1 is ignored; therefore, the return value is never used. The `puts` statement is executed correctly; however, this does not impact the program's logic.

## Solution
The solution involves properly capturing and utilizing the return value from `badproc`. In this case, we demonstrate how to handle the return value with a `if` statement to ensure it's effectively used.