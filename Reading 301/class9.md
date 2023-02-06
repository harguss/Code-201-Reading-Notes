# **Reading-Notes 09**

## Code 301 - Foundations of Software Development

## Functional Programming Concepts <https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa>

1. What is functional programming?
   Functional programming is a programming paradigm that emphasizes immutability, pure functions, and the avoidance of side-effects. It is based on mathematical functions and treats computation as the evaluation of mathematical functions, and is often used to write more readable, testable, and maintainable code.
2. What is a pure function and how do we know if something is a pure function?
   a. It returns the same output for the same   input every time it is called.
   b. It does not modify any values outside of its scope.
   c. It does not rely on any state or data from the outside world, and only uses its input arguments to determine its output.

3. What are the benefits of a pure function?
   They don't have side-effects and always produce the same output for a given input.
4. What is immutability?
  Immutability refers to the concept of an object or value that cannot be changed after it has been created. In other words, once an object has been created and its state set, its state cannot be modified. Instead of modifying an object's state, a new object is created with the desired changes.
5. What is Referential transparency?
   In JavaScript, referential transparency is achieved when a function only depends on its inputs (arguments) and does not have any side-effects, such as modifying global state or making network requests. Functions that meet these criteria are called "pure functions", and their behavior can be predicted solely by their inputs and implementation.

## Videos

 Node JS Tutorial for Beginners #6 - Modules and require()<https://www.youtube.com/watch?v=xHLd36QoS4k>

1. What is a module? It is (js)file that has a specific purpose and is created for orgaanizational purposes.
2. What does the word ‘require’ do? It is a function that creates a path for the modules that a file needs.
3. How do we bring another module into the file the we are working in? Use module.export and and make it  to what you want to make availible outside of its scope.
4. What do we have to do to make a module available? You have to then make a varible that is = to the require function.
