# Reading Notes

What is a ‘Controlled Component’?

a component that can update based on user input and by setState().
It's also controlled by react

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

we wait to store the users responses React allows updating state by partial state. This allows active validation.

How do we target what the user is entering if we have an event handler on an input field?

By using its input name

Why would we use a ternary operator?
 so that code would be less messy.

Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

console. log(x===y? true:false)
