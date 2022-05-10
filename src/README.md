# Types of Programming Language:
- **a)Procedural Languages:**
    - A program is simply a list of instructions which is executed line by line.
    - As the length of program increases, the complexity also increases making it
      difficult to maintain large programs.
    - Relative fast
    - Ex: C etc.
- **b)Object Oriented Languages:**
    - A programming pattern which deals with the concept of objects to build programs.
    - Modelled around real world.
    - A real world object has
      ***attributes/data:*** Attributes define data for an object.
      ex: attribute of car would be color, speed, noOfTypes etc.
      the attributes will have specific values like red for color.
      ***behaviour/methods:*** Behaviour depicts what can be done with the object and it may manipulate the value of attributes.
    - Behaviour also define the way an object interact with other objects.
    - Objects exhibit similar property in OOP also.
    - Relatively slow in execution
    - Ex: JAVA, C++ etc.
  
----
# Features of Object-Oriented Programming:
### Classes:
- A class is defined as the blueprint for an object.
- It serves as a plan or a template.

### Objects:
- Objects are teh instances of a class.
- All objects of a class will have same attributes and behaviour as defined in class; the only difference the values of those attributes may vary.
- classes are logical in nature  i.e- it does not has a physical existance.
- For Ex.- furniture does not has any existance but table,chair do exist.

### Abstraction:
- Abstraction is a way to manage complexity by abstrcting the details.
  For ex.- we drive a car with the provided abstraction like brakes, steering etc.
  So, abstraction is way to manage complexity by concentrating only on essentials and supressing implementation details.

### Inheritance:
- Inheritance is a way to adopt characterstics of parent class.
- There exists a parent-child relationship among the classes.
- When a class inherits another class, it has all the properties of the parent-class and it may have additional properties of it's own.
- For Ex: To make a Scientific Calculator with complex operations and basic operations the Basic Calculator can be inherited instead of adding the basic operations from scratch.

### Encapsulation:
- Encapsulation is a feature of binding data into objects to hide them from outside world.
- It restricts direct access to the data.
- The access of data is to be done through the methods of the class.
- The data is hidden from outside world thus protected.
  Ex:-
``` java
    class Encapsule{
        //encapsulated variable.
        private int a = 10;
        
        public setA(int value){
            a = value;
        }
    }
    
    class Main{
        public static void main(String []args){
            Encapsule obj = new Encapsule();
            //obj.a = 20; //encapsulated variable can't access directly
            obj.setA(20);
        }
    }
 ```

### Polymorphism:
-   Polymorphism means same thing being used in different ways.
- There are two type of polymorphism
  - a) compile-time polymorphism.
  - b) run-time polymorphism.

----
----
# Introduction to Java:
# Java:
- Programming Language: Java is a high level, object-oriented programming language.
- Platform: Java is also a platform, as it has it's own runtime environment JVM (Java Virtual Machine).
  JVM provides a platform which accepts the bytecode and executes on machine.
    
## History Of Java:
- Developed by James Gosling and team at Sun Microsystem in 1991.
- Oak was the first name of Java
- Oracle acquired sun microsystem in 2010.
----

## Features of Java: 

### Platform Independence:
- Java is designed to be platform neutral so that it can run on multiple platforms.
- Java source code is compiled into an intermediate form called bytecode. This bytecode is platform independent but can not run 
directly on any operating system.
The Java compiler is same for all platforms (unlike c/c++ where compilers are platform dependent).
To run this platform independent bytecode, JVM(Java virtual machine) is required which is platform specific.

![ Platform Independence of Java ](../assets/images/java-program-execution.png);

### Object Oriented:
- Java is nearly 100% object-oriented language.
- Everything in Java (constant, variable, method) are defined inside a class and accessed through objects.
- Java support primitive data type like int, byte, short \.\. etc. and these are not objects.

### Both Compiled and Interpreted: 
- #### Compilation: 
  - The program source code is first converted into native machine code through a compiler.
The output of compiler is a executable program (.exe file)
  - This executable program(.exe file) load directly into processor and gets executed
  - The advantage is fast speed as the compiler can perform optimization because it looks at the program as a whole not 
      line by line.
  - The disadvantage would be slower debugging (for each change the entire program needs to be re-compiled) and reduced
   portability (as the program needs to be compiled for each specific platform)

- #### Interpretation: 
  - An interpreter reads one line of code and executes it before going for next line.
  The line is converted into native machine code and executed before moving for next line.
  - In interpretation there is no intemediate steps between writing the code and running it.
  - The advantage will be fast debugging as there is no intermediate step between writing a program and running it) 
   and increased portability.
  - The disadvantage would be slower speed

- #### Java's Approach:
  - **Java follows both compilation and interpretation.**
  - Compilation: The Java program is compiled into an intermediate form bytecode (.class file). 
  - Then the JVM interprets this bytecode
  - The bytecode will run on any platform which has JVM installed (as the program runs in JVM, so platform doesn't matter).

### Automatic Memory Management :
- JVM performs Automatic Memory Management 
- To create an instance of a class new operator is used. And when the object is no longer being referenced it is automatically removed 
from memory.
- This is also called Garbage Collection.


### Multithreading: 
- Java supports Multithreading.
- Multi-Processing: The simultaneous execution of multiple processes/programs at the same time 
Ex: Concurrent execution of multiple programs like word, chrome, editor etc.

- Multithreading: The simultaneous execution of multiple sub-process/thread of a process at the same time.
EX: Concurrent execution of multiple sub-processes of a program like operating multiple tabs in a chrome browser.
- Thread: A lightweight sub-process of a process.
- So, Multithreading is process of executing multiple threads simultaneously.

### Secured
        

