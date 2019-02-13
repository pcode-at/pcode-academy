# Functional Programming
Functional programming is an important concept that you have to understand if you want to be a great JavaScript developer.

## Resources
### Pure Functions
Pure functions are simple but very useful. They are predictable and therefore very easy to test. It is very important that you have as many logic as possible in pure functions. With them, your code will be simple to understand and bug resistant. The main characteristic of a pure function is that it has no side effects. Read this [article](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976).

### Function Composition
With function composition, your code gets more readable. You reduce the using of variables which exist only to hold transient values between one operation and the next. We learned this technique from this [article](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-function-composition-20dfb109a1a0). [The Dao of Immutability](https://medium.com/javascript-scene/the-dao-of-immutability-9f91a70c88cd) is also a very nice read.

### Core concept
If you have finished reading the articles of the two topics above you are a ready for [Master the JavaScript Interview: What is Functional Programming?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0).


## Comments
In the mentioned articles above you often will find the function [`Object.assign()`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/assign). Instead of using this syntax we now use the new [spread operator](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/Spread_operator) that comes with ES6. [Replace](https://redux.js.org/recipes/using-object-spread-operator) one syntax with the other is really easy.
