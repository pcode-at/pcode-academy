
# Closures
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

This will lead to this output: `example increment 1 2 3`, but why? Maybe you say now that is just common sense or it must result in this output. Closures are the reason for this behavior in JavaScript and it is important that you understand this concept.


## Resources
I strongly recommend reading the article [I never understood JavaScript closures](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8). It explains closures very nicely. If you want to read more there is also the article [Master the JavaScript Interview: What is a Closure?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36) from Eric Elliott.
