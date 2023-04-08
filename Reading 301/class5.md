# **Reading-Notes

## React Docs - Thinking in React

1. What is the single responsibility principle and how does it apply to components?     The single responsibility principle, is that a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?
To build a static version of your app that renders your data model,build components that reuse other components and pass data using props. Do not use state, statee is for interactivity.

3. Once you have a static application, what do you need to add?   You will then add the interactive UI.

4. What are the three questions you can ask to determine if something is state?
  1  Is it passed in from a parent via props? If so, it probably isn’t state.
  2  Does it remain unchanged over time? If so, it probably isn’t state.
  3 Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. How can you identify where state needs to live?
For each piece of state in your application:

*Identify every component that renders something based on that state.

*Find a common owner component (a single component above all the components that need the state in the hierarchy).

*Either the common owner or another component higher up in the hierarchy should own the state.

*If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Let’s run through this strategy for our application

*ProductTable needs to filter the product list based on state and SearchBar needs to display the search text and checked state.

*The common owner component is FilterableProductTable.

*It conceptually makes sense for the filter text and checked value to live in FilterableProductTable

## Higher-Order Functions

1. What is a “higher-order function”?

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

3. Explain how either map or reduce operates, with regards to higher-order functions.

## array.reduce()

## Overview

`arr.reduce( (accumulator,value,index) => {...}, initialvalue)`

### Basics

`.reduce()` iterates over an array and returns the last version of the "accumulator" ... in each iteration, based on the value and/or idx of the current element in the array, you have the opportunity to modify and return the accumulator. After the last iteration of the array, that accumulator value is returned to the caller. `initialvalue` represents the value of the accumulator in the first iteration.

**Add up all the numbers in an array**
In this example, the accumulator starts out as 0 (the initial value) and for each iteration, we simply add onto it, and then return it.  That return value gets fed into the next iteration so that you can continually operate on it and return the final value.

```js
let numbers = [1,2,3,4];
let sum = numbers.reduce( function(accumulator,value,idx) {
  accumulator = accumulator + value;
  return accumulator;
}, 0);

// sum would be 10
```

**Change the shape of you data**
In this example, we'll take an array of objects and return back an object, keyed by the 'name' property. The initial value is an empty object, and as we iterate, we create a new entry in it, returning it as we build on.

```js
  let people = [
    {name:'Fred', role:'Developer'},
    {name:'Suzy', role:'Developer'},
    {name:'Gina', role:'Manager'},
    {name:'Jim', role:'Support'}
  ];
  
  let folks = people.reduce( (accumulator, person, idx) => {
    accumulator[person.name] = person.role;
    return accumulator;
  }, {} );
  
  // folks:
  {
    Fred: 'Developer',
    Suzy: 'Developer',
    Gina: 'Manager',
    Jim: 'Support'
  }
  
```

## Reference

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce)
- [Medium](https://medium.com/@JeffLombardJr/understanding-foreach-map-filter-and-find-in-javascript-f91da93b9f2c)
