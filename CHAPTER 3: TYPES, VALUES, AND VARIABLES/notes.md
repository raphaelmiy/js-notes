# CHAPTERS, VALUES AND VARIABLES

The kinds of values that can be represented and manipulated in a programming language are known as types. When a programm wants to retain a value for future use, it assigns the value to a variable.

JavaScript can be divided into two categeries: *primitive types* and *object types*. Primitive types include numbers, strings of text, and Boolean truth values.

The special JavaScript values **null** and **undefined** are primitive values, but they are not numbers, strings, or booleans. Each value is typically considered to be the sole member of its own special type.

ES6 adds a new special-purpose type, known as ***Symbol***, that enables the definition of language extensions without harming barkward compatibility.

Any JS value that is not a number, a string, a boolean, a symbol, null, or undefined is an object. An object (that is, a member of the type object) is a collection of properties where each property has a name and a value (either a primitive value or another object).

An ordinary JS object is an unordered collection of named values. The language also defines a special kind of object, known as an ***array***, that represents an ordered collection of numbered values. The JS language includes special syntax for working with arrays, and arrays have some special behavior that distinguishes them from ordinary objects.

## Other Usefull Object Types

-Set Object: represents a set of values.

-Map Object: represents a mapping from keys to values.

-Typed array types: Facilitate operations on arrays of bytes and other binary data.

-RegExp Type: represents textual patterns and enables sophisticated matching, searching and replacing operations on strings.

-Data Type: Represents dates and times and supports rudimentary date arithmetic

-Error and its Subtypes: represent errors that can arise when executing JS code.

Functions and classes are not just part of the language syntax: they are themselves values that can be manipulated by JS programs. Like any JS value that is not a primitive value, functions and classes are a specialized kind of object.

JS's object types are *mutable* and its primitive types are *immutable*. A value of a mutable type can change.

Constants and variables allow you to use names to refer to values in your programs. Constants are declared with **const** and variables are declared with **let**. JS constants and variables are ***untyped***: declarations do not specify what kind of values will be assigned.
