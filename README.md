![CF](http://i.imgur.com/7v5ASc8.png) LAB-36
=================================================

## Remote CRUD

### Author: Vanessa

### Links and Resources
* [part one](https://codesandbox.io/s/j6qkn33qw)
* [part two](https://codesandbox.io/s/p5wqx064jj)

### Assignment 1 - Counter
* Create a Counter Provider component, which exposes the following state:
  * `count` - A number (default to 0)
  * `increment` - A reference to a function that increases the count
  * `decrement` - A reference to a function that decreases the count
* In the index.js, import CounterContext and wrap `<App />` in it, so that all child components can optionally subscribe to it as consumers.
* Your `<App />` component should simply pull in and render the following child components ...
* Create the following child components that register as a `.Consumer` to the provided context.
  * `<Incrementer />` - Renders a button that, when clicked, calls the `increment()` method in the `Counter Provider`
  * `<Decrementer />` - Renders a button that, when clicked, calls the `decrement()` method in the `Counter Provider`
  * `<Counter />` - Renders the current value of `count` from the Counter Provider
* Provide good styling. Use the css-in-js methodology within the components themselves.

## Assignment 2 - To Do
You have been provided, in the `starter-code` folder, a working To Do manager application, written using standard React Component State

* Refactor the app to make use of Context
* Create a `context` for the Application
* Create a separate `<Counter />` component that reads and displays the `count` from Context
* Create separate components for the main To App elements
  * `form` - Adds and updates to do list items
  * `list` - Lists items, manages complete state and form visibility
  
### Setup
#### `.env` requirements
* `npm i` install dependencies

#### Running the app
* open sandbox link

### Components
```
├── LAB.md
├── README.md
├── package.json
├── public
│   └── index.html
└── src
    ├── __tests__
    │   └── components
    │       └── app.test.js
    ├── components
    │   ├── api.js
    │   ├── app.js
    │   └── record
    │       ├── actions.js
    │       ├── if.js
    │       ├── list.js
    │       ├── record.js
    │       ├── record.module.scss
    │       └── reducers.js
    ├── index.js
    ├── setupTests.js
    └── store
        ├── index.js
        └── middleware
            └── reporter.js
```


#### UML
![Data flow](./uml.jpg)
