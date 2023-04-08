# **Reading-Notes-10**

## Understanding the JavaScript Call Stack <https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4>

1. What is a ‘call’?  function invocation
2. How many ‘calls’ can happen at once? One-The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
3. What does LIFO mean?
   At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
5. What causes a Stack Overflow?
 A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## JavaScript error messages <https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c>

1. What is a ‘reference error’? This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

2. What is a ‘syntax error’? This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

3. What is a ‘range error’? Try to manipulate an object with some kind of .length and give it an invalid length (-1)and this kind of errors will show up.

4. What is a ‘type error’? Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

5. What is a breakpoint? Set a breakpoint, which will make your program stop at that point only if a condition is met, this is beneficial for when you want to debug huge cycles for specific values. In this example the breakpoint will point stop when the index reaches 40.
6. What does the word ‘debugger’ do in your code?
