# Java
* Java is a popular programming language that is used for developing a wide range of applications. It is a class-based, object-oriented language that is designed to be easy to use and easy to read. It was originally developed by Sun Microsystems and is now owned by Oracle Corporation. Java is used for developing a variety of applications, including mobile and web applications, games, and more. It is known for its platform independence, which means that Java programs can run on any platform that supports the Java virtual machine.

## The four pillars of object-oriented programming

* **Abstraction** 
    - is a fundamental concept in object-oriented programming. It is a technique that allows a programmer to create complex systems by hiding the details of the implementation and exposing only the essential features of an object. This allows the programmer to focus on the big picture and work with objects at a higher level of abstraction, without needing to know the details of how the objects are implemented.

    - Abstraction is typically achieved through the use of interfaces and abstract classes. An interface defines a set of public method signatures, an object must then provide an implementation for those methods. This allows the programmer to specify what an object can do, without needing to specify how in the interface. An abstract class, on the other hand, provides both implemented methods and method without implementations. What's unique about abstract class is that it prevents the creation an object that is a member of that abstract class. This allows the programmer to create a common foundation for a set of related objects, without needing to duplicate the same code in multiple classes.

    - Abstraction is a useful technique because it allows a programmer to design complex systems in a modular way. It helps to improve the reusability and maintainability of the code, and it makes it easier to understand and work with large programs. It is an essential part of object-oriented programming in Java and other languages.

* **Encapsulation**
    - It is a mechanism that allows a programmer to hide the internal details of an object and expose only the object's public interface. This allows the programmer to create a black box that other parts of the program can use without needing to know how the object is implemented.

    - Encapsulation is typically achieved by using access modifiers like private, protected, and public to control the visibility of the object's data and methods. For example, a class might have a private field that holds some sensitive data, and a public method that allows other parts of the program to access that data in a controlled manner. This ensures that the data is only accessed in the ways that the programmer intended, and helps to prevent unintended side effects and bugs.

    - Encapsulation also allows a programmer to change the implementation of an object without affecting other parts of the program. For example, if an object has a public method that performs some calculation, the programmer can change the internal implementation of that method without breaking any code that depends on the method. This makes the code more flexible and maintainable over time.

    - Overall, encapsulation is a powerful technique that allows a programmer to create well-defined, modular objects that can be used effectively in a larger program. It is a fundamental concept in object-oriented programming. 

* **Inheritance** 
    - It is a programming concept that refers to the ability of a class to derive attributes and behaviors from another class. Inheriting means a subclass can use the attributes and behavior of the superclass without having to re-implement them. This is realized by using the extends keyword for Abstract class and implements for Interface. This can save time and improve the modularity of the code by allowing common attributes and behavior to be defined in a single place and shared among multiple classes. This allows for a clear organization of related classes and helps to avoid duplication of code.
    
    - For example, a SportsCar class might inherit from a Car class, inheriting all of the data and methods of the Car class, and adding new behavior specific to sports cars.

* **Polymorphism** 
    - It is a programming concept that refers to the ability of a single entity, such as a variable, a function, or an object, to have multiple forms. Polymorphism allows for entities to be treated as a single type, even if they have different underlying forms. This can be useful for creating flexible and modular code that is easy to maintain and extend. There are two main types of polymorphism: static pand dynamic polymorphism. Static polymorphism is achieved through method overloading, which allows for multiple methods with the same name but different parameters to be defined in the same class. Dynamic polymorphism is achieved through method overriding, which allows a subclass to override the behavior of a superclass method. This allows the same method call to behave differently depending on the type of object on which it is called.

    - **Method overloading** is a programming concept that refers to the ability to create multiple methods with the same name but with different parameters in the same class. This allows for more flexibility and reusability of code, because the same method name can be used to perform different tasks depending on the number and type of arguments passed to the method. When a method is called, the Java runtime environment determines which version of the method to execute based on the number and type of arguments passed. This is known as dynamic dispatch or late binding. Method overloading is often used as a means of providing multiple versions of a method that perform the same task but take different types or numbers of arguments.

    - **Method overriding** is a programming concept that refers to the ability of a subclass to override the behavior of a superclass method. Method overriding allows a subclass to provide its own implementation for a method that is already defined in the superclass. This allows the same method call to behave differently depending on the type of object on which it is called. For example, if a superclass defines a method named "calculateArea" that calculates the area of a shape, a subclass might override this method to provide a more specific implementation that calculates the area of a rectangle. This allows the subclass to use the same method name as the superclass, but with a different implementation that is more suited to the specific requirements of the subclass. Method overriding is often used to provide more specialized behavior for subclasses, while still allowing them to share common functionality with the superclass.

