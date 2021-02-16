---
title: React (JavaScript library)
date: "2021-01-01T00:00:00.000Z"
description: "React (also known as React.js or ReactJS) is an open-source, front end, JavaScript library[3] for building user interfaces or UI components."
---

React (also known as React.js or ReactJS) is an open-source, front end, JavaScript library[3] for building user interfaces or UI components. It is maintained by Facebook and a community of individual developers and companies.[4][5][6] React can be used as a base in the development of single-page or mobile applications. However, React is only concerned with state management and rendering that state to the DOM, so creating React applications usually requires the use of additional libraries for routing,[7][8] and fully-fledged form solutions.[9] React Router[10] and Formik[11] are examples of such libraries respectively.

Basic usage

The following is a rudimentary example of React usage in HTML with JSX and JavaScript.

The Greeter function is a React component that accepts a property greeting. The variable App is an instance of the Greeter component where the greeting property is set to 'Hello World!'. The ReactDOM.render method then renders our Greeter component inside the DOM element with id myReactApp.

When displayed in a web browser the result will be

Notable features
Components

React code is made of entities called components. Components can be rendered to a particular element in the DOM using the React DOM library. When rendering a component, one can pass in values that are known as "props":[12]

The two primary ways of declaring components in React is via functional components and class-based components.
Functional components

Functional components are declared with a function that then returns some JSX.

Class-based components

Virtual DOM

Another notable feature is the use of a virtual Document Object Model, or virtual DOM. React creates an in-memory data-structure cache, computes the resulting differences, and then updates the browser's displayed DOM efficiently.[13] This process is called reconciliation. This allows the programmer to write code as if the entire page is rendered on each change, while the React libraries only render subcomponents that actually change. This selective rendering provides a major performance boost.[citation needed] It saves the effort of recalculating the CSS style, layout for the page and rendering for the entire page.[citation needed]

Lifecycle methods

Lifecycle methods use a form of hooking that allows the execution of code at set points during a component's lifetime.

    shouldComponentUpdate allows the developer to prevent unnecessary re-rendering of a component by returning false if a render is not required.
    componentDidMount is called once the component has "mounted" (the component has been created in the user interface, often by associating it with a DOM node). This is commonly used to trigger data loading from a remote source via an API.
    componentWillUnmount is called immediately before the component is torn down or "unmounted". This is commonly used to clear resource-demanding dependencies to the component that will not simply be removed with the unmounting of the component (e.g., removing any setInterval() instances that are related to the component, or an "eventListener" set on the "document" because of the presence of the component)
    render is the most important lifecycle method and the only required one in any component. It is usually called every time the component's state is updated, which should be reflected in the user interface.
