# Call Stack and Debugging

### Call Stack
> The "call stack" refers to a place in memory where an interpreter can store its position inside functions while fetching the values of other function returns. As functions invoke other functions they are progressively "stacked" on top of each other. If the call stack exceeds its alloted space it will result in a stack overflow.

The call stack is single threaded and function executions can only occur one at a time. These events follow a last in, first out principle.

### Errors

1. Reference Errors: Typically use of a variable before it is declared or improper use of let/const
2. Sytax Errors: An error in the syntax of your code itself
3. Range Errors: Manipulating an obect with an invalid iterator length
4. Type Errors: Data types are incompatible in some way

## References
[Call Stack](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

[Errors](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)