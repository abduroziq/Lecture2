# TABLE OF CONTENTS
* 1) SCOPE
* 2) HOISDING
* 3) RECURSION
* 4) CLOSURE
>


# SCOPE


* 1) GLOBAL SCOPE
* 2) FUNCTION  SCOPE
* 3) BLOCK SCOPE
* 4) MODULE SCOPE

## GLOBAL SCOPE
>A variable declared outside a function, becomes GLOBAL.
>
>Variables declared Globally (outside any function) have Global Scope.
>
>Global variables can be accessed from anywhere in a JavaScript program.
>
>Variables declared with var, let and const are quite similar when declared outside a block.
>
>They all have Global Scope:

## FUNCTION  SCOPE

>JavaScript has function scope: Each function creates a new scope.
>
>Variables defined inside a function are not accessible (visible) from outside the function.
>
>Variables declared with var, let and const are quite similar when declared inside a function.
>

## BLOCK SCOPE

>Before ES6 (2015), JavaScript had only Global Scope and Function Scope.
>
>ES6 introduced two important new JavaScript keywords: let and const.
>
>These two keywords provide Block Scope in JavaScript.
>
>Variables declared inside a { } block cannot be accessed from outside the block:

# HOISTING 
>Hoisting is (to many developers) an unknown or overlooked behavior of JavaScript.

If a developer doesn't understand hoisting, programs may contain bugs (errors).

To avoid bugs, always declare all variables at the beginning of every scope.

Since this is how JavaScript interprets the code, it is always a good rule.

## ( var)
>There’s a temptation to think that all of the code you see in a
JavaScript
program is interpreted line-by-line, top-down in order, as the program
execute. While that is essentially true, there’s one part of that as‐
assumption that can lead to incorrect thinking about your program.
# let 
>Variables defined with let and const are hoisted to the top of the block, but not initialized.
>
>Meaning: The block of code is aware of the variable, but it cannot be used until it has been declared.
>
>Using a let variable before it is declared will result in a ReferenceError.
>
>The variable is in a "temporal dead zone" from the start of the block until it is declared:

# const
Using a const variable before it is declared, is a syntax error, so the code will simply not run.