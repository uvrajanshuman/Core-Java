# Types of Programming Language:
- a)Procedural Languages:
    - A program is simply a list of instructions which is executed line by line.
    - As the length of program increases, the complexity also increases making it
      difficult to maintain large programs.
    - Relative fast
    - Ex: C etc.
- b)Object Oriented Languages:
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
## Encapsulation:
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
            ___obj.a = 20;___
            //indirect access.
            obj.setA(20);
        }
    }
 ```

### Polymorphism:
-   Polymorphism means same thing being used in different ways.
- There are two type of polymorphism
  a) compile-time polymorphism.
  b) run-time polymorphism.

    
        