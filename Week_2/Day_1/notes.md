# Week 2 day 1 notes

## Outline: 
[x] Manual Testing 

[x] Making assertions

[x] Bringing in outside code 

[x] Exporting our code 

5) Intro to NPM: a Node package manager
6) Mocha test runner 
7) Ignoring files/folders
8) Chai assertion library
9) What is TDD? 
10) Practice unit testing 

### Three big things to cover
1) Intro to testing
2) Move code out of/into files
Using other people's code

## Manual Testing:
Writing code, then console.logging the function, then going to the terminal to run the code, and check that the output is what we expect. 

## Making assertions in node: 
import our assert function
  
    const assert = require('assert').strict;

    turns all instances of assert.equal into assert.strictEqual

Then we can use: 
    
    assert.equal(actual, expected);

## Exporting out code 
When we are exproting a single function/object: 

    module.exports = functionName;

when we are exporting multiple functions/objects: 

    module.exports.function1 = function1; 
    module.exports.function2 = function2; 

    OR

    module.exports = {
      function1,
      function2
    }

    When we call a function exported this way, we need to spcify the key when we are assigning it to a value. 

    ****Side note - if the key in an object is the same as the vaule, then you can just implement the key name and the object will assume that the value is the same as the key****

## ignoring files on git
So when we are wanting to ignore files when uploading to git(which we should do with out nodes_modules) we just create a file .gitignore and presumably include the file in there


## Test=Driven developement 
* we write the tests before we write our code
* n-driven development 
* Red then green! git 