## JDK, JRE, JVM

* **Java Development Kit** (JDK)
    - A JDK (Java Development Kit) is a software development kit that provides tools and libraries for developing Java applications. It includes the Java Runtime Environment (JRE), which allows Java programs to be executed, as well as a set of development tools, such as a compiler and a debugger, that are needed to create and run Java programs. In other words, a JDK is a package that contains all the necessary tools for developing and running Java programs.

* **Java Runtime Environment** (JRE)
    - The Java Runtime Environment (JRE) is a software package that provides a runtime environment in which Java programs can be executed. It includes the Java Virtual Machine (JVM), which is the virtual machine that runs Java programs, as well as a set of libraries and other files that are needed by the JVM to run Java programs. It is typically included as part of the JDK (Java Development Kit), which also includes the development tools needed to create Java programs.

* **Java Virtual Machine** (JVM)
    - A Java Virtual Machine (JVM) is a virtual machine that is responsible for interpreting and executing Java bytecode, which is the machine code representation of a Java program. It is the part of the Java Runtime Environment (JRE) that is responsible for executing Java programs. JVM is platform-independent, meaning that it can be implemented on any hardware and operating system, and Java programs can be run on any platform that has a JVM installed on it. This is one of the key features of Java that allows it to be portable across different systems.

## Primitive Data Types
    - boolean   : 1bit
    - byte      : 1byte = 8bit
    - short     : 2byte = 16bit
    - char      : 2byte = 16bit
    - int       : 4byte = 32bit
    - float     : 4byte = 32bit
    - long      : 8byte = 64bit
    - double    : 8byte = 64bit

## Array

* **Array**
    - An array is a data structure that stores a collection of elements of the same data type. Each element in an array has a unique index that starts from 0, which is a positive integer that identifies the position of the element inside the array. Arrays are useful for organizing and storing data in a structured manner, and they are a fundamental building block of many computer programs.

* **List**
    - a List represents an ordered sequence of objects. It is a data structure that provides an ordered collection of elements that can be accessed by their index. A List allows duplicate elements and provides various methods for adding, removing, and searching for elements. It is similar to an array, but it has a variable size that can grow or shrink as needed. It can be thought of as a dynamic array that can grow and shrink as needed.

* **Set**
    - a Set is a collection of unique elements. Sets are useful for storing elements in a collection when you don't need to care about the order of the elements, and you don't want to have any duplicate elements.

## Autoboxing

* Autoboxing is a feature of the Java programming language that allows the automatic conversion of primitive data types to their corresponding wrapper class objects and vice versa. This allows developers to work with primitive data types (such as int, and char) in a more object-oriented way, without having to explicitly convert them to and from their wrapper classes (which in Integer, and Character). For example, when a primitive type is used in a context where an object is expected, the compiler automatically wraps the primitive value in an object of the appropriate wrapper class. This allows the use of primitive types and objects interchangeably in the code.

## Wrapper Class

* a Wrapper class is a class that wraps (encloses) a primitive data type and provides it with an object-oriented interface. For example, the primitive type int has a corresponding wrapper class called Integer, which provides methods for converting int values to and from other data types, as well as for performing various operations on int values. Other primitive types, such as char, float, and boolean, also have corresponding wrapper classes. These classes provide useful methods for working with the corresponding primitive type, as well as allowing primitive types to be used as objects.

## Class and Object

* a Class is a template that is used to create objects. It defines the attributes and behaviors that an object of that class will have. Classes are defined using the "class" keyword, followed by the name of the class and a set of curly braces that enclose the class's body. The body of a class can include variables (also known as fields or attributes) that define the state of an object, as well as methods that define the behavior of an object. 

    - For example, a class called "Dog" might define attributes such as breed, size, and color, as well as behaviors such as barking and wagging its tail. Each object created from the Dog class will have its own unique values for these attributes, but it will be able to perform the same behaviors as other objects created from the same class. Classes are a fundamental concept in object-oriented programming.

* an Object is a member (also called an instance) of a Java class. Each object has an identity, a behavior and a state. Objects are created at runtime from templates, which are also known as classes. The identity of an object is their address in memory, their states and behavior are defined in the class they belong to.

