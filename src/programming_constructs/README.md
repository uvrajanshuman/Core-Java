# Java Programming Constructs

## Sample Java Program

- HelloWorld.java
```Java
    class HelloWorld{
    // Execution of program starts from main method
    public static void main(String []args){
        System.out.println("Hello World");
    }
}
```
Steps of execution 
1. compile the HelloWorld.java to generate **HelloWorld.class**

    `c:user\desktop\javac HelloWorld.java`

2. execute the generated **HelloWorld.class**

    `c:user\desktop\java HelloWorld`

- Why save as HelloWorld.java (same as class name)
    - After compilation each Java class is placed into a new file with same name as the class with .class extension
    - And to run the class name should be provided instead of source-file name
    - So, it is a good practice to save file with same name as class so that .class file is also generated with same name

---
## Variables
Variables are the symbolic name of memory locations where some data can be stord.
These values may change during the execution of program

Ex: 

`int a = 10;`

## Constants
Constants are also symbolic name of memory locations where some data is stored.
The value needs to be initialized at the time of declaration.
These values can not changed after initialization.

EX: 

`final int A = 10; //value can't be changed afterwards`

## Data Types
There are two kinds of Data Types:
1. Primitive Data Type (built-in data type)
2. Non-Primitive Data Type (user-defined data type)

- All the variables in Java must be declared before using them.

There are 8 primitive data types in Java

|Data Type|Default Value|Size|
|---------|-------------|----|
|byte|0|8|
|short|0|16| 
|int |0|32|
|long |0|64|
|float|0.0|32|
|double| 0.0|64|
|char|'\u0000'|16|
|boolean|false|Not defined|

- In Java Garbage values are not allowed; so if a variable is not initialized (assigned a value)
it gets it's default value.
- The size of all the data types of Java is pre-defined (unlike c/c++ where size of data type varies on machine) because Java is portable.
And this makes it uniform across platforms.

## Identifier
Identifiers are the names given to variables, constants, methods, classes, interfaces and packages.
**Rules for naming an identifier**
1. It can be any combination of letters, digits, underscores and currnecy symbol.
2. The first character of an identifier can never be a digit.
3. The whitespaces are not allowed.
4. The reserved words can't be used as an identifier.

**Naming Convention**

**1. class or interface identifiers:**

Begins with uppercase letter and first letter of each subsequent word is uppercase
    
EX:

`public class MyCalculator`

`public interface Calculator`

**2. variable or method identifiers:** 

starts with lowercase and every subsequent word is uppercase letter
    
Ex:

`int studentName;`

`void showResult()`

**3. constant identifiers:**

specified in uppercase and subsequent words are seperated with underscores;
    
Ex:

`final double TAX_RATE = 7.5;`

**4. package identifiers:**

specified in all lowercase
    
Ex:
        
`package mypackage.subpackage`


## Keywords
    
Keywords are the pre-defined identifiers for specific purposes

## Literals

A literal is a value that can be passed to a variable or constant.

Literals can be numeric (for byte, short, int, long, float, double),
character, boolean, string and null.

Ex: `int a = 10;`

int: data-type

a: variable

10: literal

### Numeric literal

Thease can be represented in binary, decimal, octal or hexadecimal notation
and can be assigned to all numeric types and character.

- Binary Literal:

    Combination of 0 and 1; prefixed with 0b or OB

    `int bin = 0b1010001; // bin = 81`
    
    `char bin = 0b1010001; // bin = Q`
    
    `float bin = 0b1010001; // bin = 81.0`


- Octal Literal:
    
    Combination of digits from 0 to 7; prefixed with 0

  `int oct = 011; // oct = 9`

  `char oct = 0150; // oct = h`

  `float oct = 0234; // oct = 156.0`


- Hexadecimal Literal:
    
    Combination of digits from 0 to 9 and A to F; prefixed with 0x or 0X

  `int hex = 0x0001; // hex = 1`

  `char hex = 0x45; // hex = E`

  `float oct = 0xA3; // hex = 163.0`


**Note:**
    
