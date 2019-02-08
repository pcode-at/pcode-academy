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
It shows very well the usage of the function [Object.keys](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/keys) but in my opinion an Array would have been the better choice for storing the fishes in the state.

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


