# Java
* Java is a popular programming language that is used for developing a wide range of applications. It is a class-based, object-oriented language that is designed to be easy to use and easy to read. It was originally developed by Sun Microsystems and is now owned by Oracle Corporation. Java is used for developing a variety of applications, including mobile and web applications, games, and more. It is known for its platform independence, which means that Java programs can run on any platform that supports the Java virtual machine.

## The Four Pillars of Object-Oriented Programming

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
    - It is a programming concept that refers to the ability of a single entity, such as a variable, a function, or an object, to have multiple forms. Polymorphism allows for entities to be treated as a single type, even if they have different underlying forms. This can be useful for creating flexible and modular code that is easy to maintain and extend. There are two main types of polymorphism: static and dynamic polymorphism. Static polymorphism is achieved through method overloading, which allows for multiple methods with the same name but different parameters to be defined in the same class. Dynamic polymorphism is achieved through method overriding, which allows a subclass to override the behavior of a superclass method. This allows the same method call to behave differently depending on the type of object on which it is called.

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

* Stack
    - In Java, the stack is a region of memory that is used to store local variables and function parameters, as well as for storing the return address of a function when it is called. When a Java program is executed, the Java Virtual Machine (JVM) creates a stack for each thread that is used to execute the program. Data that is stored in the stack has a fixed size, and is allocated and de-allocated in a last-in-first-out (LIFO) manner. Where the most recently added item is the first one to be removed. This means that when a function is called, its parameters and local variables are added to the top of the stack, and when the function returns, these variables are removed from the stack.

    - One important property of the stack is that it is limited in size. This means that if a program tries to add too many items to the stack, it will run out of memory and will throw a StackOverflowError. This can occur if a program has a lot of recursive function calls or if there is an infinite loop that adds items to the stack without removing them.

    - The stack is an important part of the Java runtime environment and is used to store and manage the execution of a Java program. It is a crucial component of the Java Virtual Machine and plays a vital role in the execution of a Java program.

* Heap
    - In Java, the heap is a region of memory that is used to store objects. When a Java program is executed, the Java Virtual Machine (JVM) creates a heap that is shared by all threads running in the program. It is used to store objects that are created during the execution. When an object is created using the new operator, it is allocated space on the heap and a reference to the object is returned. The object remains on the heap until it becomes eligible for garbage collection, at which point it is removed from the heap and the memory it occupies is made available for reuse.

    - One important property of the heap is that it is not limited in size. This means that a Java program can create as many objects as it needs, as long as there is sufficient memory available on the heap. However, if the heap becomes full and there is no more memory available, the program will throw an OutOfMemoryError.

    - The heap is an important part of the Java runtime environment because it is a region of memory that is used for dynamically allocating memory at runtime. It is used to store and manage the objects that are created during the execution of a Java program.

* In general, the stack is faster and more efficient than the heap, but has the disadvantage of having a fixed size, which makes it more limited in terms of the amount of data that can be stored. The heap, on the other hand, is more flexible in terms of memory usage, but is slower and less efficient than the stack.

## Garbage Collector

* In Java, the garbage collector is a part of the Java Virtual Machine (JVM) that is responsible for reclaiming memory that is no longer being used by the program. The garbage collector runs in the background, monitoring the objects that are stored on the heap (a region of memory used to store objects in Java). When an object becomes eligible for garbage collection, the garbage collector removes the object from the heap and reclaims the memory that it occupies. The garbage collector works by identifying objects that are no longer reachable by the program. An object is considered reachable if there is a reference to it from another object that is itself reachable. If an object is not reachable, it is eligible for garbage collection.

* There are several different algorithms that the JVM can use to perform garbage collection, but the most common one is the mark-and-sweep algorithm. This algorithm works by first marking all of the objects that are still in use, and then sweeping through the heap and deleting any objects that were not marked. Other variety of algorithms to identify unreachable objects and reclaim their memory used by the garbage collector aside from mark-and-sweep include reference counting, and generational garbage collection.

* This can make it easier to write programs, as the programmer does not have to worry about explicitly freeing up memory when it is no longer needed. However, garbage collection can also introduce overhead, as the JVM must periodically pause the program to perform garbage collection.

