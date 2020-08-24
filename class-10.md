# Read: 10 - The Call Stack and Debugging

## The Call Stack defined on MDN

- Call stack
  - A mechanism for an interpreter to keep track of its place in a script that calls multiple functions - what function is currently being run and what functions are called from within that function, etc.
- Process
  1. We start with an empty Call Stack.
  2. Whenever we invoke a function, it is automatically added to the Call Stack.
  3. Once the function has executed all of its code, it is automatically removed from the Call Stack.
  4. Ultimately, the Stack is empty again.

## Understanding the JavaScript Call Stack

- The call stack is primarily used for function invocation (call)
  - Since the call stack is single, function(s) execution is done, one at a time, from top to bottom.
- **Call stack** is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).
- **LIFO** - the last function that gets pushed into the stack is the first to pop out, when the function returns.
- **Temporarily store**
  - When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.
- **Manage function invocation**
  - The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.
    - Think of yourself standing on a queue, in a grocery store cash point. You can only be attended to after the person in front of you have been attended to. That’s synchronous.
- The cause of stack overflow
  - A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error. Example below

```
function callMyself(){
  callMyself();
}
callMyself();
```

- The key takeaways from the call stack are:
  - It is single-threaded. Meaning it can only do one thing at a time.
  - Code execution is synchronous.
  - A function invocation creates a stack frame that occupies a temporary memory.
  - It works as a LIFO — Last In, First Out data structure.

## JavaScript error messages

![Example of Errors](img/error.PNG)

- Different types of errors
  - Reference error
    - ```foo = 'Hello' // Uncaught ReferenceError: foo is not defined let foo```
  - Syntax error
    - ```JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1```
  - Range error
    - Manipulate an object with some kind of length and give it an invalid length
  - Type error
    - Accessing a property in an undefined type of variable.
- Debugging
  - Console.log();
  - Debugger;
- Adding names to your functions whenever possible so that the call stack is more readable without having to dive into each step.
- When we do not handle errors properly, meaning that anything after that error will not be executed.
  - To avoid this we usually try to catch the errors so we can gracefully fallback to a default state of our application in case of an error.
- Before a commit/push, remove all the debugging stuff from your code.

[Back to README](README.md)
