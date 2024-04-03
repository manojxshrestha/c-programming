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


# Topics to be covered :
<hr>
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

**1. Program to display "Hello, World!" on the screen:**


```
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
```
**2. Program to read an integer from the user and display it back:**

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

**3. Program to calculate the area of a rectangle using user input:**

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

**4. Program to convert temperature from Celsius to Fahrenheit:**
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

**5. Program to calculate the sum of two numbers entered by the user:**

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

**These programs cover basic concepts like declaring variables, using different data types, taking input from the user, and displaying output.**

# Chapter 2: Topics including instructions and operators:

**6. Program to calculate the area of a circle using radius:**

```
#include <stdio.h>

int main() {
    float radius, area;
    printf("Enter radius of the circle: ");
    scanf("%f", &radius);
    area = 3.14 * radius * radius;
    printf("Area of the circle: %.2f\n", area);
    return 0;
}
```

**7. Program to check whether a number is even or odd:**

```
#include <stdio.h>
int main() {
    int num;
    printf("Enter an integer: ");
    scanf("%d", &num);
    if (num % 2 == 0) {
        printf("%d is even.\n", num);
    } else {
        printf("%d is odd.\n", num);
    }
    return 0;
}
```

**8. Program to find the maximum of two numbers:**

```
#include <stdio.h>
int main() {
    int num1, num2, max;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    max = (num1 > num2) ? num1 : num2;
    printf("Maximum number: %d\n", max);
    return 0;
}
```

**9. Program to swap two numbers using a temporary variable:**

```
#include <stdio.h>

int main() {
    int num1, num2, temp;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    temp = num1;
    num1 = num2;
    num2 = temp;
    printf("After swapping: \nFirst number: %d\nSecond number: %d\n", num1, num2);
    return 0;
}
```

**10. Program to check whether a year is a leap year or not:**

```
#include <stdio.h>
int main() {
    int year;
    printf("Enter a year: ");
    scanf("%d", &year);
    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        printf("%d is a leap year.\n", year);
    } else {
        printf("%d is not a leap year.\n", year);
    }
    return 0;
}
```
**These programs demonstrate basic control structures like if-else statements and the use of arithmetic and comparison operators**


# Chapter 3: Topics including conditional statements:

**11. Program to find the largest among three numbers**

```
#include <stdio.h>
int main() {
    int num1, num2, num3;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &num1, &num2, &num3);
    
    if (num1 >= num2 && num1 >= num3) {
        printf("%d is the largest.\n", num1);
    } else if (num2 >= num1 && num2 >= num3) {
        printf("%d is the largest.\n", num2);
    } else {
        printf("%d is the largest.\n", num3);
    }
    return 0;
}
```


**12. Program to check whether a number is positive, negative, or zero:**

```
#include <stdio.h>
int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);
    if (num > 0) {
        printf("%d is positive.\n", num);
    } else if (num < 0) {
        printf("%d is negative.\n", num);
    } else {
        printf("The number is zero.\n");
    }
    return 0;
}
```

**13. Program to check whether a character is a vowel or consonant:**

```
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    scanf(" %c", &ch);
    
    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
        ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
        printf("%c is a vowel.\n", ch);
    } else {
        printf("%c is a consonant.\n", ch);
    }
    return 0;
}
```

**14.Program to check whether a year is a leap year or not using conditional operator:**

```
#include <stdio.h>
int main() {
    int year;
    printf("Enter a year: ");
    scanf("%d", &year);
    (year % 4 == 0 && year % 100 != 0) || (year % 400 == 0) ? printf("%d is a leap year.\n", year) : printf("%d is not a leap year.\n", year);
    return 0;
}
```

**15.Program to find the maximum of two numbers using conditional operator:**
```
#include <stdio.h>
int main() {
    int num1, num2, max;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    max = (num1 > num2) ? num1 : num2;
    printf("Maximum number is: %d\n", max);
    return 0;
}
```
**These programs illustrate the use of if-else statements and conditional operators for decision-making in C programming.**


# Chapter 4: Topics including loop control statements:

**16. Program to print numbers from 1 to 10 using a while loop:**

```
#include <stdio.h>
int main() {
    int i = 1;
    printf("Numbers from 1 to 10: ");
    while (i <= 10) {
        printf("%d ", i);
        i++;
    }
    printf("\n");
    return 0;
}
```

**17. Program to calculate the factorial of a number using a for loop:**

```
#include <stdio.h>
int main() {
    int num, factorial = 1;
    printf("Enter a positive integer: ");
    scanf("%d", &num);
    for (int i = 1; i <= num; i++) {
        factorial *= i;
    }
    printf("Factorial of %d: %d\n", num, factorial);
    return 0;
}
```

**18. Program to print Fibonacci series up to a given number using a while loop:**

```
#include <stdio.h>
int main() {
    int limit, num1 = 0, num2 = 1, nextTerm;
    printf("Enter the limit of Fibonacci series: ");
    scanf("%d", &limit);    
    printf("Fibonacci series up to %d: ", limit);
    while (num1 <= limit) {
        printf("%d, ", num1);
        nextTerm = num1 + num2;
        num1 = num2;
        num2 = nextTerm;
    }
    printf("\n");
    return 0;
}
```

**19. Program to find the sum of natural numbers from 1 to n using a for loop:**

```
#include <stdio.h>
int main() {
    int n, sum = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);    
    for (int i = 1; i <= n; i++) {
        sum += i;
    }
    printf("Sum of natural numbers from 1 to %d: %d\n", n, sum);
    return 0;
}
```

**20. Program to check whether a number is prime or not using a for loop:**

```
#include <stdio.h>
int main() {
    int num, isPrime = 1;
    printf("Enter a positive integer: ");
    scanf("%d", &num);
    for (int i = 2; i <= num / 2; i++) {
        if (num % i == 0) {
            isPrime = 0;
            break;
        }
    }
    if (num <= 1 || !isPrime) {
        printf("%d is not a prime number.\n", num);
    } else {
        printf("%d is a prime number.\n", num);
    }
    return 0;
}
```

**These programs demonstrate the usage of different loop control statements such as while loop and for loop for iterating over a range of values, performing calculations, and checking conditions repeatedly.**