* It's also important to note that the garbage collector is not a silver bullet for managing memory in a Java program. There are still a number of best practices that programmers should follow to ensure that their programs use memory efficiently, such as avoiding holding onto references to objects that are no longer needed and minimizing the number of objects that are created.

## Method & Parameters

* Method
    - is a block of code that performs a specific task. Methods are defined within a class, and can be called from other parts of the program to execute the task that they define. Methods are used to modularize and organize code, making it easier to reuse and maintain.

    - syntax:
    ```
    [access modifier] [non-access modifier] [return type] [method name]([parameter list]) {
        // method body
    }
    ```

    - access modifier and non-access modifier are swappable

    - A method has a name, a return type, and a list of parameters. The name of the method is used to identify the method and call it from other code. The return type specifies the data type of the value that the method returns, or void if the method does not return a value. The parameters are used to pass information to the method, and can have their own data types and names.

* Parameters
    - is a variable that is passed to a method as an argument when the method is called. The parameter is used to pass information and it allows the method to perform its task using the supplied information.

## Main() Method
```java
public static void main(String[] args) {
    // main method body
}
```
* The main() method is the entry point of a Java program. It is a special method that is called when the program is executed, and it is where the program's code begins to execute. The main() method takes an array of strings as an argument. This array can be used to pass command line arguments to the program. It must be marked as "public", so it can be called from outside the class which it is defined. It must also be marked as "static", so it can be called without created and instance of the class. Then have the "void" keyword so it does not return a value.

## Constructor

* a constructor is a special type of method that is used to create and initialize an object. Every class has at least one constructor, and a class can have multiple constructors with different parameter lists. A constructor has the same name as the class, and does not have a return type.
```
[access modifier] [class name]([parameter list]) {
  // constructor body
  // uses this keyword
}
```

## Variable Scope

* Local or Block Scope
    - These are variables that are defined within a method or a block of code. They are only accessible within the block in which they are defined and are not visible to other parts of the program.
    ```java
    public class Example {
        
        public static void main(String[] args) {
            int x = 10; // local variable x
            System.out.println(x);

            {
                int y = 20; // local variable y
                System.out.println(y);
            }

            System.out.println(y); // error: y is not visible here
        }
    }
    ```

* Instance or Object Scope
    - This a variable that is defined at the class level, outside of any method or block of code. It is associated with an instance of a class and is accessible to all methods of the class. Instance variables are created when an instance of a class is created and are destroyed when the instance is garbage collected. They are stored in the memory heap, which is shared among all instances of a class.

    ```java
    public class Example {

        int x; // instance variable x

        public void setX(int value) {
            x = value;
        }

        public int getX() {
            return x;
        }
    }
    ```
    ```java
    public class Main {

        public static void main(String[] args) {
            Example ex1 = new Example();
            ex1.setX(10);
            System.out.println(ex1.getX()); // prints 10

            Example ex2 = new Example();
            ex2.setX(20);
        System.out.println(ex2.getX()); // prints 20
        }
    }
    ```

* Static or Class Scope
    - uses "Static" keyword. The static variables and methods are associated with a class, rather than with an instance of the class. This means that they are shared among all instances of the class, and it is not visible or accessible to the code outside of that class.


    ```java
    class MyClass {

        static int x = 0;  // static variable with class scope

        static void incrementX() {  // static method with class scope
            x++;
        }
    }
    ```
    ```java
    // same package
    public class Main {

    public static void main(String[] args) {
        int y = MyClass.x;  // access static variable x from outside the class
        MyClass.incrementX();  // call static method incrementX from outside the class
        }
    }
    ```

* Global Scope
    - variables and methods are accessible anywhere in the program
  
    ```java
    // public allows the class to be declared anywhere in the program
    Public class Example {

        static int x = 0; // static variable with class scope, having the class declared as public makes it a global variable

        static void methodOne() { // static method with class scope, having the class declared as public makes it a global variable
            x += 2;
        }
    }
    ```



