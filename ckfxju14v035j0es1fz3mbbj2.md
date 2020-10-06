## 5 JavaScript tricks you don't know about

In this article I will be showing you some awesome 🔥🔥 JavaScript tricks that you probably didn't knew about....

These tricks will help you in writing competitive JavaScript and much more....


## 1. Use Strict

If you have some basic knowledge of <a href="https://www.typescriptlang.org">**TypeScript**</a>, then you must be knowing about this.

Use Strict enables strict mode in JavaScript
<ul>
    <li>Does not allow the use of undeclared variables</li>
    <li>Will make you write more secure 🔐 JavaScript</li>
    <li>Deleting a variable or object is not allowed</li>
    <li>And many more things...</li>
</ul>


### How to enable Strict Mode

```
// Add this line of code at the start of your *.js file

"use strict";
```


For more information look into the article on <a href="https://www.w3schools.com/js/js_strict.asp">W3school</a>


## 2. You don't really need semi-colon “;” 

Yeah, you heard that right...
<br>
JavaScript adds semicolons where it is needed and it doesn't find any.

But this semicolon adding does not work as needed sometimes and can give you unnecessary errors ❌. I prefer to keep them, because I don't want to take any chances. You can check more about this <a href="https://flaviocopes.com/javascript-automatic-semicolon-insertion/#:~:text=JavaScript%20semicolons%20are%20optional.,but%20many%20people%20prefer%20them.&text=This%20is%20all%20possible%20because,adds%20it%20behind%20the%20scenes.">here</a>



## 3. Run a function at the time of declaration

Known as the self calling functions or also Immediately Invoked Function Expression (IIFE). It is a function which automatically executes when you create it.

Examples
```
// Example 1
(function(){
    console.log("This is an example of IIFE function");
})();
```

``` 
// Example 2: This function prints sum of two numbers
(function(a,b){
     console.log(a+b);
})(10,35);
```


## 4. Throw custom Errors

Yes!! This is possible in JavaScript, you can throw your own exceptions.

You will mostly use this while debugging, when wrong parameters are passed to a function or according to your wish :)...

Syntax of throwing custom errors...
```
function divide(dividend, divisor){
    // The divisor should not be 0 according to the rules of mathematics
    // Also we need to check if both dividend and divisor are number
    if(typeof divisor != "number")
         throw new Error("Typeof divisor is not a number");
    if(typeof dividend != "number")
         throw new Error("Typeof dividend is not a number");
    if(divisor === 0)
         throw new Error("Divisor cannot be equal to 0");

    return dividend/divisor;
}
```

## 5. Using block scope to create temporary variables

Block scope can be very useful to avoid any unnecessary memory.

Example:
```
{
    let a = "Hello";
    console.log(a);
    // Expected output "Hello"
}
console.log(a);     // undefined
```

>Note: var is function scope, declaring variables with 'var' will not be block scoped. Use 'let' for declaring block scoped variables
<br>
<br>

So, that's all for today guys.

Hope you liked my article... If so drop a ❤️ and 👍.

You can also follow me on <a href="https://twitter.com/CodingThunder">Twitter(@CodingThunder)</a>

