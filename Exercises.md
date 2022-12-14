# Exercises

### Table of contents

**[Part 1. Basics](#part-1-basics)**

1. [Data types](#section-01-data-types)
2. [I/O: Input and Output](#section-02-input-and-output)
3. [Arithmetic operators](#section-03-arithmetic-operators)
4. [Unary operators](#section-04-unary-operators)
5. [Equality and Relation operators](#section-05-equality-relation-operators)
6. [Conditional operators](#section-06-conditional-operators)
7. [Type comparison operator](#section-07-type-comparison-operator)
8. [Bitwise and bit shift operators](#section-08-bitwise-bit-shift-operators)
9. [Methods](#section-09-methods)

**[Part 2. Control Flow](#part-2-control-flow)**

1. [Branching](#section-01-branching)
2. [Recursion](#section-02-recursion)
3. [Looping](#section-03-looping)

<br><br><br>

## Part 1. Basics

<br><br>

## Section 01. Data types

### Exercise 01. Declaration of primitives

Declare variables to hold each of the 8 primitive data types, but do not initialize them to values.  
<sub>(you should end up with 8 statements)</sub>

### Exercise 02. Integer initialization

For each of the 4 primitive data types used to store integer numbers:  
declare two uninitialized variables; using other statements, initialize the former to the smallest value possible, and the latter - to the largest value possible.  
<sub>(you should end up with 16 statements)</sub>

### Exercise 03. Fractional initialization

For each of the 2 primitive data types used to store fractional numbers:  
declare an uninitialized variable; using another statement, initialize it to some value.  
<sub>(you should end up with 4 statements)</sub>

### Exercise 04. Letters and truth

For the primitive data type used to store characters:  
declare two uninitialized variables; using other statements, initialize:

- the former to `0x4F`, but using the character literal notation.
- the latter to `k`, but using the hexadecimal value.

<sub>(you should end up with 4 statements)</sub>

### Exercise 05. Value the truth

For the primitive data type used to store truth values:  
declare two uninitialized variables;  
using other statements, intitialize them to the two _truth values_ of logic.
then, reassign each of them to the complimentary value.  
<sub>(you should end up with 6 statements)</sub>

### Exercise 06. Array declaration

For each of the 8 primitive data types:  
declare a variable which can be used to point to a collection of values of that type;
don't yet initialize the collections; don't allocate collection objects on the heap.  
<sub>(you should end up with 8 statements)</sub>

### Exercise 07. Array allocation & element initialization

For each of the 8 primitive data types:  
declare a variable which can be used to point to a collection of values of that type.  
Allocate collection objects on the heap (let each collection hold 2 elements).  
Initialize each element for every collection to a random value.  
<sub>(you should end up with the staggering 32 statements)</sub>

### Exercise 08. Array literal

Same as the previous exercise, but you are free to use a shortcut: the array literal notation.  
<sub>(you should end up with the feasible 8 statements)</sub>

### Exercise 09. String declaration

Declare a variable which can hold a reference to a `String` object;  
don't intialize it; don't allocate any objects on the heap.  
<sub>(you should end up with a single statement)</sub>

### Exercise 10. String allocation & initialization

Declare a variable which can hold a reference to a `String` object;  
allocate a new `String` object on the heap and give it a value: `super`;  
make the variable hold the referece to that object.  
<sub>(you should end up with 2 statements)</sub>

### Exercise 11. String literal

Declare a variable with the type `String` using the string literal notation;  
initialize it to a value: `nova`.  
<sub>(you should end up with a single statement)</sub>

### Exercise 12. Cats and dogs

Declare a variable with a type `String`;  
initialize it to: `Dogs are cool.`;  
using reassignment, change it to: `But cats are coolers.`.

<br><br>

## Section 02. Input and Output

### Exercise 1. Hello, World!

Simply print in the console: `Hello, world!`.

### Exercise 2. Print string value

Initialize a variable of a type `String` to a value `gobbledygook`;  
print the `char[12]` that the `String` object now holds to the console.

### Exercise 3. Concatenate!

Print a sentence that consists of 2 String literals: `Hello, ` and `world!`
using only a single `println()` method invocation.  
<sub>Use concatenation `+` to combine 2 literals into a single `String` value.</sub>

### Exercise 4. Divide and conquer

Initialize 2 variables of type `String`, to values: `Hakuna` and `Matata`;  
print a whole sentence to the console using only a single `println()` method invocation.  
<sub>Use concatenation and String literal to separate the words with a white space.</sub>

### Exercise 5. No escape!

Print a String literal `TROP DE NOTES` on the 3 different lines in the console
using only a single `println()` method invocation.
No concatenation allowed this time!  
<sub>Modify the literal if you need to, but keep it a single literal.</sub>

### Exercise 6. Table alignment

Print the values of 3 strings initialized to: `127 15 2`, `1, 7, 148`, `12, 487, 95`
using 3 `println()` method invocations; align the numbers in columns using tabulation;  
modify the values of the variables if necessary.
The result should look like a borderless table:

```
  127   15    2
  1     7     148
  12    487   95
```

### Exercise 7. Back to the basics

Declare a variable for each of the 6 numeric primitive data types (integer and fractional numbers);  
initialize each of them to a random value;  
print to the console the following pattern for each variable:  
`variable: myInteger | type: int | size: 4 bytes/32 bits | value: 156`

### Exercise 8. Format and converters

Declare and initialize 3 arrays:
one should contain 12 months names;
the other should contain a number of days in a month for each month;
the last one should contain an average monthly temperatures usual for the climate of your region.
The temperatures should be expressed as decimals with the precision `1`, e.g.: `24.7`.

Print a table that contains 3 columns: month, number of days, average temperature.
Align the output using `System.out.format()` method and appropriate converters.

### Exercise 9. A Bob Ross of CS

print the following art in the console:

```
  .-----------------------------------------------------------.
  || esc |F1 |F2 |F3 |F4 |F5 |F6 |F7 |F8 |F9 |F10|F11|F12| ??? ||
  ||_____|___|___|___|___|___|___|___|___|___|___|___|___|___||
  ||??  |!  |@  |#  |$  |%  |^  |&  |*  |(  |)  |_  |+  |     ||
  ||??__|1__|2__|3__|4__|5__|6__|7__|8__|9__|0__|-__|=__|____???||
  ||    |Q  |W  |E  |R  |T  |Y  |U  |I  |O  |P  |{  |}  |    ||
  ||???___|___|___|___|___|___|___|___|___|___|___|[__|]__|_???_||
  ||??    |A  |S  |D  |F  |G  |H  |J  |K  |L  |:  |"  ||  |   ||
  ||???____|___|___|___|_-_|___|___|_-_|___|___|___|___|\__|___||
  ||    |~  |Z  |X  |C  |V  |B  |N  |M  |<  |>  |?  |        ||
  ||???___|`__|___|___|___|___|___|___|___|,__|.__|/__|_______???||
  ||   |    |alt|    |                  |cmd|alt|    [ ???]    ||
  ||fn_|ctrl|???__|cmd_|__________________|___|__???|[??? ][ ???][ ???]||
  `-----------------------------------------------------------'
```

### Exercise 10. What did you say?

Declare a variable of the type `Scanner` to hold a reference
to an instance of the class `java.util.Scanner`.
Instantiate the class, point it to `System.in`,
store the resulting pointer in the variable.
Declare a `String` variable to hold potential user input.
Use the instance method `nextLine()` to get a line from the console.
Store the resulting `String` that is returned by the method in the string.
Print the value of the string to the console.

### Exercise 11. Follow the tune

Declare two arrays: the first one to containt variables of type `char`,
the seconds one to contain variables of type `String`.
Initialize the first to the 7 musical notes: `C, D, E, F, G, A, B`.
Initialize the second to the 7 syllables: `Do, Re, Mi, Fa, Sol, La, Si`.

Ask a user to pick a note by using a number between `1 .. 7`;
use `nextInt()` instance method of the `Scanner` class.
Print to the user both names of the same note.  
<sub>Format the output as you like. Use the number to grab the values of array elements.</sub>

<br><br>

## Section 03. Arithmetic operators

> Remains to be written

## Section 04. Unary operators

> Remains to be written

## Section 05. Equality relation operators

> Remains to be written

## Section 06. Conditional operators

> Remains to be written

## Section 07. Type comparison operator

> Remains to be written

## Section 08. Bitwise bit shift operators

> Remains to be written

## Section 09. Methods

### Exercise 01. Declaration & Definition

> Remains to be written

### Exercise 03. Output: `void` return (methods a.k.a procedures)

> Remains to be written

### Exercise 04. Output: value return (methods a.k.a functions)

> Remains to be written

### Exercise 05. Input: parameters (_placeholder_ variables in declaration)

> Remains to be written

### Exercise 06. Invocation (calling)

> Remains to be written

### Exercise 07. Input: arguments (_actual_ values in invocation)

> Remains to be written

### Exercise 08. Single parameter / argument

> Remains to be written

### Exercise 09. Multiple parameters / arguments

> Remains to be written

### Exercise 10. Passing an integer

> Remains to be written

### Exercise 11. Passing a double

> Remains to be written

### Exercise 12. Returning an integer

> Remains to be written

### Exercise 13. Returning a double

> Remains to be written

### Exercise 14. Passing an array

> Remains to be written

### Exercise 15. Returning an array

> Remains to be written

### Exercise 16. Passing a String object

> Remains to be written

### Exercise 17. Returning a String object

> Remains to be written

### Exercise 18. Passing a boolean (or refactoring into 2 functions?)

> Remains to be written

### Exercise 19. Returning a boolean

> Remains to be written

### Exercise 20. Method as abstraction

> Remains to be written

### Exercise 21. Separation of concerns

> Remains to be written

### Exercise 22. 2 semantic levels

> Remains to be written

### Exercise 23. More semantic levels

> Remains to be written

### Exercise 24. Absolute value

> Remains to be written

### Exercise 25. Square the value

> Remains to be written

### Exercise 26. Average value

> Remains to be written

### Exercise 27. Branching the control flow

> Remains to be written

### Exercise 28. Recursion

> Remains to be written

### Exercise 29. Not branching the control flow

> Remains to be written

### Exercise 30. Almost 'for loop'

> Remains to be written

### Exercise 31. Calculate factorial

> Remains to be written

### Exercise 32. Calculate square root

> Remains to be written

<br><br><br>

# Part 2. Control Flow

## Section 01. Branching

> Remains to be written

## Section 02. Recursion

> Remains to be written

## Section 03. Looping

> Remains to be written
