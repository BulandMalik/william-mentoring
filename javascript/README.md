## JavaScript

>We will follow [this](https://www.coursera.org/learn/programming-with-javascript?specialization=meta-front-end-developer) course.

>Later, you can follow [this](https://www.coursera.org/learn/react-basics?specialization=meta-front-end-developer) & [this](https://www.coursera.org/learn/advanced-react?specialization=meta-front-end-developer) advance courses as well.

## What is a scripting language?
1. A high-level programming language that is interpreted by another program at runtime rather than compiled by the computer's processor as other programming languages
2. A programming language designed for integrating and communicating with other programming languages
    
    2.1 Popular scripting languages are JavaScript, VBScript, PHP, Perl, Python, Ruby, ASP
    
    2.2 Since a scripting language is normally used in conjunction with another programming language, they are often found and used alongside HTML, Java or C++
3. The simple difference between scripting language and programming language is: Scripting languages do not require the compilation step and are rather interpreted

    3.1 C program needs to be compiled before running whereas normally, a scripting language like JavaScript or PHP need not be compiled
4. Scripting is interpreted based language, whereas Java, C, C++, and others are compiler-based language

### What is a script?
A script is nothing but sets of instructions
Series of commands

## History
For a long time, JavaScript is used only as a Client Side Front End Development language to build browser-based interactive web pages. But currently due to huge community support (Node or Nide.js) JavaScript is multi-purpose language and used to develop:

1. Full-fledged Enterprise Web Application
2. Full-blown Mobile Apps
3. Real-time Networking Apps (Chats, Audio/Video Streaming Services)
4. Games
5. Command Line Tools (CLI-Command Line Interface utilities)

## Statements
Statements are syntax constructs and commands that perform actions.
> alert('Hello');

## Comments
As time goes on, programs become more and more complex. It becomes necessary to add comments which describe what the code does and why.

Comments can be put into any place of a script. They don’t affect its execution because the engine simply ignores them.

One-line comments start with two forward slash characters `//`.

    // This comment occupies a line of its own
    alert('I have single Line Comment above');

Multiline comments start with a forward slash and an asterisk /* and end with an asterisk and a forward slash `*/`.

    /* An example with two messages.
    This is a multiline comment.
    */
    alert('I have Multi Line Comment above');

## The modern mode, "use strict"

For a long time, JavaScript evolved without compatibility issues. New features were added to the language while old functionality didn’t change.

That had the benefit of never breaking existing code. But the downside was that any mistake or an imperfect decision made by JavaScript’s creators got stuck in the language forever.

This was the case until 2009 when ECMAScript 5 (ES5) appeared. It added new features to the language and modified some of the existing ones. To keep the old code working, most such modifications are off by default. You need to explicitly enable them with a special directive: `use strict`.

The directive looks like a string: `"use strict"` or `'use strict'`. When it is located at the top of a script, the whole script works the `modern` way.

For example:

    "use strict";
    // this code works the modern way
    ...

`use strict` can be put at the beginning of a function. Doing that enables strict mode in that function only. But usually people use it for the whole script.

Modern JavaScript supports “classes” and “modules” – advanced language structures (we’ll surely get to them), that enable use strict automatically. So we don’t need to add the `use strict` directive, if we use them.

## Variables

Variables are used to store this information. A variable is a “named storage” for data.

To create a variable in JavaScript, use the let keyword.

### Variable Declaration
The statement below creates (in other words: declares) a variable with the name “message”:

>let message;

### Variable Assignment

>message = 'Hello!!!!'; // store the string 'Hello' in the variable named message

To be concise, we can combine the variable declaration and assignment into a single line:
>let message = 'Hello!'; // define the variable and assign the value

### var instead of let

In older scripts, you may also find another keyword: var instead of let:
>var message = 'Hello';

1. Its more about scoping of the variable. 
2. Variables, declared with var, are either function-scoped or global-scoped. 
3. “var” tolerates re-declarations
4. “var” variables can be declared below their use

More information can be seen [here](https://javascript.info/var). 

## Where to embed include write put JavaScript in HTML?
1. Inside the HEAD section
2. Inside the BODY section
3. External JavaScript .js file (separation of concern)

## More References
1. [You-Dont-Know-JS](https://github.com/getify/You-Dont-Know-JS)
2. [https://www.codecademy.com/learn/introduction-to-javascript](https://www.codecademy.com/learn/introduction-to-javascript)
3. [JavaScript for Beginners](https://github.com/dinanathsj29/javascript-beginners-tutorial)
4. [30-Days-Of-JavaScript](https://github.com/Asabeneh/30-Days-Of-JavaScript)
5. [Resources to Become a JavaScript Expert](https://github.com/zero-to-mastery/resources/blob/master/JavaScript.md)
