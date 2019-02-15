# Functional Programming
Functional programming is an important programming paradigm. It lets you write more declarative code that makes your code easier to read and understand. Functional programming exists not only in JavaScript but also in a lot of other programming languages too. Read [Master the JavaScript Interview: What is Functional Programming?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0) for an introduction and then work through the sections below.

## Resources
### Pure Functions
Pure functions are simple but very useful. They are predictable and therefore very easy to test. It is very important that you have as many logic as possible in pure functions. With them, your code will be simple to understand and bug resistant. The main characteristic of a pure function is that it has no side effects. Read [Master the JavaScript Interview: What is a Pure Function?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)

### Higher Order Functions
A higher order function is a function that takes a function as an argument or returns a function. This is stated in the article [Higher Order Functions (Composing Software)](https://medium.com/javascript-scene/higher-order-functions-composing-software-5365cf2cbe99) from Eric Elliott.

### Closures
A [closure](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures) is the combination of a function and the lexical environment within which that function was declared.

Considering this code example([source](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8)):


```
function createCounter() {
  let counter = 0;
  const myFunction = function() {
      counter = counter + 1;
      return counter;
    }
    return myFunction;
 }
 const increment = createCounter();
 const c1 = increment();
 const c2 = increment();
 const c3 = increment();
 console.log('example increment', c1, c2, c3);
```

This will lead to this output: `example increment 1 2 3`, but why? Maybe you say that this is just common sense or it must result in this output. Closures are the reason for this behavior and it is important that you understand this concept.

Read these articles:
* [I never understood JavaScript closures](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8) - a very good explanation
* [Master the JavaScript Interview: What is a Closure?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36) - if you want to read more about the topic in a more advanced way from Eric Elliott


### Function Composition
With function composition, your code gets more readable. You reduce the using of variables which exist only to hold transient values between one operation and the next. 

Read these articles:
* [Master the JavaScript Interview: What is Function Composition?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-function-composition-20dfb109a1a0)
* [A quick introduction to pipe() and compose() in JavaScript](https://medium.freecodecamp.org/pipe-and-compose-in-javascript-5b04004ac937) - composition tools `pipe()` and `compose()`
* [Curry and Function Composition](https://medium.com/javascript-scene/curry-and-function-composition-2c208d774983) - learn how to currying functions

### Immutability
Immutability is a very important aspect of functional programming. After you read [
Immutable Javascript using ES6 and beyond](https://wecodetheweb.com/2016/02/12/immutable-javascript-using-es6-and-beyond/) you should know how to write immutable JavaScript code and why it is so important. [The Dao of Immutability](https://medium.com/javascript-scene/the-dao-of-immutability-9f91a70c88cd) is also a very nice read.

### .map(), .reduce() and .filter()
In the article above you often read about [.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map), [.reduce()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce) and [.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter). Despite they are pure functions, they are very useful and help you write more declarative code. For a better understanding when and how you should use them read [Simplify your JavaScript – Use .map(), .reduce(), and .filter()](https://medium.com/poka-techblog/simplify-your-javascript-use-map-reduce-and-filter-bd02c593cc2d).

**Important:** Not all of the JavaScript Array [methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype#Methods) are considered to be pure functions! Some of them mutate the Array they get called on. Be aware of that when using them.

## Comments
In the mentioned articles above you often will find the function [`Object.assign()`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/assign). Instead of using this syntax we now use the new [spread operator](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/Spread_operator) that comes with ES6. [Replace](https://redux.js.org/recipes/using-object-spread-operator) one syntax with the other is really easy.

### Function Composition
In the article [A quick introduction to pipe() and compose() in JavaScript](https://medium.freecodecamp.org/pipe-and-compose-in-javascript-5b04004ac937) the author writes about the library [ramda](https://ramdajs.com/). This is also the functional programming library that we use for our projects at PCode.

### map(), .reduce() and .filter()
In the article [Simplify your JavaScript – Use .map(), .reduce(), and .filter()](https://medium.com/poka-techblog/simplify-your-javascript-use-map-reduce-and-filter-bd02c593cc2d) the author writes about how he could possibly do everything with the .reduce() function. Why is that not that clean? The answer is it is not a declarative code then. The function 'does too much'. A much better solution is to split (how he did it in the article) the code in three parts(functions) and then use [function composition](#function-composition). Always think of [SRP](https://de.wikipedia.org/wiki/Single-Responsibility-Prinzip).

## PCode Clean Code Adventure
In our [functional programming adventure](https://github.com/pcode-at/clean-code-adventure/tree/module/functional-programming/src/pcode-academy/javascript/functional-programming), you will get in touch with all the things mentioned above. You will write pure, declarative functions with .map(), .reduce() and .filter() and then compose them with a pipe to a new, highly meaningful function.

**Tip:** After you run `yarn test` press `p`in the console to filter the tests with 'functionalProgramming.test' or something short like 'funct' to run only relevant tests.