## Access Modifiers
* the term "access modifier" refers to a keyword that is used to control the visibility and accessibility of class members (variables and methods). The four access modifiers in Java are public, private, protected, and default (no keyword).

  * Public
        - The *public* access modifier indicates that a class member is visible and accessible from anywhere within the program. A class member with the public access modifier can be accessed and modified by any code that has a reference to the class in which the member is defined.

  * Private
        - The *private* access modifier indicates that a class member is only visible and accessible within the class in which it is defined. A class member with the private access modifier cannot be accessed or modified by code outside of the class.

  * Protected
        - The *protected* access modifier indicates that a class member is visible and accessible within the package, class in which it is defined, and also to subclasses of that class. A class member with the protected access modifier cannot be accessed or modified by code outside of the class or its subclasses.

  * Default
        - The *default* access modifier, also known as package-private or **no modifier**, indicates that a class member is visible and accessible within the package in which it is defined, but is not visible or accessible to code outside of the package. A class member with the default access modifier cannot be accessed or modified by code outside of the package in which it is defined.
        - 
## Non-access Modifiers

* Final
    - The final keyword can be applied to classes, fields, methods, and constructors. When applied to a class, it indicates that the class cannot be subclassed. When applied to a field, it indicates that the field cannot be modified once it has been initialized. When applied to a method, it indicates that the method cannot be overridden by a subclass. When applied to a constructor, it indicates that the constructor cannot be called from a subclass.

* Static
    - A field or method that is marked as static belongs to the class itself, rather than to any particular instance of the class. This means that it can be accessed and modified directly, without the need to create an instance of the class.

* Abstract
    - The *abstract* keyword used to indicate that a class or method is incomplete and must be implemented or overridden by a subclass. An abstract class is a class that is marked as abstract and cannot be instantiated. An abstract class can contain both abstract and concrete methods (methods with a body). Abstract methods are methods that are marked as abstract and do not have a body. They must be implemented or overridden by a subclass.

* Interface
    - an *interface* is a type that defines a set of abstract methods and variables. It is similar to a class, but does not contain any implementation. Instead, it defines a set of methods and variables that must be implemented or defined by a class that implements the interface. An interface is declared using the interface keyword, followed by the name of the interface and the list of methods and variables that it defines. All methods and variables in the interface are implicitly public and abstract, and cannot have any implementation code.

* Transient
    - the *transient* keyword is a non-access modifier that is used to indicate that a field should not be serialized (saved) when an object is persisted to storage. Serialization is the process of converting an object into a stream of bytes that can be stored or transmitted over a network. When an object is serialized, all of its fields are included in the serialized data. A field that is marked as transient is not included in the serialized data, and its value is not persisted when the object is saved.

* Volatile
    - the *volatile* keyword is a non-access modifier that is used to indicate that a field can be modified concurrently by multiple threads and should be read from main memory, rather than from a thread-local cache. In a multithreaded program, each thread can have its own local cache of variables that are accessed frequently. This can improve performance by reducing the number of accesses to main memory, but it can also cause problems if the value of a variable in a thread's local cache is not updated when the variable is modified by another thread. The volatile keyword is used to prevent this problem by ensuring that the value of a volatile field is always read from main memory, rather than from a thread-local cache. This ensures that the value of the field is always the most up-to-date value, even if it has been modified concurrently by another thread.

* Synchronized
    - the synchronized keyword is a non-access modifier that is used to synchronize the execution of a method or block of code. When a method or block of code is marked as synchronized, it can only be executed by one thread at a time. This can be useful for preventing race conditions, which can occur when multiple threads try to access and modify shared data concurrently.

* Native
    - the *native* keyword is a non-access modifier that is used to indicate that a method is implemented in native code (i.e., code written in a language other than Java). A native method is a method does not have an implementation in Java. Instead, it has a corresponding implementation in native code, which can be written in a language such as C or C++. Native methods are often used to access system-level functionality or to perform operations that are more efficient in native code.

## Package and Imports

* Package
    - In Java, a *package* is a collection of related classes and interfaces that are bundled together and given a common name. Packages are used to organize and structure the code in a Java program, and to prevent naming conflicts between different classes and interfaces. Packages are an important part of the Java language, and are used to organize and structure the code in a Java program. They are often used to group related classes and interfaces together and to prevent naming conflicts between different classes and interfaces.

* Import
    - In Java, the *import* keyword is used to include a class or interface from a package in the code. By using the import keyword, you can access and use the classes and interfaces from other packages in the code, without having to specify the fully qualified name of the class or interface. It is often used to access and use the classes and interfaces from the Java standard library and other external libraries in your code.

## Functional Interface & Lambda

