# Java Full Course

Welcome to the comprehensive C++ course! In this course, you will learn everything you need to know about the C++ programming language, from the basics to advanced topics. Each section includes detailed explanations, examples, and outputs to help you understand and practice C++ programming effectively.

## Table of Contents

1. [Introduction to java](#1.Intoduction-to-Java)
2. [Variables and Data Types](#2.Variable-And-Data-Types)
3. [Operator]
4. [Conditional Statement]
5.[loop(Control Flow)]
6.[Pattern]
7.[Function And Method]
8.[Arrays]
9.[Sorting]
10.[String]
11.[Bit Manipulation]
12.[OOPS]

## 1.Introduction to Java
Java is a high-level, object-oriented programming language developed by Sun Microsystems in 1995 (now owned by Oracle). Known for its platform independence, Java allows developers to "write once, run anywhere" through the use of the Java Virtual Machine (JVM). It is widely used for building everything from web and mobile applications to large-scale enterprise systems.

## 2.Varibale And Data Types
### 1. Variables in Java
#### Definition:
A variable is a container that holds data during the execution of a program. Each variable must be assigned a data type before it can be used. Variables store data that can be modified and reused later in the code.

Syntax:
java
Copy code
dataType variableName = value;
Example:
java
Copy code
int age = 25;       // 'age' is a variable of type int holding the value 25
String name = "John"; // 'name' is a variable of type String holding the value "John"
Types of Variables:
Local Variables: Declared inside methods, constructors, or blocks and only accessible within that scope.

Example:
java
Copy code
public void show() {
    int x = 10; // local variable, only accessible within this method
}
Instance Variables: Declared inside a class but outside methods, constructors, or blocks. They belong to an instance of the class.

Example:
java
Copy code
class Person {
    String name; // instance variable
}
Static Variables: Declared with the static keyword inside a class but outside methods. They are shared among all instances of the class.

Example:
java
Copy code
class Company {
    static String companyName = "TechCorp"; // static variable shared by all objects
}
2. Data Types in Java
Java has two main categories of data types: Primitive Data Types and Non-Primitive (Reference) Data Types.

2.1 Primitive Data Types
Primitive data types are predefined by Java and serve as the building blocks of data manipulation. There are 8 primitive data types in Java.

Data Type	Size	Default Value	Description
byte	1 byte	0	Stores whole numbers from -128 to 127
short	2 bytes	0	Stores whole numbers from -32,768 to 32,767
int	4 bytes	0	Stores whole numbers from -2^31 to 2^31-1
long	8 bytes	0L	Stores whole numbers from -2^63 to 2^63-1
float	4 bytes	0.0f	Stores fractional numbers. Sufficient for 6 to 7 decimal digits
double	8 bytes	0.0d	Stores fractional numbers. Sufficient for 15 decimal digits
boolean	1 bit	false	Stores true or false values
char	2 bytes	'\u0000'	Stores a single 16-bit Unicode character
Syntax:
java
Copy code
dataType variableName = value;
Example:
java
Copy code
int num = 100;        // int data type
float temperature = 36.6f; // float data type (suffix 'f' is required)
boolean isJavaFun = true;  // boolean data type
char grade = 'A';     // char data type
2.2 Non-Primitive (Reference) Data Types
Non-primitive data types (also known as reference types) refer to objects and can be used to call methods to perform certain operations. These types include classes, arrays, and interfaces.

String: Represents sequences of characters.
Arrays: Stores multiple values of the same type.
Classes: Defines objects and their attributes/methods.
Example:
java
Copy code
String greeting = "Hello, World!"; // String reference type
int[] numbers = {1, 2, 3, 4, 5};   // Array reference type
3. Variable Naming Rules
When naming a variable in Java, there are a few rules to follow:

The name must begin with a letter, dollar sign ($), or an underscore (_).
It cannot start with a digit.
It should be meaningful, avoiding single letters unless for temporary use.
Java is case-sensitive, so age and Age are different variables.
Example:
java
Copy code
int $age = 30;
String _name = "Alice";
4. Type Casting
Type casting refers to converting a variable from one data type to another. There are two types:

Implicit (Automatic) Casting: Smaller data types are automatically converted to larger ones.

Example:
java
Copy code
int a = 10;
double b = a; // int to double (automatic conversion)
Explicit (Manual) Casting: Larger data types are converted to smaller ones manually.

Example:
java
Copy code
double x = 9.7;
int y = (int) x; // double to int (manual casting)
