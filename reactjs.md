# React JS

1. Life circle (**Beginner**)
    - **Mounting** : Mounting means putting elements into the DOM
        > constructor()
        > getDerivedStateFromProps()
        > render()
        > componentDidMount()
    - **Updating**: The next phase in the lifecycle is when a component is updated.
        > getDerivedStateFromProps()
        > shouldComponentUpdate()
        > render()
        > getSnapshotBeforeUpdate()
        > componentDidUpdate()
    - **Unmounting**: The next phase in the lifecycle is when a component is removed from the DOM
        > componentWillUnmount()

3. **Error Boundaries** (**Senior**)
    - A react component that catch JavaScript errors anywhere in their child component tree, log those errors, and display a fallback UI instead of the component tree that crashed

4. **Reconciliation** (**Senior**)
    - **Reconciliation** is process by which React updates the UI to reflect changes in the component state
    The reconciliation algorithm is the set of rules that React uses to determine how to update the UI in the most efficient way possible. React uses a virtual DOM (Document Object Model) to update the UI
    - **The Diffing Algorithm**: React compares the virtual copy of Real DOM to an updated Copy of Virtual DOM, compares or picks out the changes, and finally renders it to real Dom.
    Content of Elements > Quantity of Elements > Tag name > Attributes > Style
5. **Optimize**
    There are many ways to optimization in react:
    - useMemo, useCallback
    - Code-Splitting: use lazy loading.
2. **useMemo, useCallback** (**Junior**)
    - **useMemo**: Allow pass function and dependencies. useMemo will only recompute memoized value when one of the dependencies has changed
    - **useCallback**: Allow pass function and dependencies. useCallback will only update function version memoized when one of the dependencies has changed
    -  Both use for memoized value. But one for memorized function one for memoized value computed

6. **Code-Splitting** (**Senior**)
   - a feature supported by bundlers like Webpack, Rollup and Browserify (via factor-bundle) which can create multiple bundles that can be dynamically loaded at runtime,
   **Code-splitting** your app can help you “lazy-load” just the things that are currently needed by the user
7. **What is JSX?**
     JSX is a syntax extension for JavaScript that allows developers to write HTML-like code in their JavaScript files.

8. **What is the difference between a higher-order component (HOC) and a render prop in React?**
Answer: A higher-order component is a function that takes a component and returns a new component with additional functionality, while a render prop is a function that is passed as a prop to a component and returns a React element.

9. **useContext, Consumer, provider in react**
    In React, the useContext() hook, Consumer, and Provider are all related to the Context API, which provides a way to share data between components without having to pass props down the component tree manually at every level.
    - The **useContext()** hook is used to access the context of a parent component from a child component without having to pass props down the component tree. It takes a context object created by the createContext() function and returns the current value of the context.
    - The **Consumer** component is another way to access the context in a child component. It takes a function as a child and passes the current value of the context to that function as an argument.
    - The **Provider** component is used to provide the context to the child components. It takes a value prop that represents the current value of the context.

10. **What is the difference between a functional component and a class component in React?**
    A functional component is a simpler and more lightweight way of creating a component in React, while a class component is a more powerful and flexible way of creating a component.
    - Functional components are defined as JavaScript functions that take in props as an argument and return a React element. They are stateless and do not have access to lifecycle methods or the this keyword. They are also easier to read, test, and maintain than class components.
    - Class components, on the other hand, are defined as JavaScript classes that extend the React.Component class. They have access to lifecycle methods, state, and the this keyword. They are more powerful and flexible than functional components, but also more complex and harder to read.

11. **What is the virtual DOM in React?**
    The virtual DOM (VDOM) is a lightweight copy of the actual DOM that React uses to keep track of changes and update the UI efficiently. The VDOM is a JavaScript object that represents the structure of the actual DOM, and it is updated whenever there is a change in the state or props of a component.
    * Here's an example of how the VDOM works in React:

    - A user clicks a button, triggering a change in the state of a component.
    - React updates the VDOM to reflect the new state of the component.
    - React compares the new VDOM to the previous VDOM to determine what has changed.
    - React updates only the parts of the actual DOM that have changed, such as adding or removing a DOM element or updating the text content of a DOM element.


12. **What is the purpose of the key prop in React?**
    Answer: The key prop is used to help React identify which items in a list have changed, been added, or been removed.

13. **What is the purpose of the memo() function in React?**
    Answer: The memo() function is used to memoize a component and prevent unnecessary re-renders of the component.

14. **What is the difference between server-side rendering and client-side rendering in React?**
    Answer: Server-side rendering is the process of rendering a React component on the server and sending the HTML to the client, while client-side rendering is the process of rendering a React component in the browser using JavaScript.
