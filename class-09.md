# Read: 09 - Refactoring

## Master the JavaScript Interview: What is Functional Programming?

- Functional programming
  - the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.
  - declarative rather than imperative, and application state flows through pure functions.
- Functional programming is a programming paradigm, meaning that it is a way of thinking about software construction based on some fundamental, defining principles.
- Core concepts of functional programming
  - Pure functions
    - A function which:
      - Given the same inputs, always returns the same output
      - Has no side-effects
    - **Referential transparency** - you can replace a function call with its resulting value without changing the meaning of the program
  - Function composition
    - the process of combining two or more functions in order to produce a new function or perform some computation.
  - Avoid shared state
    - Shared state - any variable, object, or memory space that exists in a shared scope, or as the property of an object being passed between scopes.
    - Problems with shared state:
    - “Race condition”
    - Functions in shared state are timing dependent
  - Avoid mutating state
    - Immutable object
      - An object that can’t be modified after it’s created.
    - **Trie data structures** - (pronounced “tree”) which are effectively deep frozen — meaning that no property can change, regardless of the level of the property in the object hierarchy.
    - Tries use **structural sharing** to share reference memory locations for all the parts of the object which are unchanged after an object has been copied by an operator, which uses less memory, and enables significant performance improvements for some kinds of operations.
  - Avoid side effects
    - any application state change that is observable outside the called function other than its return value.
    - If you keep your side effects separate from the rest of your program logic, your software will be much easier to extend, refactor, debug, test, and maintain.
    - A **higher order function** is any function which takes a function as an argument, returns a function, or both.
- Declarative vs Imperative
  - **Imperative programs** spend lines of code describing the specific steps used to achieve the desired results — the flow control: How to do things.
  - **Declarative programs** abstract the flow control process, and instead spend lines of code describing the data flow: What to do. The how gets abstracted away.

## Refactoring Javascript for Readability

- A hash function is used to map a given key to a location in the hash table.
- Methods that lead to easier to read code
  - Return early from functions
  - Cache variables so functions can be read like sentences
  - Check for Web APIs before implementing your own functionality

[Back to README](README.md)
