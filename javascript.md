# Javascript

1. **hoisting, let, var, const** (**Junior**)
    - Hoisting is default's Js behavior move all declarations to the top
    - With var declaration you can use variable before declare.The variable will be out of scope and have undefined value
    - with let, const declarations you can use variables before declare and variable will not out of scope

2. **Closure** (**Junior**)
    - Basically. Closure present a Function return function and function children can access variables of parent function.

3. **Promise** (**Junior**)
    Promise is a proxy value help you handle asynchronous function like synchronous.
    Promise have 3 state:
    **Pending**: when initial state
    **fulfilled**: when operation completed
    **rejected**: when operation failed.

4. **Promise.all** vs **Promise.allSettled** (**Pre-Senior**)
    Both use for handle many promise at same time but 
    with **Promise.all** if 1 of promises reject => all reject
    **Promise.allSettled** if 1 of promises reject => still run and return res.

5. **Optimize in javascript** (**Senior**)
    - cache, split code, use continue and break in loop, clear timeout interval, not use global variable

6. **Event loop, call stack, queue** (**Senior**)
    - **Call stack**: is data structure that keeps track of the order in which functions are called When a function is called, it is added to the top of the call stack, and when it returns, it is removed from the stack.
    - **Event loop**: a mechanism that allows JavaScript to handle asynchronous operations, such as network requests or user input, without blocking the main thread. The event loop constantly checks the queue for any tasks that need to be executed, and when it finds one, it adds it to the call stack.
    - **Queue** is a data structure that holds tasks that need to be executed by the event loop. When a task is added to the **queue**, it is not executed immediately, but instead waits for the event loop to process it.
    
7. '**this**' in javascript (**Senior**)
     The "**this**" keyword refers to the object that the current code is being executed in.
     In JavaScript, "context" usually refers to the value of the "this" keyword within a particular function or code block. The value of "**this**" can change depending on how the function is called or where the code is being executed.
     If you use arrow function **this** will be out of context but instead inherit the "**this**" value from the enclosing scope.
     
8. **What is the difference between synchronous and asynchronous code in JavaScript?**
    Answer: Synchronous code is executed in a single thread and blocks the execution until it is complete, while asynchronous code is executed in a separate thread and does not block the execution.

9. **map(), filter(), reduce()**
    - The **map()** method creates a new array by applying a function to each element of an existing array. The function takes in the current element of the array as an argument and returns a new value. The new value is then added to the new array. The map() method does not modify the original array.
    - The **filter**() method creates a new array with all elements that pass a certain test. The test is specified by a function that takes in the current element of the array as an argument and returns a boolean value. If the function returns true, the element is added to the new array. If the function returns false, the element is not added to the new array. The **filter**() method does not modify the original array.
    - The **reduce()** method reduces an array to a single value by applying a function to each element of the array. The function takes in two arguments: an accumulator and the current element of the array. The accumulator is the value that is returned by the function and is passed on to the next iteration of the function. The **reduce()** method can be used to perform various operations on an array, such as summing up all the elements or finding the maximum value. The **reduce()** method does not modify the original array.
    - 
10. **What is the difference between a shallow copy and a deep copy in JavaScript?**
    Answer: A shallow copy creates a new object that references the same values as the original object, while a deep copy creates a new object with new values that are not shared with the original object.





