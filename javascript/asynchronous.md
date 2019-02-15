# Asynchronous code
JavaScript is a single-threaded programming language. Considering this it is very important that you understand the behavior of asynchronous code.
There are three important techniques for writing asynchronous code in JavaScript:
* Callbacks
* Promises
* Async / Await


## Resources
For understanding asynchronous JavaScript in general read [Understanding Asynchronous JavaScript
](https://blog.bitsrc.io/understanding-asynchronous-javascript-the-event-loop-74cd408419ff).

### Callbacks
A callback is a function that is to be executed after another function has finished executing. Read [JavaScript: What the heck is a Callback?](https://codeburst.io/javascript-what-the-heck-is-a-callback-aba4da2deced).

### Promises
For understanding [promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) read [A Simple Guide to ES6 Promises](https://codeburst.io/a-simple-guide-to-es6-promises-d71bacd2e13a). For more information about promises and good practices read [Master the JavaScript Interview: What is a Promise?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261). It is important that you know the prototype methods [`.then`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/then), [`.catch`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/catch) and the functions available from Promise: [`Promise.all`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all) and [`Promise.race`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/race).

### Async / Await
The article [How to escape async/await hell](https://medium.freecodecamp.org/avoiding-the-async-await-hell-c77a0fb71c4c) points out the correct usage of async/await and how you can avoid common pitfalls.
