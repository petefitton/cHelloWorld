# C Tutorial from www.freecodecamp.org/news/the-c-beginners-handbook

Tutorial shows that standard C file extension is .c

#include is used for importing

<stdio.h> stands for standard input-output library which is accessible through the built-in compiler

function return type defined prior to function name

parameters defined inside of parentheses (void if no parameters are used)

curly braces for code block

semicolons for ending expressions inside of the functions

gcc is the build-in compiler in Terminal
Compiled by running:

```gcc hello.c -o hello```

Creates executable file which has no file extension

To run the file:

```./hello```

and to look at information of the file:

```ls -al hello```


### FURTHER NOTES:

C is statically typed

Static vs dynamic typed languages:
  - static type checking is done at compile-time
  - dynamic type checking is done at run-time

C/C++/Java are examples of static
Javascript/Python/Typescript are dynamic

note that C requires type declarations when variables are declared
with optional initial values (similar to JS)

```int age;```

or

```int age = 37;```

are both valid in C


Further type example:

    #include <stdio.h>

    int main(void) {
      int age = 0;
      age = 37.2;
      printf("%u", age);
    }

Note that age should be an integer.  Compile warning will force decimal number to convert to an integer


Further types in C:
int, char, short, long, float, double, long double


Different boards will use different byte values for the various types
short can be shorter than int sometimes, sometimes the same size as int
long will never be shorter than int but sometimes is the same size as int

"unsigned" declaration preceding the type word (such as "unsigned int") can limit range to positive numbers and thereby double the highest possible number for the type


increasing beyond the maximum value of an unsigned number will cause the number to cycle back to zero and increase from there

if you don't sign the value, then behavior is undefined and will provide a large number


C does not protect the limits of the type.  Must be programmed in by programmer.

compiler warns with type issues with initializations and assignments but not with mathematical operations



#### CONSTANTS

const precedes type in declaration and value must be assigned

standard to CAPITALIZE a CONSTANT variable name

```const int AGE = 38;```

OR can write:

```#define AGE 37```

(note omitted semicolon & equals sign in second example)
[type is inferred by compiler]


## OPERATORS

#### Arithmetic Operators

=
\+
\-
\*
/
%


Unary operators
\+ (+a)
\- (-a)
++ (a++ or ++a)
-- (a-- or --a)


a++ uses a and then increments
++a increments then uses a

        int a = 2;
        int b;
        b = a++ /* b is 2, a is 3 */
        b = ++a /* b is 4, a is 4 */



#### Comparison Operators

  - ==
  - \!=
  - \>
  - <
  - \>=
  - <=

#### Logical Operators
  - !
  - &&
  - ||

#### Compound Assignment Operators
  - +=
  - -=
  - *=
  - /=
  - %=

#### Ternary Operator

```<condition> ? <expression> : <expression>```

a ? b : c



sizeof returns size of the operand you pass, can pass variable or type






