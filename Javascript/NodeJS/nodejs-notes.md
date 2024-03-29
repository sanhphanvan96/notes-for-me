
### npm install -g gulp bower nodemon
### bower install --save bootstrap-css
1. **Gulp** is a task runner which we will use to make our like easier with some
automation for mundane workflow tasks
2. **Bower** is a package manager for various front end libraries like bootstrap, jquery etc. this is just a nicer way of installing these libraries in your app as opposed to downloading them manually.
3. **Nodemon** to automatically restart our server application whenever a code change happens.

### npm install gulp-inject --save-dev
### npm install --save browserify reactify vinyl-source-stream gulp react react-dom express guid
1. **browserify**: we can use node like CommonJs module pattern to add references to various libraries as opposed to adding script tags in html pages.
2. **reactify** is there to transpile JSX to javascript. JSX is xml like JavaScript syntax which react usage, you will understand exactly what I am saying once you have written some JSX code.


## Create New App:
1. mkdir school-finder
2. npm init
3. bower init

# React Flux Architecture
You must be thinking if we are going to build a whole application which is non trivial in nature with all these components, how far will I go? where will I place event handlers, all the **REST API** calls? How my application's architecture should look like? Well there is one answer to your all questions **React Flux Architecture**.

**React flux** is a programming patters for react applications which facebook usage internally. Flux ensures only unidirectional data flow throughout your application life cycle. Flux has following agents which keep the flux flow ticking:

1. **Actions**: these are the payloads with some data and some context (type) in short objects, these are created by some helper functions as a result of an activity in the view(mostly). For example when user clicks on an add button, we will create an action which will contain infomation to be added and the context. All actions are sent to the dispacher.

2. **Dispatcher**: dispatcher works like a global hub which triggers all the listeners rgistered to it whenever an action is sent to it.

3. **Stores**: stores register themselves with dispatchers, when dispatcher broadcasts an actions arrival, stores update themselves if that action is relavant to those stores, and emit a change event which causes UI to get updated.

4. **Views**: Views are the html rendered components.
------

# 10 JavaScript concepts you need to know: [Here](https://docs.google.com/document/d/1lGPcHJPUr1R6N2yMtTws94_BjTU7AP_LkkJysI-4T1I/edit#)

1. **Value vs. Reference** — Understand how objects, arrays, and functions are copied and passed into functions. Know that the reference is what’s being copied. Understand that primitives are copied and passed by copying the value.
2. **Closures** — Know that a function retains access to the scope that it was created in. Know what this lets us do, such as data hiding, memoization, and dynamic function generation.
3. **this** — Know the rules of this binding. Know how it works, know how to figure out what it will be equal to in a function, and know why it’s useful.
4. **new** — Know how it relates to object oriented programming. Know what happens to a function called with new. Understand how the object generated by using new inherits from the function’s prototype property.
5. **Prototypes & Inheritance** — Understand that inheritance in JavaScript works through the [[Prototype]] chain. Understand how to set up inheritance through functions and objects and how new helps us implement it. Know what the __proto__ and prototype properties are and what they do.
6. **Asynchronous JS** — Understand the event loop. Understand how the browser deals with user input, web requests, and events in general. Know how to recognize and correctly implement asynchronous code. Understand how JavaScript is both asynchronous and single-threaded.
7. **Higher Order Functions** — Understand that functions are first-class objects in JavaScript and what that means. Know that returning a function from another function is perfectly legal. Understand the techniques that closures and higher order functions allow us to use.
8. **apply, call, bind** — Know how each of these functions work. Know how to use them. Know what they do to this.
9. **Scope** — Understand the difference between global scope, function scope, and block scope. Understand which variables are available where. Know how the JavaScript engine performs variable lookup.
10. **Hoisting** — Understand that variable and function declarations are hoisted to the top of their available scope. Understand that function expressions are not hoisted.
------
