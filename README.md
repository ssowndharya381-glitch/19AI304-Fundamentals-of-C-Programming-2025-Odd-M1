# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>

int main() {

    int num = 10;          
    float pi = 3.14f;      
    char grade = 'A';      
    char name[] = "Hello";  
    printf("Integer literal: %d\n", num);
    printf("Float literal: %.2f\n", pi);
    printf("Character literal: %c\n", grade);
    printf("String literal: %s\n", name);

    return 0;
}
```
# Output:
<img width="922" height="347" alt="image" src="https://github.com/user-attachments/assets/ae2f3d9c-ccba-49dc-9432-573a07158807" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>
#define VALUE1 10  
int main() {
    const int VALUE2 = 20;   
    printf("Macro Constant = %d\n", VALUE1);
    printf("Constant Variable = %d\n", VALUE2);
    return 0;
}
```
# Output:
<img width="941" height="340" alt="image" src="https://github.com/user-attachments/assets/193277e1-3df1-4be7-bcdf-ba9d56a6b8ff" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int age = 18;          
    float height = 5.6f;   
    double weight = 55.75; 
    char grade = 'A';      
    printf("Integer value (age): %d\n", age);
    printf("Float value (height): %.2f\n", height);
    printf("Double value (weight): %.2lf\n", weight);
    printf("Character value (grade): %c\n", grade);

    return 0;
}
```
# Output:
<img width="931" height="314" alt="image" src="https://github.com/user-attachments/assets/9045bcb2-e47c-4665-b6e4-c06644a3be6d" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    printf("\n   Arithmetic Operations \n");
    printf("Addition = %d\n", a + b);
    printf("Subtraction = %d\n", a - b);
    printf("Multiplication = %d\n", a * b);

    if (b != 0) {
        printf("Division = %d\n", a / b);
        printf("Remainder = %d\n", a % b);
    } else {
        printf("Division = Not possible (division by zero)\n");
        printf("Remainder = Not possible (division by zero)\n");
    }

    printf("\n   Bitwise Operations  \n");
    printf("a & b (AND)= %d\n", a & b);
    printf("a | b (OR) = %d\n", a | b);
    printf("a ^ b (XOR)= %d\n", a ^ b);
    printf("a << 1 (Left Shift) = %d\n", a << 1);
    printf("b << 1 (Left Shift) = %d\n", b << 1);
    printf("a >> 1 (Right Shift)= %d\n", a >> 1);
    printf("b >> 1 (Right Shift)= %d\n", b >> 1);
    printf("~a (NOT) = %d\n", ~a);
    printf("~b (NOT) = %d\n", ~b);
    return 0;
}
```
# Output:
<img width="940" height="396" alt="image" src="https://github.com/user-attachments/assets/00a0cbfc-98a5-4d5c-8610-9b4f9c8bc3a5" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    char ch;
    printf("Enter a character: ");
    scanf(" %c", &ch);
    (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||
     ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U') ?
        printf("%c is a Vowel\n", ch) :
    ((ch>='a'&&ch<='z') || (ch>='A'&&ch<='Z')) ?
        printf("%c is a Consonant\n", ch) :
    (ch>='0' && ch<='9') ?
        printf("%c is a Digit\n", ch) :
        printf("%c is a Special Symbol\n", ch);
    return 0;
}
```

# Output:
<img width="890" height="362" alt="image" src="https://github.com/user-attachments/assets/36ee277d-46db-44c3-a682-24178799fcbd" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


