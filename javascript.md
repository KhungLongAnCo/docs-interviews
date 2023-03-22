# Interview question

1. hoisting, let, var, const
    - Hoisting is default's Js behavior move all declarations to the top
    - With var declaration you can use variable before declare.The variable will be out of scope and have undefined value
    - with let, const declarations you can use variables before declare and variable will not out of scope

2. Closure
    - Basically. Closure present a Function return function and function children can access variables of parent function.

3. Promise
    Promise is a proxy value help you handle asynchronous function like synchronous.
    Promise have 3 state:
    Pending: when initial state
    fulfilled: when operation completed
    rejected: when operation failed.

4. Promise.all vs Promise.allSettled
    Both use for handle many promise at same time but 
    with Promise.all if 1 of promises reject => all reject
    Promise.allSettled if 1 of promises reject => still run and return res.

5. Optimize in javascript
    - cache, split code, use continue and break in loop, clear timeout interval, not use global variable

6. Event loop, call stack, queue

    

