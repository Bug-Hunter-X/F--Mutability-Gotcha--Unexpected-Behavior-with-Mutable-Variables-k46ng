# F# Mutability Gotcha: Unexpected Behavior with Mutable Variables

This example demonstrates a potential issue with mutable variables in F#.  When a function uses mutable variables, modifying those variables *after* the function's initial call can lead to unexpected results if the function isn't designed to handle this mutability. 

The `bug.fs` file contains code showcasing this unexpected behavior. The solution (`bugSolution.fs`) demonstrates a way to handle the situation correctly by either passing in new values directly, or by using immutable values. 