> All integer literals are of type int by default;
> To define them as long, suffix L or l is used;
> Ex: Long l = 234567l;

> All floating literals are of type double by default. 
> To define them as float suffix F or f is used.
> EX: float f: 24.6f;

## Character Literals:

A single character enclosed in single quotes.
This can also be done by prefixing four hexadecimal digits (representing 16 bit unicode character) with '\u';
EX:

` char a = 'A';`

` char b = '1';`

` char c = '$';`

` char d = '\u004e';`

` char e = '\t'; //escape sequence`

Note:
> An escape sequence represents a character by prefixing it with '\'
>  \t    -- Horizontal tab
>  \n    -- New Line
>  \"    -- Double quote

## Boolean literal

A boolean literal can either be true or false.

Default value is false;

Ex:

`boolean active = true;`

## String literal

A string literal consists of zero or more characters enclosed in double quotes.

EX:

`String s = "Amay";`

## Null literal

It is assigned to object reference variable.

Unassigned object reference variable have null as value.

----

# Operators
An operator manipulate one or more operands to produce some result.

> Ex: a+b     
> a,b are operands while + is operator

On the basis of no. of operands there are three types of operators.
1. unary operator -> single operand
2. Binary operator -> two operands.
3. Ternary operator -> three operands.

**General Classification**

**1. Arithmetic operator**

  >'+' Addition
> 
> '-' Substraction
> 
> '*' Multiplication
> 
> '/' Division
> 
> '%' Modulo (to find remainder)

**Note**:

'+' operator in Java is overloaded. when it's operands are numeric then simple division takes place.
But, when one of the operand is string then other operand also get converted into string and String Concatenation takes place.

EX:

    1+2 // 3 (operands numeric)

    "Abc" + 2 //Abc2 (one operand is string)

    "Abc" + "Def" //AbcDef (both operands are string)

**2. Relational operator**

Thease operators always return a boolean value.
> '==' Equal to
> 
> '!=' Not equal to
> 
> '<' Less than
> 
> '<='  Less than or Equal
> 
> '>'  Greater than
> 
> '>'   Greater than or equal

**3. Bitwise operator**

**4. Logical operator**

Results in boolean value.

> '&&' logical And
> 
> '||' logical Or
> 
> '!' not

- '&&' Logical And
  
In case of AND if the first operand is false, no matter what the second operand is the result will always be false

| operand1 | operand2                       | result |
|----------|--------------------------------|--------|
| true     | false                          | false  |
| false    | *does not matter* (true/false) | false  |
| true     | true                           | true   |

- '||' Logical OR

In case of OR if the first operand is true, no matter what the second operand is the result will always be true

| operand1 | operand2                       | result |
|----------|--------------------------------|--------|
| false    | false                          | false  |
| true     | *does not matter* (true/false) | true   |
| false    | true                           | true   |

- '!' Logical OR

Inverts the value

| operand1 | result | 
|----------|--------|
| ! true   | false  | 
| ! false  | true   | 

**5. Assignment operator**

> Simple assignment operator
> 
> '='
> 
> Compound assignment operators
> 
> '+=' , '-=', '*=', '/=', '%=', '<<=', '>>=', '&=', '|=', '^=', '>>>='

Ex:

```java
class Demo{
  public static void main(String[] args) {
    int a = 10; // a== 10  Simple Assignment 
    
    a += 10;  // a = a+10 ; a==20;  Compound Assignment
  }
}
```


**6. Ternary operator**

> **operan1 ? operand2 : operand3**
> 
> operand1 must result into a boolean value
> if operand1 results in true; then operand2 is returned.
> if operand1 results in false; then operand3 is returned.

```java
class Demo{
  public static void main(String[] args) {
    int a = 10;
    int b = 20;
    int c = (a>b) ? a : b;
    System.out.println(c); //20
    System.out.println("greater number is: "+(a>b ? a :b)); // greater number is 20
  }
}

```

- works in C but not in Java. 
- In Java ternary operator must return a value.
- Ex: 
``` C
int main(){
  int a = 10;
  int b = 20;
  a>b ?printf("a is greater"):(b is greater);
}

```




