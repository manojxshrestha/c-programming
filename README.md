# Title: Comprehensive Guide to C Programming: 50 Programs

```
Presented by: Manoj Shrestha
Class: 12
Email: manojxshrestha@gmail.com
College: PNHSS
```

# Introduction:
<hr>
Welcome to my comprehensive guide to learning C programming! Throughout this guide, we’ll explore 50 fundamental programs that will help you become more skilled and knowledgeable in the C programming language.

In this introduction, we’ll give you some background information on why learning C programming is important. We’ll also briefly review some key resources that can help you along the way.

Our goal with this guide is to help you understand C programming better and improve your skills. However, it’s important to note that there may be some limitations to consider as you use this guide.

So, let’s dive in and start exploring the world of C programming together!
<hr>

# Materials & Methods:

To execute the programs outlined in this guide, the following materials and methods are recommended:

Materials:

1. Computer with a C compiler installed (e.g., GCC, Clang)
2. Text editor or integrated development environment (IDE) for writing and editing C code

Methods:

1.Write each program in a text editor or IDE.
2.Save the program with a .c extension (e.g., program1.c).
3.Compile each program using the C compiler installed on your computer.
4. Run the compiled program to observe its output.
5. Debug any errors encountered during compilation or execution.

<hr>
Topics to be covered :

Installation + Setup

Chapter 1 - Variables, Data types + Input/Output

Chapter 2 - Instructions & Operators

Chapter 3 - Conditional Statements

Chapter 4 - Loop Control Statements

Chapter 5 - Functions & Recursion

Chapter 6 - Pointers

Chapter 7 - Arrays

Chapter 8 - Strings

Chapter 9 - Structures

Chapter 10 - File I/O
<hr>


# Chapter 1:  Topics including variables, data types, and input/output:
<hr>
1. Program to display "Hello, World!" on the screen:
<hr>

```
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
```
2. Program to read an integer from the user and display it back:

```
#include <stdio.h>
int main() {
    int num;
    printf("Enter an integer: ");
    scanf("%d", &num);
    printf("You entered: %d\n", num);
    return 0;
}
```

3. Program to calculate the area of a rectangle using user input:

```
#include <stdio.h>
int main() {
    float length, width, area;
    printf("Enter length: ");
    scanf("%f", &length);
    printf("Enter width: ");
    scanf("%f", &width);
    area = length * width;
    printf("Area of rectangle: %.2f\n", area);
    return 0;
}
```

4. Program to convert temperature from Celsius to Fahrenheit:
```
#include <stdio.h>
int main() {
    float celsius, fahrenheit;
    printf("Enter temperature in Celsius: ");
    scanf("%f", &celsius);
    fahrenheit = (celsius * 9 / 5) + 32;
    printf("Temperature in Fahrenheit: %.2f\n", fahrenheit);
    return 0;
}
```

5. Program to calculate the sum of two numbers entered by the user:

```
#include <stdio.h>
int main() {
    int num1, num2, sum;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    sum = num1 + num2;
    printf("Sum: %d\n", sum);
    return 0;
}
```
<hr>
These programs cover basic concepts like declaring variables, using different data types, taking input from the user, and displaying output.
<hr>

