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

Ex: `int a = 10;`

## Constants
Constants are also symbolic name of memory locations where some data is stored.
The value needs to be initialized at the time of declaration.
These values can not changed after initialization.

EX: `final int A = 10; //value can't be changed afterwards`

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
it gets it's default value
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