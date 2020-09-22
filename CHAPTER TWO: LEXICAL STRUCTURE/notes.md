# CHAPTER TWO: LEXICAL STRUCTURE

The set of elementary rules that specifies how you write programs in a language. It is the lowest level syntax of a language: it specifies what variable names look like, the delimiter characters for comments, and how one program statement is separated from the next, for example.

## Comments

```javascript
// This is a comment

/* This is also a comment */ // here is another comment.

/* This is a multiline comment
The multiline comment continues
*/
```

## Literals

A data value that appears directly in a program.

```javascript
12                                  // The number twelve
1.2                                // The number one point two
"Hello Miy"                       // A string of text
'Hi'                             // Another string
true                            // A Boolean value
false                          // The other Boolean value
null                          // Absence of an object
```

## Identifiers and Reserved Words

Identifiers are used to name constants, variables, properties, functions and classes and to provide labels for certain loops in JS code. An identifier must begin with a letter, an underscore or a dollar sign. Digits are not allowed as the first character so that JS can easily distinguish identifiers from numbers.