## Stack & Heap
    - The stack is a region of memory that is used for storing local variables and function parameters, as well as for storing the return address of a function when it is called. Data that is stored in the stack has a fixed size, and is allocated and deallocated in a last-in-first-out (LIFO) manner. This means that when a function is called, its parameters and local variables are pushed onto the top of the stack, and when the function returns, they are popped off the top of the stack.

    - The heap, on the other hand, is a region of memory that is used for dynamically allocating memory at runtime. Data that is stored in the heap can have a variable size, and is allocated and deallocated in any order. This allows for more flexibility in terms of memory usage, but can also make it more difficult to manage the memory effectively.

    - In general, the stack is faster and more efficient than the heap, but has the disadvantage of having a fixed size, which makes it more limited in terms of the amount of data that can be stored. The heap, on the other hand, is more flexible in terms of memory usage, but is slower and less efficient than the stack.

## Method & Parameters
    - is a block of code that performs a specific task and can be called by other code. Methods are used to modularize and organize code, making it easier to reuse and maintain.

    A method has a name, a return type, and a list of parameters. The name of the method is used to identify the method and call it from other code. The return type specifies the data type of the value that the method returns, or void if the method does not return a value. The parameters are used to pass information to the method, and can have their own data types and names.

## public static void main(String[] args) {}
The main() method is the entry point of a Java program. It is called when the program is run and is where the execution of the program begins. The main() method takes an array of strings as an argument. This array can be used to pass command line arguments to the program.

## Constructor
    - a constructor is a special type of method that is used to initialize an object. Every class has at least one constructor, and a class can have multiple constructors with different parameter lists. A constructor has the same name as the class, and does not have a return type.

## Variable Scope
    - the scope of a variable is the region of the code where the variable is visible and can be accessed.

        - A local variable has a local scope, which means that it is only visible and can only be accessed within the block of code where it is defined.

        - An instance variable has an instance scope, which means that it is associated with a specific instance of a class, and can be accessed from any method of that instance.

        - A class variable has a class scope, which means that it is associated with the class itself, and can be accessed from any method of that class, regardless of the instance of the class.

        - A global variable has a global scope, which means that it is visible and can be accessed from anywhere in the code.

## Access Modifiers
    - public
        - specifies that a class member is visible and accessible to any other class, regardless of its package.

    - protected
        - specifies that a class member is visible and accessible to any other class within the same package, as well as any subclasses of the class, regardless of their package.

    - private
        -  specifies that a class member is only visible and accessible within the class where it is defined.

    - default
        - If no access modifier is specified for a class member, it is given the default access modifier. The default access modifier specifies that a class member is visible and accessible to any other class within the same package, but not to classes in other packages.

## Non-acces Modifiers

## Package and Imports

## Generics

## Interface & Abstract Class
    - Interface
        - is a reference type that defines a set of methods that a class can implement. An interface does not contain any implementation for the methods it defines - it only specifies the method signatures.

    - Abstract Class
        - is a class that cannot be instantiated, but can be extended by other classes. An abstract class can contain both abstract and concrete methods, which means that it can define methods without an implementation, as well as methods with an implementation.

## Functional Interface & Lambda
    - Functional Interface
        - a functional interface is an interface that has a single abstract method. Functional interfaces are used as the basis for lambda expressions and method references, which allow you to create anonymous functions and pass them as arguments to other methods.

    - Lambda
        - A lambda expression is an anonymous function that can be created and passed as an argument to a method. It is defined using the -> operator, and consists of a parameter list and a body. The parameter list specifies the input to the lambda expression, and the body defines the actions that the lambda expression performs.

## String API
    The String API is a set of classes and methods that allow developers to work with strings in Java. The String class is one of the most commonly used classes in the Java API, and it provides a number of methods for manipulating strings, such as concatenating, comparing, and searching for substrings. Some of the key methods in the String API include length(), charAt(), indexOf(), substring(), and trim().

    In addition to the String class, the Java API also provides a number of other classes and interfaces that are related to working with strings, such as the StringBuilder class, which allows developers to efficiently modify strings, and the CharSequence interface, which provides a common set of methods for working with characters.

## Exception

## Checked and Unchecked Exceptions

## Exception Handling/Declaring

## Custom Exception

## Maven

## Project Coordinate

## JSON

## Javalin
