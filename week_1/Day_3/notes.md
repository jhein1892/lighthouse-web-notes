# Notes for Day 3

### <u>Table of Content for the Day</u>
1) Object
2) Methods
3) This
4) Memory


#### Objects
Objects are a way of rememebers/storing info in JS

other names: associative array, map, dictionary, hasy 

in JS objects are similar to phonebooks, dictionaries, or group mail boxes IRL.<u> An object is a structure for storing key value pairs</u>

    Object {
    Key : value,
    Key2 : value2,
    ... 
    }

* declaring objects follows the same rules as for a regular variable
    
      const dogs = {"bacon" : "an excitable dog", "fluffers"  : "a good boy", "pickles": "likes food"}

      You don't need to have quotations around the key for this to work. 

* pulling a specific value 

      dogs.fluffers;
      returns  "a good boy"

      or dogs["fluffers"];
    
* adding objects

      dogs.lola = "a sweet dog"

      adds the key "lola", and the value "a sweet dog"

      using this will also allow you to update a value

      or dogs["lola"] = "a sweet dog"

* Deleting a key

      delete dogs.lola; 

      will remove that key:value pair from the object

      or delete dogs["lola"] 

Its worth noting that you can't access pairs using index. They pairs within the objects are ordered by key, not position. 

* Keys need to be unique within the object. 
* Values do not need to be unique

### Why would need to have two different types of notation?

1) if you happen to have a key with spaces, you wont be able to access it using dot notation. 
2) using square brackets, we can put in any valid js statement. And JS will try and execute any instructions within the bracket before looking up the values. AKA dynamically accessing

        dogs["fluff" + "ers"];
        returns the value for "fluffers" 

### Methods

We can add objects, and arrays to our objects, and call them in the way you would think: 
    
    for calling nested array: 
    objectName.keyOfArray[indexOfArray]

    reurns the index of the key

    for calling a nested object: 

    objectName.KeyofNestedObject.KeyOfNestedKey: 

    returns the value of the nested kay 

if you have an function that is a value within an object, its called a method. 


what we are trying to do with objects is to encapsulate real world info data. Objects are a pairing of behaviour + properties/data 

### This

using 'this' can be used anywhere in your programms

    console.log(this)

means different things depending on where it's used. But it really wants to refer to a parent object. So it refers to whatever the parent is of the line that this is called. 
        
    const object {
    prints : this
    }

    when we call object.prints
    we will see 'object' 

if you are using a function, calling this will refer to whatever is to the left. 

    object.prints
    caling this on prints (looking to the left) is going to refer to object

    if there is nothing to the left
    e.g calling "this" on 
    object

    reterns global program 

### Memory

1) primitive types 
    * numbers, strings, boolean
      
      <u>What are these?</u>
      
      The variables are being directly placed within a location in your memory. 

      So if you copy a primitive variable type, all changes made to once of the versions, does not affect the value of the copy. They are considered two separate values
2) reference types 
    * functions, arrays, objects 

      <u> What are these?</u> 

      There is still the box. But rather than the value of the variable being placed in the box, we place a reference(or pointer): which is essentially just a map that lets us know where the object is located. 

      when we copy these types, we are just copying the reference to the object. So we now have two maps to the same object. 
 
