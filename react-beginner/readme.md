# React-beginner module

## Introduction
In this module of the PCode Academy you will get a solid understanding of React.js. After this module you are able to create your own application written in JavaScript with React.js.

## Course
Here is the link to the online course: https://courses.wesbos.com/account/access/5c58437885f96c03c1e313d8

## Comments

### Video #8
We always starting a component as a stateless functional component. At the time we need lifecycle methods we change it to a class component. You can read more about these two component types [here](https://programmingwithmosh.com/react/react-functional-components/). 

### Video #13
This video is all about data handling and the state of components in React. It is important that you understand the unidirectional data flow and the problems that came with it. In this [article](https://medium.com/dailyjs/when-do-i-know-im-ready-for-redux-f34da253c85f) you will get a nice, visual explanation and a glimpse into the state-management library [Redux](https://redux.js.org/).

#### 22:00
Here you will see how you can update the state. The course instructor also mentions the word 'immutable'. It is important that when you update the state you follow these [immutable update patterns](https://redux.js.org/recipes/structuring-reducers/immutable-update-patterns). In this [article](https://wecodetheweb.com/2016/02/12/immutable-javascript-using-es6-and-beyond/) you will learn more about why writing immutable JavaScript code is a good practice.

### Video #15
#### 04:00
It shows very well the usage of the function [Object.keys](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/keys) but in my opinion in this case an Array would have been the better choice for storing the fishes in the state.

#### 05:00
The course instructor uses correctly a unique identifier(a simple timestamp - so it is unique if he doesn't add more than one fish per millisecond) as key for this generated components. Please read this [article](https://medium.com/@robinpokorny/index-as-a-key-is-an-anti-pattern-e0349aece318) carefully. It will give you a better understanding about the `key` prop in React and why index as a key is an anti-pattern.

#### 08:30
TypeScript! It would give you a nice autocomplete in such cases.

#### 10:30
ES6 destructuring is very nice and important for writing cleaner code. If you are not already familiar with it or/and want to learn more about it, read this [article](https://codeburst.io/es6-destructuring-the-complete-guide-7f842d08b98f).
 
### Video #17
#### 04:00
Passing only these things down that are explicitly needed. This is very important and you will learn more about that when you learn the state-management library [Redux](https://redux.js.org/).

#### 05:35
The course instructor Wes Bos talks about functional programming. This is a very crucial concept that helps you writing cleander code. I highly recommend to read this [article](https://hackernoon.com/functional-programming-in-js-map-filter-reduce-pt-5-308a205fdd5f). It points out some very helpful JavaScript functions for arrays.

#### 10:40
"...but it doesn't make a whole lot of sense to make a separate component just for this one item". This is what Wes Bos said when he created a render function in the same file. It is not always easy when you should create an own component in a seperate file for something. I tend to create bigger components first and split it up later if needed. One reason for that is when a component contains too much logic. A second reason could be if I need a part of the component somewhere else. Take the part out and make an own component for it. So your code will be clean and simple.

#### 11:37
Look at the line 23: `<ul>{orderIds.map(this.renderOrder)}</ul>`. If you asked yourself where he passes the `key` prop than you might want to read this [article](https://dev.to/danhomola/point-free-gotchas-in-javascript--3pfi). It is a technique called point-free style.

#### 14:05
Usage of the bang! operator. It is simply a other word for the logical not operator. Checkout this [article](https://medium.com/@pddivine/javascript-bang-bang-i-shot-you-down-use-of-double-bangs-in-javascript-7c9d94446054)! 💣

### Video #18
#### 08:30
Lifecycle methods are very important if you want develop great React applications. Please read this [documentation](https://reactjs.org/docs/react-component.html) before you want to use a specfific lifecycle method in your code. Here is a very neat [cheatsheet](https://devhints.io/react#lifecycle)!

#### 13:30
Always clear open connections in the componentWillUnmount lifecycle method or you will run into memory leak problems. Here is a short example [video](https://teamtreehouse.com/library/prevent-memory-leaks-with-componentwillunmount). If you want to read more about closing connections or XHR requests, then check out this [article](https://medium.freecodecamp.org/how-to-work-with-react-the-right-way-to-avoid-some-common-pitfalls-fc9eb5e34d9e).

### Video #19
#### 04:05
Wouldn't it be nice if you get a correct auto-completion for the params available here? In addition to that think of a person who is not familiar with the code. This person has to look into the code which params are available for the specific route. All these problems get solved with TypeScript!

#### 07:00
Again with the usage of TypeScript, you would notice this kind of bug without switching to the browser. You would see it directly in your code (VSCode) editor instead.

#### 09:30
JavaScript is a single-threaded programming language. Considering this it is very important that you understand the behaviour of asynchron code. I highly recommend reading this [article](https://blog.bitsrc.io/understanding-asynchronous-javascript-the-event-loop-74cd408419ff). Also check out this [article](https://medium.freecodecamp.org/avoiding-the-async-await-hell-c77a0fb71c4c). It points out the correct usage of async/await and how you can avoid common pitfalls.

### Video #20
#### 01:57
As I mentioned above the usage of an object instead of an array for storing the fishes wasn't maybe the correct decision. It is just common sense that if something is written in plural you can iterate over this. Keep this in mind for writing a simple and easy to understand code.

#### 08:18
If the application would use Redux you could avoid this complex data handling, because you could access the whole data state of the application in every (container) component.

#### 15:07
With TypeScript you would encounter this bug immediately in your editor and not during runtime.

### Video #21
#### 01:15
Again an array would have been the better choice. You see with an array instead you just use the [Array.filter](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) function for deleting the fish and thats it.



## PCode Clean Code Adventure
Video #17 14:05: Line 8 and 24
16:47: Line 10 and 13: Give me a solution where you 
