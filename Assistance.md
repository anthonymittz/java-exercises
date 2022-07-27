# Assistance

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

1. You should end up with 8 statements, without any use of the assignment operator.

2. You should end up with 16 statements.  
   First 8 are used to declare variables.  
   Last 8 are used to intialize this variables to actual values.

3. You should end up with 4 statements.  
   First 2 are declaration statements.  
   Last 2 are assignment statements.

4. You should end up with 4 statements. First 2 are declaration statements.  
   The next one uses 'character literal' notation (single quotes) to assign a value.  
   The last one uses a hexadecimal integer value to assign a value.  
   Use ASCII / UTF-8 tables to find the appropriate hex codes.

5. You should end up with 6 statements. First 2 are declaration statements.  
   The next 2 are initialization to the 'truthy' and 'falsey' values, in no particular order.  
   The last 2 are reassignment: the one that was 'falsey' becomes 'truthy', the other - vice versa.

6. You should end up with 8 statements. All of them are declaration statments.  
   Don't use 'array literal' notation to assign values.  
   Don't allocate any objects on the heap using the 'new' keyword.

7. You should end up with 32 statements. First 8 are declaration statements.  
   Don't use 'array literal' notation to assign values.  
   The next 8 are statements used for allocation of array objects on the heap.  
   The next 16 statements are used to assign values to each of the array elements.

8. You should end up with 8 statements.  
   They are declaration statements which include initialization using  
   the 'array literal' notation (list of values in curly braces).

9. You should end up with 1 declaration statement.

10. You should end up with 2 statements. The first one is a declaration statement.  
    The second one is an assignment of the address of a newly allocated `String` object.  
    Use the `new String("foo")` to initialize it to a value.  
    However, note that this form is redundant: we have _two_ similar strings, one of which is literal.

11. You should end up with 1 statement. Use the 'String literal' notation  
    (characters that form the string enclosed in double quotes).

12. And there's no point arguing the contrary.

13. Use a `java.util.Scanner` class to get the user input and store it in a variable.  
    Given that we work within the range 1..7, the variable is not necessary the `int` type.  
    Visual styling of the answer is up to you.

## Section 02. Input and Output

1.  Inside the `java.lang` package, there's a class called `System`,  
    which has a static field (class variable) called `out` (of the type `java.io.PrintStream`),  
    which has a `println()` method which takes exactly 1 parameter (a value to print) and returns `void` (nothing).  
    Or, for short: `System.out.println("foo");`.

2.  Simply print the value that a variable has or refers to (depends on the data type).

3.  Concatenation looks like addition, but it's not an addition.  
    _Gluing `String` values together_ to be precise.

4.  Yes, concatenating a whitespace is a thing: `"foo" + " " + "bar"`.

5.  Use an escape character `\n` to insert the "new line" command.

6.  Use an escape character `\t` to insert tabulation.

7.  There will be a bunch of manual typing and repetetive code, be ready. No loops yet!

8.  Use the `System.out.format()` method,  
    which takes a string with converters/flags already inserted,  
    and arguments, for each of the integer/float converter used.  
    Use the converters:

    - `%d` for a decimal integer
    - `%f` for a float
    - `%n` for a platform-independent "new line"

      Note that you can specify the "guide" to align to by using flags:

    - `%10d` - decimal, 10 characters in width, right justified
    - `%010d` - decimal, 10 characters in width with leading zeroes, right justified
    - `%+d` - decimal, include sign, right justified
    - `%-d` - decimal, left-justified
    - `%.3f` - float, 3 places after decimal point, right justified

    More on the topic: [Formating numeric print output](https://docs.oracle.com/javase/tutorial/java/data/numberformat.html).

9.  Have fun and use tons of `println()` statements.

10. Do not forget to close the stream after you've grabbed the input.  
    Be sure to close it when you do error/exception handling, just before exiting your program.

    ```java
    Scanner myScanner = new Scanner(System.in);
    String input = myScanner.nextLine();
    ...
    myScanner.close();
    ```

11. Use `int input = myScanner.nextInt();`.  
    This variable can be used later to grab the necessary element of the array.  
    Just don't forget the fact that arrays are 0-indexed.

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
