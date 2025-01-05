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

## 6.Loops (Control Flow)
Java Loops is a repository containing examples and explanations of loop constructs in Java.

## Table of Contents

- [Introduction](#introduction)
- [Syntax](#syntax)
- [Types of Loops](#types-of-loops)
  - [1. `for` Loop](#1-for-loop)
  - [2. `while` Loop](#2-while-loop)
  - [3. `do-while` Loop](#3-do-while-loop)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In programming, loops are used to execute a block of code repeatedly until a certain condition is met. They help in reducing redundancy and improving code readability by allowing the same set of instructions to be executed multiple times.

This repository provides explanations and examples of various loop constructs available in Java, helping developers understand how to efficiently utilize them in their code.

## Syntax

The basic syntax of a loop in Java consists of an initialization step, a condition, and an increment (or decrement) step. The general structure looks like this:

```java
for (initialization; condition; increment/decrement) {
    // code block to be executed
}
```

```java
while (condition) {
    // code block to be executed
}
```

```java

do {
    // code block to be executed
} while (condition);
```

### Types of Loops
### 1. for Loop
The for loop is used when you know the number of iterations in advance.

Example : for Loop
```java
for (int i = 0; i < 5; i++) {
    System.out.println("Iteration: " + i);
}
```

### 2. while Loop
The while loop is used when you want to execute a block of code repeatedly until a specified condition is false.

Example 2: while Loop
```java
int i = 0;
while (i < 5) {
    System.out.println("Iteration: " + i);
    i++;
}
```

### 3. do-while Loop
The do-while loop is similar to the while loop, but it ensures that the code block is executed at least once before checking the condition.

Example 3: do-while Loop
```java
int i = 0;
do {
    System.out.println("Iteration: " + i);
    i++;
} while (i < 5);
```

## 8.Function and Method

This repository provides a comprehensive reference guide for methods and functions in the Java programming language. Whether you're a beginner looking to understand basic concepts or an experienced developer seeking clarification on advanced features, this guide aims to assist you in navigating through Java's extensive library of methods and functions.

## Table of Contents

1. [Introduction](#introduction)
2. [Basic Methods](#basic-methods)
3. [Standard Library Functions](#standard-library-functions)
4. [Advanced Techniques](#advanced-techniques)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction

Java is a versatile programming language widely used for developing various types of applications, including web, mobile, and enterprise software. Methods and functions play a crucial role in Java programming, allowing developers to organize code into reusable blocks and perform specific tasks efficiently.

## Basic Methods

In Java, a method is a collection of statements that perform a specific task and is defined within a class. Here are some fundamental types of methods:

### Instance Methods

Instance methods are associated with objects of a class and can access instance variables and other instance methods.

```java
public class MyClass {
    int x;

    // Instance Method
    void setX(int newValue) {
        x = newValue;
    }

    public static void main(String[] args) {
        MyClass obj = new MyClass();
        obj.setX(10);
        System.out.println("Value of x: " + obj.x); // Output: 10
    }
}
```
### Static Methods
Static methods belong to the class rather than any specific instance and can be invoked without creating an object of the class.

```java
public class MyClass {
    static int square(int num) {
        return num * num;
    }

    public static void main(String[] args) {
        int result = MyClass.square(5);
        System.out.println("Square of 5: " + result); // Output: 25
    }
}
```
## 9. Arrays

## Introduction to Arrays in Java

Arrays are fundamental data structures in Java, allowing you to store multiple values of the same type in a single variable. An array in Java is a container object that holds a fixed number of values of a single data type. Arrays can be of any data type, including primitive types such as int, char, double, etc., or reference types such as objects.

Arrays in Java are zero-indexed, meaning the index of the first element is 0, the index of the second element is 1, and so on. Arrays have a fixed size, which is determined at the time of their creation and cannot be changed dynamically. However, Java provides dynamic arrays through ArrayList, which can resize itself dynamically.

## Syntax of Arrays in Java

### Declaration:
```java
dataType[] arrayName;
```
Initialization:
```java
dataType[] arrayName = new dataType[arraySize];
```
Example:
```java
// Declaration
int[] numbers;

// Initialization
numbers = new int[5];

// Array Literal Initialization
int[] numbers = {1, 2, 3, 4, 5};
```

Accessing Elements:
```java
arrayName[index];
```
Example:
```java
int[] numbers = {10, 20, 30, 40, 50};
System.out.println(numbers[0]); // Output: 10
System.out.println(numbers[2]); // Output: 30
```

Array Length:
```java
arrayName.length;
```
Example:
```java
int[] numbers = {10, 20, 30, 40, 50};
System.out.println(numbers.length); // Output: 5
```
### Multidimensional Arrays:

Definition: A multidimensional array in Java is an array of arrays. It allows you to store elements in multiple dimensions, such as rows and columns.

Declaration and Initialization:

```java
// Declaration
int[][] matrix;

// Initialization
matrix = new int[3][4]; // Creates a 2D array with 3 rows and 4 columns
```
Accessing Elements:

Elements of a multidimensional array are accessed using multiple indices. For a 2D array, you need two indices: one for the row and one for the column.
```java
matrix[0][0] = 1; // Assigns 1 to the element at the first row and first column
int y = matrix[1][2]; // Retrieves the value of the element at the second row and third column

```
Initialization with Values:

You can initialize a multidimensional array with specific values at the time of declaration.

```java
int[][] matrix = { {1, 2, 3}, {4, 5, 6}, {7, 8, 9} }; // Initializes a 2D array with specific values
```
Ragged Arrays:

In Java, multidimensional arrays can have different lengths for each row. Such arrays are called ragged arrays.
```java
int[][] raggedArray = { {1, 2}, {3, 4, 5}, {6} }; // Initializes a ragged 2D array
```

## Questions and Programs

1.	WAP to create an array of size n
2. 	WAP to calculate sum of all the array elements
3.	WAP to product of all the array elements
4. 	WAP to calculate the difference of sum of even elements and odd elements 
5.	WAP to display all numbers between two given range
6. 	WAP to reverse an array
7.	WAP to find largest element from an array
8. 	WAP to find smallest element from an array
9.    WAP to find the difference of maximum and minimum element of an array
10.	WAP to find the second largest element in an array
11.	WAP to find the second smallest element in an array
12.	WAP to sort an array in ascending order
13.	WAP to sort an array in descending order
14.	WAP to Sort first half in ascending order and second half in descending
15.	WAP to Finding the frequency of elements in an array
16.	WAP to Sorting elements of an array by frequency 
17.	WAP to Finding the Longest Palindrome in an Array
18.	WAP to Counting Distinct Elements in an Array
19.	WAP to Finding  Repeating elements in an Array
20.	WAP to Finding Non Repeating elements in an Array
21.	WAP to Removing Duplicate elements from an array
22.	WAP to Finding Minimum scalar product of two vectors
23.	WAP to Finding Maximum scalar product of two vectors in an array
24.	WAP to Counting the number of even and odd elements in an array
25.	WAP to Find all Symmetric pairs in an array
26.	WAP to Find maximum product sub-array in a given array
27.	WAP to Finding Arrays are disjoint or not
28.	WAP to Determine Array is a subset of another array or not
29.	WAP to Determine can all numbers of an array be made equal
30.	WAP to Finding Minimum sum of absolute difference of given array
31.	WAP to Sort an array according to the order defined by another array
32.	WAP to Replace each element of the array by its rank in the array
33.	WAP to Finding equilibrium index of an array
34.	WAP to left rotate an array by k position
35.	WAP to right rotate an array by k position
36.	WAP to find Balanced Parenthesis 
37.	WAP to sort an array which consists of only 0, 1 and 2.
38.	WAP to Find the “Kth” max and min element of an array
39.	WAP to Move all the negative elements to one side of the array
40.	WAP to Find the Union and Intersection of the two sorted arrays.
41.	WAP to Find Largest sum contiguous Subarray
42.	WAP to Minimize the maximum difference between heights
43.	WAP to Minimum no. of Jumps to reach the end of an array
44.	WAP to Find duplicate in an array of N+1 Integers
45.	WAP to Merge 2 sorted arrays without using extra space
46.	WAP for Kadane’s Algorithm
47.	WAP for Merge Intervals
48.	WAP for Count Inversion
49.	WAP for Best time to buy and Sell stock
50.	WAP to Find all pairs on integer array whose sum is equal to given number
51.	WAP to Find if there is any subarray with sum equal to 0
52.	WAP to Find factorial of a Large Number
53.	WAP to Find common elements In 3 sorted arrays
54.	WAP to Rearrange the array in alternating positive and negative items 
55.	WAP to Find all elements that appear more than ” n/k ” times
56.	WAP to Maximize profit by buying and selling a share at-most twice
57.	WAP to find Next Permutation
58.	WAP to Find longest consecutive subsequence
59.	WAP for Trapping Rain water problem
60.	WAP for Chocolate Distribution problem
61.	WAP to find Smallest Subarray with sum greater than a given value
62.	WAP for Three way partitioning of an array around a given value
63.	WAP that require Minimum no. of operations to make an array palindrome
64.	WAP to find Median of 2 sorted arrays of equal size
65.	WAP to find Median of 2 sorted arrays of different size
66.	WAP to Find a peak element which is not smaller than its neighbours
67.	WAP to Find the missing integer
68.	WAP to Count Pairs with the given sum
69.	WAP to Find a triplet that sums to a given value
70.	WAP for Coin Change Problem
