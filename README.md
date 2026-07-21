# Documentation-on-JavaScript


## What is JavaScript??

JavaScript (JS) is a high‑level, interpreted programming language primarily used to make web pages interactive. It runs in browsers, on servers (via Node.js), and in many modern applications.

JavaScript is a programming language that adds interactivity to websites. You can use it to control just about anything — form data validation, button functionality, game logic, dynamic styling, animation updates, and much more. This article gets you started with JavaScript and walks you through adding some fun features to your first website.

- Created by: Brendan Eich (1995)

- Standardized as: ECMAScript

- Main uses: Web interactivity, dynamic content, backend services, mobile apps, game development.
  
- JavaScript is case-sensitive


## ⚙️ Key Features

- Dynamic typing → Variables don’t need explicit type declarations.

- Prototype-based OOP → Objects inherit directly from other objects.

- Event-driven → Responds to user actions (clicks, inputs, etc.).

- Cross-platform → Runs on any device with a browser.

- Asynchronous programming → Supports callbacks, promises, and async/await.




## Declarations
JavaScript has three kinds of variable declarations.

- var
Declares a variable, optionally initializing it to a value.

- let
Declares a block-scoped, local variable, optionally initializing it to a value.

- const
Declares a block-scoped, read-only named constant.


## Variables
-You use variables as symbolic names for values in your application. The names of variables, called identifiers, conform to certain rules.

A JavaScript identifier usually starts with a letter, underscore (_), or dollar sign ($). Subsequent characters can also be digits (0 – 9). Because JavaScript is case sensitive, letters include the characters A through Z (uppercase) as well as a through z (lowercase).


## Variable scope
A variable may belong to one of the following scopes:

- Global scope: The default scope for all code running in script mode.
- Module scope: The scope for code running in module mode.
- Function scope: The scope created with a function.
In addition, variables declared with let or const can belong to an additional scope:

Block scope: The scope created with a pair of curly braces (a block).
When you declare a variable outside of any function, it is called a global variable, because it is available to any other code in the current document. When you declare a variable within a function, it is called a local variable, because it is available only within that function.


## Variable hoisting

var-declared variables are hoisted, meaning you can refer to the variable anywhere in its scope, even if its declaration isn't reached yet. You can see var declarations as being "lifted" to the top of its function or global scope. However, if you access a variable before it's declared, the value is always undefined, because only its declaration and default initialization (with undefined) is hoisted, but not its value assignment.

- before variable hosting
  
console.log(x);  // Output: undefined

var x = 5;

console.log(x);  // Output: 5

- after variable hosting

var x;            // declaration hoisted

console.log(x);    // undefined (since only declared, not assigned yet)

x = 5;            // assignment happens here

console.log(x);   // 5


