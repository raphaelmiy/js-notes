# CHAPTER ONE NOTES AND CODE

Javascript's most important datatype is the object.

An object is a collection of name/value pairs, or a string to value map.

```javascript
let book = {                    // Objects are enclosed in curly braces.
    topic: "JavaScript",       // The property "topic" has value "JavaScript".
    edition: 7                // The property "edition" has value 7.
};                           // The curly brace marks the end of the object.
```

The properties of an object can be accessed with . or []

Properties can also be accepted conditionally with ?.

```javascript
book.topic                      // => "JavaScript".
book["edition"]                // => 7: another way to access property values.
book.author = "Raphael"       // Create new property value by assignment.
book.contents = {};          // {} is an empty object with no properties.
book.contents?.ch01?.sect1  // undefined: book.contents has no ch01 property.
```

JavaScript also supports arrays (numerically indexed lists) of values:

```javascript
let primes = [2, 3, 5, 7];    // An array of 4 values delimited with [ and ].
primes[0]                    // => 2: the first element (index 0) of the array.
primes.length               // => 4: how many elements are there in the array.
primes[primes.length-1]    // => 7: the last element of the array.
primes[4] = 11;           // Alter an existing element of the array by assignment.
```

Arrays and objects can hold other arrays and objects.
```javascript
let points = [          // An array with two elements.
    {x: 0, y: 0},      // Each element is an object.
    {x: 1, y: 1}
];
let data = {                    // An object with 2 properties.
    trial1: [[1,2], [3,4]],    // The value of each property is an array.
    trial2: [[2,3], [4,5]]    // The elements of the arrays are arrays.
};
```

### Expressions

An expression is a phrase of JavaScript that can be evaluated to produce a value. The use of . and [] to refer to the value of an object property or array element is an expression. 

### Statements

If JavaScript expressions are like phrases, then JavaScript statements are like full sentences. A expression is something that computes a value but doesn't do anything: it doesn't alter the program state in any way. Statements on the hand hand don't have a value but they do alter the state.

### Functions

A function is a named and parameterized block of JavaScript code that you define once and can then invoke over and over again. 

```javascript
let x = 5, y = 65
function plus1(x) {                     // Define a function named plus1 with a parameter x
    return x + 1;                      // Return a value one larger than the value passed in
}                                     // Functions are enclosed in curly braces.

plus1(x)

let square = function(x) {           // Functions are values and can be assigned to vars
    return x * x;                   // Compute the function's value
};                                 // Semi colon marks the end of the assignment

square(plus1(y))                 // Invoke two functions in one sentence
```

When we use functions with objects we get methods. When functions are assigned to the properties of an object, we call them methods. All JavaScript objects including arrays have methods.

```javascript
let a = [];                       // Create an empty array
a.push(1,2,3);                   // The push () method adds elements to an array
a.reverse();                    // Reverse the order of elements.
```

We can define our own methods too. The 'this' keyword refers to the object on which the method is defined.

```javascript
points.dist = function() {      // Define a method to compute distance between points
    let p1 = this[0];
    let p2 = this[1];
    let a = p2.x-p1.x;         // Difference in x coordinates
    let b = p2.y-p1.y;        // Difference in y coordinates
    return Math.sqrt(a*a +   // The Pythagorean theorem
    b*b);                   // The Math.sqrt computes the square root
};
points.dist()             // => Math.sqrt(2): distance between our 2 points.
```

JavaScript statements include conditionals and loops using the syntax of C, C++, Java and other languages.

```javascript
function abs(x) {                           // A function to compute the absolute value.
    if (x >= 0) {                          // The if statement ...
        return x;                         // ... execute
    }
    else {
        return -x;
    }
}
abs(-10) === abs(10)
```
