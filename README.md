# cmm-test

This is a test set for c-- compiler, the Programming Assignment of Principles of Compilers at Nanjing University.

This test set is distributed in the hope that it will be useful, but without any warranty. Pull requests are always welcome.

# Implementation Specification

The test set assumes the implementation follows the specification below :

- C/C++ style comments should be supported.
- Implementations can optimize the output code according to the "as-if" rule; that is, implementations are free to change the output as long as it does not change the observable behaviors of the output program. This overrides all following rules.
- Logical operation (&&, ||, !) evaluates to 1 if the value is true, or 0 if false.
- Logical AND (&&) / OR(||) are evaluated in short-circuit style.
- All expressions within a statement are evaluated in *LEFT-TO-RIGHT* order. This includes operands in binary operations and function parameters. All expressions *MUST* be evaluated even if the value is discarded, with one exception that the expression skipped in short-circuited evaluation *MUST NOT* be evaluated.
- Unlike C/C++, when function parameter is of array type, the array has full value semantics and thus the entire array is passed by value.
