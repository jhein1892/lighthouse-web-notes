# Day 4 notes 

## Table of Contents
1) Functions are values 
2) Function declarations vd function expression
3) What are anonymous functions
4) Arrow functions 
5) Function calling vs passing 
6) Callback functions and higher order functions  
---
### 1) Functions are values 

Functions are values. simple. We can call on them in the same way as the values that we spoke about yesterday. 

### 2) Function declaration vs Function expression / 3) anaonymous functions

Functional declaration 
      
    function englishgreeting() {
      console.log('Hello world)
    }

Functional expression (anonymous Function)

    const spanishGreeting = function () {
      console.log('hola mundo)
    }


in both examples we are calling the functions after we've declared them. 

But with javascripts 'hoisting', you can call a function before it's declared. 

Using functional expression, we are required to define a function before we call them. So we should try to use this as much as possible, since it makes it easier to read and debug. 

### 4) Arrow Functions

Function expression arrow function

    
    const japansesGreeting = () => {
      console.log('konnnichiwa sekai');
    }

    with implicit return: 
    
    const returnsTen = () => 10; 
    
    // which is the same as 

    const longReturnsTen = function () {
      return 10; 
    }
    
### 5) Function calling vs passing

When we want to call a function within another function, we should try and pass the function within the parent function, so we don't need to call a function within a function. 
      
    e.g: 

    we want to be calling: 

    Function(helperFunction);

    NOT

    Function(helperFunction());  

### 6) What are callbacks

Callbacks are a function that is called by another function. Specifically when passes as a parameter to said function. 

    e.g: 

    const higherOrderGreeting = (greeting) {
      console.log(3);
      console.log(2);
      console.log(1);
      console.log('...');
      greeting(); <-- call the greeting as a function. Make sure the arg when calling is a function! 
    }

    when calling it: 

    higherOrderGreeting(spanishGreeting); 
    higherOrderGreeting(englishGreeting);
    ...

so we are passing a function(arg) as an argument within a function(func). 

Callbacks are great at limiting the amount of repeating code. If you're doing the same logic repeatedley, create a helper function and call it within your parent function. 