* Functional Interface
    - a functional interface is an interface that has a single abstract method (SAM). A functional interface is used to represent a function as an object, and is often used in conjunction with lambda expressions, method references, and streams. To define a functional interface, you use the @FunctionalInterface annotation. Functional interfaces are used as the basis for lambda expressions and method references, which allow you to create anonymous functions and pass them as arguments to other methods.

* Lambda
    - a lambda is an expression of an anonymous function that can be used to create objects of functional interfaces. A lambda expression consists of a list of parameters, the -> operator, and a body. The parameters are the inputs to the lambda expression, and the body is the code that is executed when the lambda expression is called. Lambda expressions are often used to pass a function as an argument to a method.

## Generics

* In Java, generics are a feature that allows you to define classes, interfaces, and methods that work with any type, rather than being restricted to a specific type. Generics are used to create reusable and flexible code that can be used with multiple types, while still providing type safety. To define a generic class, interface, or method, you use a type parameter, which is a placeholder for a specific type that will be provided when the class, interface, or method is used.

    ```java
    class MyClass<T> {  // generic class with a type parameter T

        T value;  // field of type T

        MyClass(T value) {  // constructor with a parameter of type T
            this.value = value;
        }

        T getValue() {  // method that returns a value of type T
            return value;
        }
    }
    ```
    ```java
    class Main {

        void test() {
            MyClass<String> obj = new MyClass<>("hello");  // creates an instance of MyClass with T=String
            String value = obj.getValue();  // okay, getValue() returns a String
        }
    }
    ```


## String API

* In Java, the String class is a final class in the java.lang package that represents a string of characters. The String class has a number of methods that are used to manipulate and transform strings. These methods are known as the String API. The String API is a set of classes and methods that allow developers to work with strings in Java. The String class is one of the most commonly used classes in the Java API, and it provides a number of methods for manipulating strings, such as concatenating, comparing, and searching for substrings.

    - Here are some common methods in the String API:

    `length()` This method returns the length of the string.
    `charAt(int index)` This method returns the character at the specified index in the string.
    `indexOf(String str)` This method returns the index of the first occurrence of the specified string in the original string, or -1 if the string is not found.
    `substring(int beginIndex, int endIndex)` This method returns a new string that is a substring of the original string, starting at the specified begin index and ending at the specified end index.
    `toLowerCase()` This method returns a new string with all the characters in the original string converted to lower case.
    `toUpperCase()` This method returns a new string with all the characters in the original string converted to upper case.
    `trim()` This method returns a new string with leading and trailing whitespace removed.
    `replace(char oldChar, char newChar)` This method returns a new string with all occurrences of the specified old character replaced with the specified new character.
    `split(String regex)` This method splits the string into an array of strings based on the specified regular expression.

    - In addition to the String class, the Java API also provides a number of other classes and interfaces that are related to working with strings, such as the StringBuilder class, which allows developers to efficiently modify strings, and the CharSequence interface, which provides a common set of methods for working with characters.

## Exception

* Exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions. When an exception occurs, the Java runtime system creates an exception object that contains information about the error, including its type and the state of the program when the error occurred.

* Exceptions can be thrown by the Java runtime system or by your own code. For example, if you try to divide a number by zero, the Java runtime system will throw an exception. Similarly, if you try to access an array element with an index that is out of bounds, the runtime system will throw an exception.

* Exceptions are represented by classes in the Java language. The Java API provides a hierarchy of exception classes, which are derived from the base class Throwable. There are two main types of exceptions in Java: checked exceptions and unchecked exceptions.

# Throwable

* In Java, Throwable is a class that represents the base class for all exceptions and errors. It is the superclass of all classes that can be thrown by the Java runtime system or by your own code. 

* Throwable has two subclasses: Exception and Error. Exception represents exceptional conditions that a well-written program should anticipate and handle. Error represents serious problems that should not be caught by your program, but rather should be handled by the Java runtime system.

* Throwable has two main methods: getMessage() and printStackTrace(). The getMessage() method returns a string that describes the error, and the printStackTrace() method prints the stack trace to the standard error stream.

## Checked and Unchecked Exceptions

