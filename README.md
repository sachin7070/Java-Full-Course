# Java ♨️ Full Course

Welcome to the comprehensive **Java** course! In this course, you will learn everything you need to know about the Java programming language, from the basics to advanced topics. Each section includes detailed explanations, examples, and outputs to help you understand and practice Java programming effectively.

## Table of Contents 📝

1. [Introduction to Java](#1-introduction-to-java)  
2. [Flowcharts and Pseudocode](#2-flowcharts-and-pseudocode)  
3. [Variables and Data Types](#3-variables-and-data-types)  
4. [Operators](#4-operators)  
5. [Conditional Statements](#5-conditional-statements)  
6. [Loops (Control Flow)](#6-loops-control-flow)  
7. [Patterns](#7-patterns)  
8. [Functions and Methods](#8-functions-and-methods)  
9. [Arrays](#9-arrays)  
10. [Sorting](#10-sorting)  
11. [Strings](#11-strings)  
12. [Bit Manipulation](#12-bit-manipulation)  
13. [Object-Oriented Programming (OOP)](#13-object-oriented-programming-oop)  
14. [Recursion](#14-recursion)  
15. [Divide and Conquer](#15-divide-and-conquer)  
16. [Time Complexity](#16-time-complexity)  
17. [Backtracking](#17-backtracking)  
18. [ArrayLists](#18-arraylists)  
19. [Linked Lists](#19-linked-lists)  
20. [Stacks](#20-stacks)  
21. [Queues](#21-queues)  
22. [Greedy Algorithms](#22-greedy-algorithms)  
23. [Binary Trees](#23-binary-trees)  
24. [Binary Search Trees (BST)](#24-binary-search-trees-bst)  
25. [Heaps](#25-heaps)  
26. [Hashing](#26-hashing)  
27. [Tries](#27-tries)  
28. [Graphs](#28-graphs)  

---

## 1. Introduction to Java

Java is a high-level, object-oriented programming language developed by Sun Microsystems in 1995 (now owned by Oracle). Known for its platform independence, Java allows developers to "write once, run anywhere" through the use of the Java Virtual Machine (JVM). It is widely used for building everything from web and mobile applications to large-scale enterprise systems.

---

## 2. Flowcharts and Pseudocode

Flowcharts and pseudocode are tools that help in visualizing and planning algorithms before coding. These are essential for understanding logic and problem-solving.

---

## 3. Variables and Data Types

### 1. Variables in Java

#### Definition:
A variable is a container that holds data during the execution of a program. Each variable must be assigned a data type before it can be used. Variables store data that can be modified and reused later in the code.

Syntax:
```java
dataType variableName = value;
```
Example:
```java
int age = 25;       // 'age' is a variable of type int holding the value 25
String name = "John"; // 'name' is a variable of type String holding the value "John"
```
### Types of Variables:
### Local Variables:
Declared inside methods, constructors, or blocks and only accessible within that scope.

Example:
```java
public void show() {
    int x = 10; // local variable, only accessible within this method
}
```
### Instance Variables:
Declared inside a class but outside methods, constructors, or blocks. They belong to an instance of the class.

Example:
```java
class Person {
    String name; // instance variable
}
```
### Static Variables: 
Declared with the static keyword inside a class but outside methods. They are shared among all instances of the class.

Example:
```java
class Company {
    static String companyName = "TechCorp"; // static variable shared by all objects
}
```
###  Data Types in Java
Java has two main categories of data types: Primitive Data Types and Non-Primitive (Reference) Data Types.

### Primitive Data Types
Primitive data types are predefined by Java and serve as the building blocks of data manipulation. There are 8 primitive data types in Java.

| Data    | Type    | Size      | Default Value | Description                                                     |
|---------|---------|-----------|---------------|-----------------------------------------------------------------|
| `byte`  | Primitive | 1 byte  | 0             | Stores whole numbers from -128 to 127                           |
| `short` | Primitive | 2 bytes | 0             | Stores whole numbers from -32,768 to 32,767                     |
| `int`   | Primitive | 4 bytes | 0             | Stores whole numbers from -2<sup>31</sup> to 2<sup>31</sup>-1   |
| `long`  | Primitive | 8 bytes | 0L            | Stores whole numbers from -2<sup>63</sup> to 2<sup>63</sup>-1   |
| `float` | Primitive | 4 bytes | 0.0f          | Stores fractional numbers. Sufficient for 6 to 7 decimal digits |
| `double`| Primitive | 8 bytes | 0.0d          | Stores fractional numbers. Sufficient for 15 decimal digits     |
| `boolean`| Primitive| 1 bit   | false         | Stores true or false values                                     |
| `char`  | Primitive | 2 bytes | '\u0000'      | Stores a single 16-bit Unicode character                        |

Syntax:
```java
dataType variableName = value;
```
Example:
```java
int num = 100;        // int data type
float temperature = 36.6f; // float data type (suffix 'f' is required)
boolean isJavaFun = true;  // boolean data type
char grade = 'A';     // char data type
```
### Non-Primitive (Reference) Data Types
Non-primitive data types (also known as reference types) refer to objects and can be used to call methods to perform certain operations. These types include classes, arrays, and interfaces.

String: Represents sequences of characters.
Arrays: Stores multiple values of the same type.
Classes: Defines objects and their attributes/methods.
Example:
```java
String greeting = "Hello, World!"; // String reference type
int[] numbers = {1, 2, 3, 4, 5};   // Array reference type
```
### Variable Naming Rules
When naming a variable in Java, there are a few rules to follow:

The name must begin with a letter, dollar sign ($), or an underscore (_).
It cannot start with a digit.
It should be meaningful, avoiding single letters unless for temporary use.
Java is case-sensitive, so age and Age are different variables.
Example:
```java
int $age = 30;
String _name = "Alice";
```
##4. Type Casting
Type casting refers to converting a variable from one data type to another. There are two types:

Implicit (Automatic) Casting: Smaller data types are automatically converted to larger ones.

Example:
```java
int a = 10;
double b = a; // int to double (automatic conversion)
```
Explicit (Manual) Casting: Larger data types are converted to smaller ones manually.

Example:
```java
double x = 9.7;
int y = (int) x; // double to int (manual casting)
```

## 4. Operators

Operators in Java are special symbols or keywords used to perform operations on variables and values. They are essential for performing computations, making decisions, and manipulating data. Java supports several types of operators, which are categorized as follows:

---

### 1. Arithmetic Operators

Arithmetic operators are used to perform basic mathematical operations.

| Operator | Description        | Example          |
|----------|--------------------|------------------|
| `+`      | Addition           | `a + b`          |
| `-`      | Subtraction        | `a - b`          |
| `*`      | Multiplication     | `a * b`          |
| `/`      | Division           | `a / b`          |
| `%`      | Modulus (Remainder)| `a % b`          |

**Example:**
```java
int a = 10, b = 3;
System.out.println(a + b); // Output: 13
System.out.println(a - b); // Output: 7
System.out.println(a * b); // Output: 30
System.out.println(a / b); // Output: 3
System.out.println(a % b); // Output: 1
```
### 2. Relational (Comparison) Operators

Relational operators are used to compare two values and return a boolean result (`true` or `false`).

| Operator | Description                 | Example   |
|----------|-----------------------------|-----------|
| `==`     | Equal to                   | `a == b`  |
| `!=`     | Not equal to               | `a != b`  |
| `>`      | Greater than               | `a > b`   |
| `<`      | Less than                  | `a < b`   |
| `>=`     | Greater than or equal to   | `a >= b`  |
| `<=`     | Less than or equal to      | `a <= b`  |

### Example:
```java
int a = 10, b = 20;
System.out.println(a == b); // Output: false
System.out.println(a != b); // Output: true
System.out.println(a > b);  // Output: false
System.out.println(a < b);  // Output: true
System.out.println(a >= b); // Output: false
System.out.println(a <= b); // Output: true
```
### 3. Logical Operators

Logical operators are used to combine multiple boolean expressions or conditions.

| Operator | Description      | Example                   |
|----------|------------------|---------------------------|
| `&&`     | Logical AND      | `(a > b) && (a < c)`      |
| `||`     | Logical OR       | `(a > b) || (a < c)`      |
| `!`      | Logical NOT      | `!(a > b)`               |

### Example:
```java
int a = 10, b = 20, c = 30;
System.out.println((a > b) && (a < c)); // Output: false
System.out.println((a > b) || (a < c)); // Output: true
System.out.println(!(a > b));          // Output: true
```
## 4. Assignment Operators

Assignment operators are used to assign values to variables.

| Operator | Description        | Example                   |
|----------|--------------------|---------------------------|
| `=`      | Assign             | `a = b`                  |
| `+=`     | Add and assign      | `a += b` (equivalent to `a = a + b`) |
| `-=`     | Subtract and assign | `a -= b` (equivalent to `a = a - b`) |
| `*=`     | Multiply and assign | `a *= b` (equivalent to `a = a * b`) |
| `/=`     | Divide and assign   | `a /= b` (equivalent to `a = a / b`) |
| `%=`     | Modulus and assign  | `a %= b` (equivalent to `a = a % b`) |

### Example:
```java
int a = 10, b = 5;
a += b; // a = a + b (a becomes 15)
System.out.println(a);
a -= b; // a = a - b (a becomes 10)
System.out.println(a);
a *= b; // a = a * b (a becomes 50)
System.out.println(a);
a /= b; // a = a / b (a becomes 10)
System.out.println(a);
a %= b; // a = a % b (a becomes 0)
System.out.println(a);
```
## 5. Bitwise Operators

Bitwise operators operate on bits and perform bit-by-bit operations.

| Operator | Description            | Example       |
|----------|------------------------|---------------|
| `&`      | Bitwise AND            | `a & b`       |
| `|`      | Bitwise OR             | `a | b`       |
| `^`      | Bitwise XOR            | `a ^ b`       |
| `~`      | Bitwise Complement     | `~a`          |
| `<<`     | Left shift             | `a << 2`      |
| `>>`     | Right shift            | `a >> 2`      |

### Example:
```java
int a = 5, b = 3; // Binary: a = 0101, b = 0011
System.out.println(a & b);  // Output: 1 (0101 & 0011 = 0001)
System.out.println(a | b);  // Output: 7 (0101 | 0011 = 0111)
System.out.println(a ^ b);  // Output: 6 (0101 ^ 0011 = 0110)
System.out.println(~a);     // Output: -6 (inverts the bits of 5)
System.out.println(a << 1); // Output: 10 (0101 << 1 = 1010)
System.out.println(a >> 1); // Output: 2 (0101 >> 1 = 0010)
```
## 6. Unary Operators

Unary operators operate on a single operand.

| Operator | Description            | Example              |
|----------|------------------------|----------------------|
| `+`      | Positive               | `+a`                |
| `-`      | Negative               | `-a`                |
| `++`     | Increment              | `++a` or `a++`      |
| `--`     | Decrement              | `--a` or `a--`      |
| `!`      | Logical Complement     | `!a`                |

### Example:
```java
int a = 5;
System.out.println(+a);  // Output: 5
System.out.println(-a);  // Output: -5
System.out.println(++a); // Output: 6 (pre-increment: increments before use)
System.out.println(a++); // Output: 6 (post-increment: increments after use)
System.out.println(--a); // Output: 6 (pre-decrement: decrements before use)
System.out.println(a--); // Output: 6 (post-decrement: decrements after use)
```
### 7. Ternary Operator

The ternary operator is a shorthand for `if-else` statements. It uses the following syntax:

```java
condition ? valueIfTrue : valueIfFalse
```
Example:

```java
int a = 10, b = 20;
int max = (a > b) ? a : b;
System.out.println(max); // Output: 20
```


## 5.Conditional Statements

Conditional statements in Java allow you to control the flow of your program based on certain conditions. The primary conditional statements in Java are `if`, `if-else`, and nested `if-else`.

### 1. `if` Statement

The `if` statement in Java is used to execute a block of code only if a specified condition is true. It has the following syntax:

```java
if (condition) {
    // code to be executed if the condition is true
}
```
Example:

```java
int x = 10;
if (x > 5) {
    System.out.println("x is greater than 5");
}
```

### 2. else if Statement
The else if statement allows you to specify a new condition if the previous condition is false. It allows for multiple conditions to be checked. It has the following syntax:

```java
if (condition1) {
    // code to be executed if condition1 is true
} else if (condition2) {
    // code to be executed if condition2 is true
} else {
    // code to be executed if all conditions are false
}
```
Example:

```java
int y = 20;
if (y > 10) {
    System.out.println("y is greater than 10");
} else if (y < 10) {
    System.out.println("y is less than 10");
} else {
    System.out.println("y is equal to 10");
}
```

### 3. else Statement
The else statement is used to execute a block of code if the condition of the if statement is false. It has the following syntax:

```java
if (condition) {
    // code to be executed if the condition is true
} else {
    // code to be executed if the condition is false
}
```
Example:

```java
int z = 5;
if (z > 10) {
    System.out.println("z is greater than 10");
} else {
    System.out.println("z is not greater than 10");
}
```

### 4. Nested if-else Statement
Nested if-else statements allow you to include one if-else statement inside another. This allows for more complex conditional logic. It has the following syntax:

```java
if (condition1) {
    // code to be executed if condition1 is true
    if (condition2) {
        // code to be executed if both condition1 and condition2 are true
    } else {
        // code to be executed if condition1 is true and condition2 is false
    }
} else {
    // code to be executed if condition1 is false
}
```
Example:

```java
int z = 5;
if (z > 10) {
    System.out.println("z is greater than 10");
} else if (z < 10) {
    System.out.println("z is less than 10");
} else {
    System.out.println("z is equal to 10");
}
```
## Contribution

Contributions to this project are welcome. If you have any suggestions for improvements or new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


