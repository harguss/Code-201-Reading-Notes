# Class 3

## Reading

## React Docs - lists and keys

1. What does .map() return?   An array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?  You can use map()

3.Each list item needs a unique _key___.

4.What is the purpose of a key?   It is a special string attribute you need to include when creating a list of elements.

## The Spread Operator

1. What is the spread operator?  It is three dots (...)
2.List 4 things that the spread operator can do.
It allows us to use all the elements in an array.
It allows us to operate Math functions on an array.
It can concat a string or merge two or more arrays without using concat() function.
It allows us to copy all elements of an already existing array into a new array and perform push, pop operations without even disturbing the previous array.

3.Give an example of using the spread operator to combine two arrays.
const numbers = [1, 2, 3, 4, 5, 6];
const [one, two, ...rest] = numbers;

4.Give an example of using the spread operator to add a new item to an array.
Give an example of using the spread operator to combine two objects into one.
Videos
How to Pass Functions Between Components

In the video, what is the first step that the developer does to pass functions between components?
In your own words, what does the increment function do?
How can you pass a method from a parent component into a child component?
How does the child component invoke a method that was passed to it from a parent component?
Bookmark and Review
React Tutorial through ‘Declaring a Winner’
React Docs - Lifting State Up