* A *checked exception* is an exception that the Java compiler forces you to handle in your code. Checked exceptions are those that extend the Exception class, which is a subclass of Throwable. When a method throws a checked exception, it must either catch the exception in a try-catch block or declare the exception in the method's throws clause. If a method declares a checked exception in its throws clause, the calling method must either catch the exception or declare it in its own throws clause. This continues up the call stack until the exception is caught or until it reaches the top of the stack, at which point the program will terminate.

* Checked exceptions are intended to represent exceptional conditions that a well-written program should anticipate and handle. For example, an IOException might be thrown when a program attempts to read from a file and the file is not found. This is a condition that a well-written program should anticipate and handle.

* An *unchecked exception* is an exception that the Java compiler does not force you to handle in your code. Unchecked exceptions are those that extend the **RuntimeException** class, which is a subclass of Throwable. If an unchecked exception is thrown and not caught, it will propagate up the call stack until it is caught by an appropriate try-catch block or until it reaches the top of the call stack, at which point the program will terminate.

* Unchecked exceptions are intended to represent exceptional conditions that are internal to the program and that the programmer cannot reasonably be expected to anticipate or prevent. For example, an ArrayIndexOutOfBoundsException might be thrown when a program attempts to access an array element with an index that is out of bounds. This is a condition that is internal to the program and that the programmer cannot reasonably be expected to anticipate or prevent.

## Exception Handling

* Try-Catch Block
    - the try-catch block is a mechanism for handling exceptions. It consists of a try block followed by one or more catch blocks. The try block contains code that might throw an exception. If an exception is thrown, execution of the try block is terminated and control is transferred to the appropriate catch block. If no exception is thrown, the try block is executed to completion and the catch blocks are skipped.

    - If the exception is not of any of the specified types, it will propagate up the call stack until it is caught by an appropriate try-catch block or until it reaches the top of the call stack, at which point the program will terminate.

    - You can also include a finally block after the catch blocks to specify code that should be executed regardless of whether an exception is thrown. The finally block is optional, but if included, it will always be executed whether an exception is thrown or not.

```java
try {
// code that might throw an exception
} catch (ExceptionType1 e) {
// code to handle ExceptionType1
} catch (ExceptionType2 e) {
// code to handle ExceptionType2
} finally {
// code to be executed regardless of whether an exception is thrown
}
```

## Exception Declaring

* Exception declaring is a mechanism for handling exceptions that may be thrown by a method. When a method throws an exception, it must either catch the exception in a try-catch block or declare the exception in the method's throws clause. To declare an exception in a method's throws clause, you can use the throws keyword followed by the exception class.


```java
public void doSomething() throws IOException {
   // code that might throw an IOException
}
```

* If an IOException is thrown, it must be caught by the calling method or declared in the calling method's throws clause. This continues up the call stack until the exception is caught or until it reaches the top of the stack, at which point the program will terminate.

* Declaring an exception in a method's throws clause is necessary for checked exceptions, which are those that extend the Exception class. Checked exceptions are those that the Java compiler forces you to handle in your code. If a method throws a checked exception and does not catch it or declare it in its throws clause, the Java compiler will generate an error.

*Declaring exceptions in a method's throws clause is an important part of exception handling in Java, as it allows you to communicate to the calling method that an exception may be thrown and that the calling method should be prepared to handle it.

### throw

* throw is a keyword that is used to explicitly throw an exception

### throws

* throws is a keyword that is used in the method signature to declare an exception that may be thrown by the method

## Custom Exception

```java
public class MyException extends Exception {
   // constructor and other methods
}
```
```java
try {
   // code that might throw a custom exception
   if (someErrorCondition) {
      throw new MyException("Error message");
   }
} catch (MyException e) {
   // code to handle the custom exception
}
```

## Exception Hierarchy

