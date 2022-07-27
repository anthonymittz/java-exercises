# Exercises

### Table of contents

**[Part 1. Basics.](#part-1-basics)**

1. [Data types](#section-01-data-types)
2. [I/O: Input and Output](#section-02-input-and-output)
3. [Arithmetic operators](#section-03-arithmetic-operators)
4. [Unary operators](#section-04-unary-operators)
5. [Equality and Relation operators](#section-05-equality-relation-operators)
6. [Conditional operators](#section-06-conditional-operators)
7. [Type comparison operator](#section-07-type-comparison-operator)
8. [Bitwise and bit shift operators](#section-08-bitwise-bit-shift-operators)

# Part 1. Basics

## Section 01. Data types

### Exercise 01. Declaration of primitives

Declare a variable for each of the 8 primitive data types,
without actually initializing them with values.  
<sub>(you should end up with 8 statements)</sub>

### Exercise 02. Integer initialization

For each of the 4 primitive data types used to store integer numbers,
declare two variables without any initialization.
Using another statements, separate from declaration statements,
initialize one to the smallest value possible,
and the other - to the largest value possible.  
<sub>(you should end up with 16 statements)</sub>

### Exercise 03. Fractional initialization

For each of the 2 primitive data types used to store fractional numbers,
declare a variable without initialization.
Using another statement, initialize each of the variables to some value.  
<sub>(you should end up with 4 statements)</sub>

### Exercise 04. Letters and truth

For the primitive data type used to store characters,
declare two variables without intialization.
Using another statements, initialize each of the variables:

- one to `0x4F`, but using the "character literal" notation.
- another to `k`, but using the hexadecimal value.

<sub>(you should end up with 4 statements)</sub>

### Exercise 05. Value the truth

For the primitive data type used to store truth values,
declare two variables without initialization.
Using another statements, intitialize them to 2 possible values (1 for each varialbe).
Then, reassign each of the two variables to the complimentary value.  
<sub>(you should end up with 6 statements)</sub>

### Exercise 06. Array declaration

For each of the 8 primitive data types, declare a variable which can be used
to point to a non-primitive collection of primitive variables.
Don't yet initialize (assign) / allocate any collections on the heap.  
<sub>(you should end up with 8 statements)</sub>

### Exercise 07. Array allocation & element initialization

For each of the 8 primitive data types, declare a variable which can be used
to point to a non-primitive collection of primitive variables.
The next step is to allocate an object on the heap for each of the variables.
Let each collection contain 2 elements.
The next step is to initialize each element for every collection to a random value.  
<sub>(you should end up with the staggering 32 statements)</sub>

### Exercise 08. Array literal

Same as the previous exercise, but you are free to use a shortcut: the array literal notation.  
<sub>(you should end up with the more feasible 8 statements)</sub>

### Exercise 09. String declaration

Declare a variable which can be used to point to a `String` object.
Don't intialize it / allocate any objects on the heap.  
<sub>(you should end up with a single statement)</sub>

### Exercise 10. String allocation & initialization

Declare a variable which can be used to point to a `String` object.
Allocate a new `String` object on the heap, give it a value `foo`,
and assign its address to the variable.  
<sub>(you should end up with 2 statements)</sub>

### Exercise 11. String literal

Declare a variable with the type `String` using the string literal notation. Initialize it to a value `bar`.  
<sub>(you should end up with a single statement)</sub>

### Exercise 12. Cats and dogs

Declare a variable with a type String.  
Initialize it to `Dogs are cool`.  
Change the value of the variable to `But cats are coolers.`

## Section 02. Input and Output

### Exercise 1. Hello, World!

Simply print in the console: `Hello, world!`.

### Exercise 2. Print string value

Initialize a variable of a type `String` to a value `gobbledygook`.
Print the value of the variable in the console.

### Exercise 3. Concatenate!

Print a sentence that consists of 2 String literals: `Hello, ` and `world!`
using only a single `println()` method invocation.  
<sub>Use concatenation `+` to combine 2 literals into a single `String` value.</sub>

### Exercise 4. Divide and conquer

Initialize 2 variables of type `String`, to values: `Hakuna` and `Matata`.
Print a whole sentence to the console using only a single `println()` method invocation.  
<sub>Use concatenation and String literal to separate the words with a white space.</sub>

### Exercise 5. No escape!

Print a String literal `TROP DE NOTES` on the 3 different lines in the console
using only a single `println()` method invocation.
No concatenation allowed this time!  
<sub>Modify the literal if you need to, but keep it a single literal.</sub>

### Exercise 6. Table alignment

Print the values of 3 strings initialized to: `127 15 2`, `1, 7, 148`, `12, 487, 95`
using 3 `println()` method invocations. Align the numbers in columns using tabulation.
Modify the values of the variables if necessary.
The result should look like a borderless table:

```
  127   15    2
  1     7     148
  12    487   95
```

### Exercise 7. Back to the basics

Declare a variable for each of the 6 numeric primitive data types (integer and fractional numbers).  
Initialize each of them to a random value.  
Print to the console the following pattern for each variable:  
`variable: myInteger | type: int | size: 4 bytes/32 bits | value: 156`

### Exercise 8. Format and converters

Declare and initialize 3 arrays:
one should contain 12 months names;
the other should contain a number of days in a month for each month;
the last one should contain an average monthly temperatures usual for the climate of your region.
The temperatures should be expressed as decimals with the precision 1, e.g.: `24.7`
Assume that it is _not_ a leap year, thus no 29th of February.

Print a table that contains 3 columns: month, number of days, average temperature.
Align the output using `System.out.format()` method and appropriate converters.

### Exercise 9. A Bob Ross of CS

print the following art in the console:

```
.-----------------------------------------------------------------------------.
||Es| |F1 |F2 |F3 |F4 |F5 | |F6 |F7 |F8 |F9 |F10|                  C= AMIGA   |
||__| |___|___|___|___|___| |___|___|___|___|___|                             |
| _____________________________________________     ________    ___________   |
||~  |! |" |§ |$ |% |& |/ |( |) |= |? |` || |<-|   |Del|Help|  |{ |} |/ |* |  |
||`__|1_|2_|3_|4_|5_|6_|7_|8_|9_|0_|ß_|´_|\_|__|   |___|____|  |[ |]_|__|__|  |
||<-  |Q |W |E |R |T |Z |U |I |O |P |Ü |* |   ||               |7 |8 |9 |- |  |
||->__|__|__|__|__|__|__|__|__|__|__|__|+_|_  ||               |__|__|__|__|  |
||Ctr|oC|A |S |D |F |G |H |J |K |L |Ö |Ä |^ |<'|               |4 |5 |6 |+ |  |
||___|_L|__|__|__|__|__|__|__|__|__|__|__|#_|__|       __      |__|__|__|__|  |
||^    |> |Y |X |C |V |B |N |M |; |: |_ |^     |      |A |     |1 |2 |3 |E |  |
||_____|<_|__|__|__|__|__|__|__|,_|._|-_|______|    __||_|__   |__|__|__|n |  |
|   |Alt|A  |                       |A  |Alt|      |<-|| |->|  |0    |. |t |  |
|   |___|___|_______________________|___|___|      |__|V_|__|  |_____|__|e_|  |
|                                                                             |
`-----------------------------------------------------------------------------'
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

## Section 03. Arithmetic operators

> TODO: yet to be written

## Section 04. Unary operators

> TODO: yet to be written

## Section 05. Equality relation operators

> TODO: yet to be written

## Section 06. Conditional operators

> TODO: yet to be written

## Section 07. Type comparison operator

> TODO: yet to be written

## Section 08. Bitwise bit shift operators

> TODO: yet to be written
