# Functional Programming
Functional programming is an important concept that you have to understand if you want to be a great JavaScript developer.

## Resources
### Pure Functions
Pure functions are simple but very useful. They are predictable and therefore very easy to test. It is very important that you have as many logic as possible in pure functions. With them, your code will be simple to understand and bug resistant. The main characteristic of a pure function is that it has no side effects. Read [Master the JavaScript Interview: What is a Pure Function?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976).

### Function Composition
With function composition, your code gets more readable. You reduce the using of variables which exist only to hold transient values between one operation and the next. We learned this technique from [Master the JavaScript Interview: What is Function Composition?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-function-composition-20dfb109a1a0). [The Dao of Immutability](https://medium.com/javascript-scene/the-dao-of-immutability-9f91a70c88cd) is also a very nice read.

### Core concept
If you have finished reading the articles of the two topics above you are a ready for the [Master the JavaScript Interview: What is Functional Programming?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0).

### .map(), .reduce() and .filter()
In the article above you often read about [.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map), [.reduce()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce) and [.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter). They are very useful and help you write more declarative code. For a better understanding when and how you should use them read [Simplify your JavaScript – Use .map(), .reduce(), and .filter()](https://medium.com/poka-techblog/simplify-your-javascript-use-map-reduce-and-filter-bd02c593cc2d). Check out all available [methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype#Methods) for Arrays in JavaScript.

## Comments
In the mentioned articles above you often will find the function [`Object.assign()`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/assign). Instead of using this syntax we now use the new [spread operator](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/Spread_operator) that comes with ES6. [Replace](https://redux.js.org/recipes/using-object-spread-operator) one syntax with the other is really easy.

### map(), .reduce() and .filter()
In the article [Simplify your JavaScript – Use .map(), .reduce(), and .filter()](https://medium.com/poka-techblog/simplify-your-javascript-use-map-reduce-and-filter-bd02c593cc2d) the author writes about how he could possibly do everything with the .reduce() function. Why is that not that clean? The answer is it is not a declarative code then. The function 'does too much'. A much better solution is to split (how he did it in the article) the code in three parts(functions) and then use [function composition](#function-composition). Always think of [SRP](https://de.wikipedia.org/wiki/Single-Responsibility-Prinzip).
