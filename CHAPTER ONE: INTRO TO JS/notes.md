# CHAPTER ONE NOTES AND CODE

Javascript's most important datatype is the object.

An object is a collection of name/value pairs, or a string to value map.

```javascript
let book = {                // Objects are enclosed in curly braces.
    topic: "JavaScript",    // The property "topic" has value "JavaScript"
    edition: 7              // The property "edition" has value 7
};                          // The curly brace marks the end of the object
```

The properties of an object can be accessed with . or []

Properties can also be accepted conditionally with ?.

```javascript
book.topic                  // => "JavaScript"
book["edition"]             // => 7: another way to access property values.
book.author = "Raphael"     // Create new property value by assignment.
book.contents = {};         // {} is an empty object with no properties.
book.contents?.ch01?.sect1  // undefined: book.contents has no ch01 property.
```

JavaScript also supports arrays (numerically indexed lists) of values:

```javascript
let primes = [2, 3, 5, 7];    // An array of 4 values delimited with [ and ].
primes[0]                    // => 2: the first element (index 0) of the array.
primes.length               // => 4: how many elements are there in the array.
primes[primes.length-1]    // => 7: the last element of the array.
primes[4] = 11;           // Alter an existing element of the array by assignment.