```java
Throwable
  |
  +-- Exception
  |     |

```
**Checked Exceptions**
```java
Throwable
  |
  +-- Exception
  |     |
  |     +-- IOException
  |     |
  |     +-- SQLException
  |     |
  |     +-- ReflectiveOperationException
  |     |     |
  |     |     +-- ClassNotFoundException
  |     |     |
  |     |     +-- NoSuchFieldException
  |     |     |
  |     |     +-- NoSuchMethodException
```
**Unchecked Exceptions**
```java
Throwable
  |
  +-- Exception
  |     |
  |     +-- RuntimeException
  |           |
  |           +-- ArithmeticException
  |           |
  |           +-- ArrayIndexOutOfBoundsException
  |           |
  |           +-- ArrayStoreException
  |           |
  |           +-- ClassCastException
  |           |
  |           +-- EnumConstantNotPresentException
  |           |
  |           +-- IllegalArgumentException
  |           |
  |           +-- IllegalMonitorStateException
  |           |
  |           +-- IllegalStateException
  |           |
  |           +-- IllegalThreadStateException
  |           |
  |           +-- IndexOutOfBoundsException
  |           |
  |           +-- NegativeArraySizeException
  |           |
  |           +-- NullPointerException
  |           |
  |           +-- NumberFormatException
  |           |
  |           +-- SecurityException
  |           |
  |           +-- StringIndexOutOfBoundsException
  |           |
  |           +-- TypeNotPresentException
  |           |
  |           +-- UnsupportedOperationException
```
**ERRORS**
```java
Throwable
  |
  +-- Error
        |
        +-- AbstractMethodError
        |
        +-- ExceptionInInitializerError
        |
        +-- IllegalAccessError
        |
        +-- InstantiationError
        |
        +-- InternalError
        |
        +-- LinkageError
        |     |
        |     +-- ClassCircularityError
        |     |
        |     +-- ClassFormatError
        |     |
        |     +-- NoClassDefFoundError
        |
        +-- NoSuchFieldError
        |
        +-- NoSuchMethodError
        |
        +-- OutOfMemoryError
        |
        +-- StackOverflowError
```


## Maven

* Apache Maven is a build automation tool used primarily for Java projects. It provides a way to manage project dependencies, build the project, and run tests.

* Maven uses a declarative approach to building projects, meaning that you describe the project and its dependencies in a simple configuration file called pom.xml (short for "Project Object Model"). Maven then takes care of downloading the necessary dependencies, building the project, and performing other tasks as specified in the pom.xml file. In addition to its build automation capabilities, Maven can also be used to manage a project's documentation, reporting, and release process. It has a large and active community of users and developers, and is widely used in the Java development community.

## Project Coordinate

* a project coordinate is a set of values that uniquely identifies a project. It consists of three elements: a group ID, an artifact ID, and a version number.

    - The group ID is a string that identifies the group or organization that owns the project. It typically follows the reverse domain name notation, such as com.example.myproject.
    - The artifact ID is a string that identifies the project within the group. It should be unique within the group and is often the same as the project's name.
    - The version number is a string that identifies a specific version of the project. It is typically in the format x.y.z, where x, y, and z are integers.

* Together, the group ID, artifact ID, and version number form a unique identifier for a project and are referred to as the project's coordinates. They are used to identify the project when it is added as a dependency to another project or when it is deployed to a repository.

    ```
    <groupId>com.example</groupId>
    <artifactId>demo</artifactId>
    <version>1.0.0</version>
    ```

* These coordinates would identify a project named "demo" that is owned by the group or organization "com.example" and is at version "1.0.0".

## Javalin

* Javalin is a lightweight, web framework for Java and Kotlin that is designed to be simple, easy to use, and easy to set up. It provides a set of APIs and tools for building web applications, REST APIs, and microservices. One of the key features of Javalin is its simplicity. It has a small and concise API, with only a few core classes and methods. This makes it easy to learn and use, and allows you to get started with building web applications quickly. Javalin is built on top of the Java Servlet API, which means it can run in any servlet container, such as Tomcat or Jetty. It also supports embedding in other Java applications, such as Spring Boot.

* Javalin is open source and has an active community of users and contributors. It is well-documented and has a number of examples and tutorials to help you get started.

## JSON

* JSON (JavaScript Object Notation) is a lightweight, text-based data interchange format that is easy for humans to read and write and easy for machines to parse and generate. It is based on a subset of the JavaScript programming language and is widely used as a data interchange format for transmitting data over the internet.

* A JSON object is a collection of key-value pairs, where the keys are strings and the values can be any of a number of data types, including strings, numbers, booleans, arrays, and other objects. JSON objects are represented as a set of curly braces containing a comma-separated list of key-value pairs.

* JSON is often used to transmit data between a server and a web application, or between two web applications. It is also used for storing and exchanging data in databases and for configuring applications.