 <center>

# C Programming Essentials in 50 Programs

</center>

![IMG_20240403_181549](https://github.com/manojxshrestha/cs-project/assets/106522935/7314b761-fd59-4aa7-bdd7-dc4446ce18c8)

```
Presented by: Mandira Rimal
Class: 12
College: PNHSS
Computer Science: Project Work
```

# Introduction:
<hr>
Welcome to the world of C programming, where endless possibilities await you! Throughout this project, we’ll explore 50 fundamental programs that will help you become more skilled and knowledgeable in the C programming language.

So, let’s dive in and start exploring the world of C programming together!
<hr>

# Materials & Methods:

To execute the programs outlined in this guide, the following materials and methods are recommended:

Materials:

1. Computer with a C compiler installed (e.g., GCC, Clang)

2. Text editor or integrated development environment (IDE) for writing and editing C code

Methods:

1. Write each program in a text editor or IDE.

2. Save the program with a .c extension (e.g., program1.c).

3. Compile each program using the C compiler installed on your computer.

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

**14. Program to check whether a year is a leap year or not using conditional operator:**

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

**15. Program to find the maximum of two numbers using conditional operator:**
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




# Chapter 5: Topics including functions and recursion:

**21. Program to find the factorial of a number using a function:**

```
#include <stdio.h>
int factorial(int n) {
    if (n == 0 || n == 1) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}
int main() {
    int num;
    printf("Enter a non-negative integer: ");
    scanf("%d", &num);
    printf("Factorial of %d: %d\n", num, factorial(num));
    return 0;
}
```

**22. Program to check whether a number is even or odd using a function:**

```
#include <stdio.h>
void checkEvenOdd(int n) {
    if (n % 2 == 0) {
        printf("%d is even.\n", n);
    } else {
        printf("%d is odd.\n", n);
    }
}
int main() {
    int num;
    printf("Enter an integer: ");
    scanf("%d", &num);
    checkEvenOdd(num);
    return 0;
}
```


**23. Program to calculate the sum of natural numbers up to a given number using recursion:**

```
#include <stdio.h>
int sumOfNaturalNumbers(int n) {
    if (n == 0) {
        return 0;
    } else {
        return n + sumOfNaturalNumbers(n - 1);
    }
}
int main() {
    int num;
    printf("Enter a positive integer: ");
    scanf("%d", &num);
    printf("Sum of natural numbers up to %d: %d\n", num, sumOfNaturalNumbers(num));
    return 0;
}
```

**24. Program to swap two numbers using functions:**

```
#include <stdio.h>
void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
int main() {
    int num1, num2;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    swap(&num1, &num2);
    printf("After swapping: \nFirst number: %d\nSecond number: %d\n", num1, num2);
    return 0;
}
```
**25. Program to find the maximum of three numbers using functions:**

```
#include <stdio.h>
int maximum(int a, int b, int c) {
    if (a >= b && a >= c) {
        return a;
    } else if (b >= a && b >= c) {
        return b;
    } else {
        return c;
    }
}
int main() {
    int num1, num2, num3;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &num1, &num2, &num3);
    printf("Maximum number: %d\n", maximum(num1, num2, num3));
    return 0;
}
```

**These programs showcase the usage of functions, including recursive functions, for performing specific tasks and modularizing the code.**


# Chapter 6: Topics including pointers:

**26. Program to demonstrate basic pointer declaration and dereferencing:**

```
#include <stdio.h>
int main() {
    int num = 10;
    int *ptr;
    ptr = &num;
    printf("Value of num: %d\n", *ptr);
    return 0;
}
```

**27. Program to swap two numbers using pointers:**

```
#include <stdio.h>
void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
int main() {
    int num1 = 5, num2 = 10;
    printf("Before swapping: num1 = %d, num2 = %d\n", num1, num2);
    swap(&num1, &num2);
    printf("After swapping: num1 = %d, num2 = %d\n", num1, num2);
    return 0;
}
```

**28. Program to find the maximum element in an array using pointers:**

```
#include <stdio.h>
int findMax(int arr[], int size) {
    int max = *arr;
    for (int i = 1; i < size; i++) {
        if (*(arr + i) > max) {
            max = *(arr + i);
        }
    }
    return max;
}
int main() {
    int arr[] = {5, 10, 3, 8, 15};
    int size = sizeof(arr) / sizeof(arr[0]);
    printf("Maximum element in the array: %d\n", findMax(arr, size));
    return 0;
}
```

**29. Program to demonstrate pointer arithmetic:**

```
#include <stdio.h>
int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int *ptr = arr;
    for (int i = 0; i < 5; i++) {
        printf("Value at address %p: %d\n", ptr, *ptr);
        ptr++;
    }
    return 0;
}
```

**30. Program to swap two strings using pointers:**

```
#include <stdio.h>
void swapStrings(char **ptr1, char **ptr2) {
    char *temp = *ptr1;
    *ptr1 = *ptr2;
    *ptr2 = temp;
}
int main() {
    char *str1 = "Hello";
    char *str2 = "World";
    printf("Before swapping: str1 = %s, str2 = %s\n", str1, str2);
    swapStrings(&str1, &str2);
    printf("After swapping: str1 = %s, str2 = %s\n", str1, str2);
    return 0;
}
```

**These programs illustrate the usage of pointers for various tasks such as accessing memory addresses, modifying values indirectly, and performing pointer arithmetic.**

# Chapter 7: Topics including arrays:

**31. Program to find the sum of elements in an array:**

```
#include <stdio.h>
int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int size = sizeof(arr) / sizeof(arr[0]);
    int sum = 0;
    for (int i = 0; i < size; i++) {
        sum += arr[i];
    }
    printf("Sum of elements in the array: %d\n", sum);
    return 0;
}
```

**32. Program to find the largest element in an array:**

```
#include <stdio.h>
int main() {
    int arr[] = {10, 25, 8, 14, 30};
    int size = sizeof(arr) / sizeof(arr[0]);
    int max = arr[0];
    for (int i = 1; i < size; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
    }
    printf("Largest element in the array: %d\n", max);
    return 0;
}
```

**33. Program to search for an element in an array:**

```
#include <stdio.h>
int main() {
    int arr[] = {3, 6, 9, 12, 15};
    int size = sizeof(arr) / sizeof(arr[0]);
    int target = 12;
    int found = 0;
    for (int i = 0; i < size; i++) {
        if (arr[i] == target) {
            found = 1;
            break;
        }
    }
    if (found) {
        printf("%d found in the array.\n", target);
    } else {
        printf("%d not found in the array.\n", target);
    }
    return 0;
}
```

**34. Program to find the reverse of an array:**

```
#include <stdio.h>
int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int size = sizeof(arr) / sizeof(arr[0]);
    printf("Original array: ");
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    printf("\nReverse array: ");
    for (int i = size - 1; i >= 0; i--) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
```

**35. Program to sort an array in ascending order:****

```
#include <stdio.h>
int main() {
    int arr[] = {25, 10, 8, 30, 14};
    int size = sizeof(arr) / sizeof(arr[0]);
    for (int i = 0; i < size - 1; i++) {
        for (int j = 0; j < size - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    printf("Sorted array in ascending order: ");
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
```

**These programs demonstrate various operations on arrays, such as finding the sum, searching for an element, reversing the array, and sorting it in ascending order.**


# Chapter 8: Topics including strings:

**36. Program to find the length of a string:**

```
#include <stdio.h>
#include <string.h>
int main() {
    char str[] = "Hello, World!";
    int length = strlen(str);
    printf("Length of the string: %d\n", length);
    return 0;
}
```

**37. Program to concatenate two strings:**

```
#include <stdio.h>
#include <string.h>
int main() {
    char str1[50] = "Hello";
    char str2[] = "World!";
    strcat(str1, str2);
    printf("Concatenated string: %s\n", str1);
    return 0;
}
```

**38. Program to compare two strings:**

```
#include <stdio.h>
#include <string.h>
int main() {
    char str1[] = "hello";
    char str2[] = "world";
    int result = strcmp(str1, str2);
    if (result == 0) {
        printf("Strings are equal.\n");
    } else if (result < 0) {
        printf("%s comes before %s in dictionary order.\n", str1, str2);
    } else {
        printf("%s comes after %s in dictionary order.\n", str1, str2);
    }
    return 0;
}
```

**39. Program to copy one string to another:**

```
#include <stdio.h>
#include <string.h>

int main() {
    char source[] = "Hello, World!";
    char destination[50];
    strcpy(destination, source);
    printf("Copied string: %s\n", destination);
    return 0;
}
```

**40. Program to reverse a string:**

```
#include <stdio.h>
#include <string.h>
int main() {
    char str[] = "Hello, World!";
    int length = strlen(str);
    for (int i = length - 1; i >= 0; i--) {
        printf("%c", str[i]);
    }
    printf("\n");
    return 0;
}
```

**These programs illustrate various string operations such as finding the length, concatenating, comparing, copying, and reversing strings.**


# Chapter 9: Topics including structures:

**41. Program to define and access structure members:**

```
#include <stdio.h>
struct student {
    int roll_no;
    char name[50];
    float marks;
};
int main() {
    struct student s1;
    s1.roll_no = 1;
    strcpy(s1.name, "John");
    s1.marks = 95.5;
    printf("Student Details:\n");
    printf("Roll Number: %d\n", s1.roll_no);
    printf("Name: %s\n", s1.name);
    printf("Marks: %.2f\n", s1.marks);
    return 0;
}
```

**42. Program to define a structure within another structure:**

```
#include <stdio.h>
struct date {
    int day;
    int month;
    int year;
};
struct employee {
    int emp_id;
    char name[50];
    struct date dob;
};
int main() {
    struct employee emp1 = {101, "Alice", {10, 4, 1990}};
    printf("Employee Details:\n");
    printf("Employee ID: %d\n", emp1.emp_id);
    printf("Name: %s\n", emp1.name);
    printf("Date of Birth: %d/%d/%d\n", emp1.dob.day, emp1.dob.month, emp1.dob.year);
    return 0;
}
```

**43. Program to pass structure to a function:**

```
#include <stdio.h>
struct point {
    int x;
    int y;
};
void display(struct point p) {
    printf("Coordinates: (%d, %d)\n", p.x, p.y);
}
int main() {
    struct point p1 = {3, 5};
    display(p1);
    return 0;
}
```

**44. Program to return a structure from a function:**

```
#include <stdio.h>
struct point {
    int x;
    int y;
};
struct point createPoint(int x, int y) {
    struct point p;
    p.x = x;
    p.y = y;
    return p;
}
int main() {
    struct point p1 = createPoint(3, 5);
    printf("Coordinates: (%d, %d)\n", p1.x, p1.y);
    return 0;
}
```

**45. Program to define an array of structures:**

```
#include <stdio.h>
struct employee {
    int emp_id;
    char name[50];
};
int main() {
    struct employee emp_array[3];
    emp_array[0].emp_id = 101;
    strcpy(emp_array[0].name, "Alice");
    emp_array[1].emp_id = 102;
    strcpy(emp_array[1].name, "Bob");
    emp_array[2].emp_id = 103;
    strcpy(emp_array[2].name, "Charlie");
    printf("Employee Details:\n");
    for (int i = 0; i < 3; i++) {
        printf("Employee ID: %d\n", emp_array[i].emp_id);
        printf("Name: %s\n", emp_array[i].name);
    }
    return 0;
}
```

**These programs demonstrate various concepts related to structures such as defining structures, accessing structure members, nesting structures, passing structures to functions, returning structures from functions, and defining arrays of structures.**




# Chapter 10: Topics including file I/O:

**46. Program to write data to a file:**

```
#include <stdio.h>
int main() {
    FILE *file_pointer;
    file_pointer = fopen("data.txt", "w");
    if (file_pointer == NULL) {
        printf("Error opening file!\n");
        return 1;
    }
    fprintf(file_pointer, "Hello, World!\n");
    fprintf(file_pointer, "This is a file.\n");
    fclose(file_pointer);
    printf("Data written to file successfully!\n");
    return 0;
}
```

**47. Program to read data from a file:**

```
#include <stdio.h>
int main() {
    FILE *file_pointer;
    char line[100];
    file_pointer = fopen("data.txt", "r");
    if (file_pointer == NULL) {
        printf("Error opening file!\n");
        return 1;
    }
    while (fgets(line, sizeof(line), file_pointer)) {
        printf("%s", line);
    }
    fclose(file_pointer);
    return 0;
}
```

**48. Program to append data to a file:**

```
#include <stdio.h>
int main() {
    FILE *file_pointer;
    file_pointer = fopen("data.txt", "a");
    if (file_pointer == NULL) {
        printf("Error opening file!\n");
        return 1;
    }
    fprintf(file_pointer, "This data is appended.\n");
    fclose(file_pointer);
    printf("Data appended to file successfully!\n");
    return 0;
}
```

**49. Program to copy contents of one file to another:**

```
#include <stdio.h>
int main() {
    FILE *source_file, *target_file;
    char ch;
    source_file = fopen("source.txt", "r");
    target_file = fopen("target.txt", "w");
    if (source_file == NULL || target_file == NULL) {
        printf("Error opening files!\n");
        return 1;
    }
    while ((ch = fgetc(source_file)) != EOF) {
        fputc(ch, target_file);
    }
    printf("File copied successfully!\n");
    fclose(source_file);
    fclose(target_file);
    return 0;
}
```

**50. Program to count number of lines in a file:**

```
#include <stdio.h>
int main() {
    FILE *file_pointer;
    char ch;
    int lines = 0;
    file_pointer = fopen("data.txt", "r");
    if (file_pointer == NULL) {
        printf("Error opening file!\n");
        return 1;
    }
    while ((ch = fgetc(file_pointer)) != EOF) {
        if (ch == '\n') {
            lines++;
        }
    }
    fclose(file_pointer);
    printf("Number of lines in the file: %d\n", lines);
    return 0;
}
```

**These programs demonstrate basic file I/O operations such as opening, reading, writing, appending, and closing files, as well as performing operations like counting lines and copying contents between files.**


# In conclusion

**This project has covered 50 essential C programming exercises, starting from basic concepts and progressing to more advanced topics. Keep coding and exploring!!**
