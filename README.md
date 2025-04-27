# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int m, n;
    scanf("%d %d", &m, &n);
    for (int i = m; i <= n; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }
    printf("\n");
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/8249de47-15e3-490f-88ad-ae7520e96f93)











## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int i,j,s,n;
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        for(s=0;s<n-i-1;s++)
        printf(" ");
        for(j=0;j<i*2+1;j++)
        printf("*");
        printf("\n");
    }
}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/311810cd-23e8-4a1d-8647-7f6fdacdf50f)






## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
include<stdio.h>

void add(int a, int b);
void subtract(int a, int b);
int main(){
int num1, num2;
printf("Enter two numbers: “);
scanf("%d %d”, &num1, &num2);
printf("\nAddition result:\n")；
add(num1, num2);
printf("\nSubtraction result\n");
subtract(num1, num2);
return 0;
}
void add(int a, int b){
int result =a +b;
printf("%d + %d = %d\n", a, b, result);
}
void subtract(int a, int b){
int result = a - b;
printf("%d - %d = %d\n", a, b, result);

}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/1159e898-8069-494a-9ca6-16e4bb70a694)







## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int number, temp, digit, sum = 0;
    printf("Enter an integer: ");
    scanf("%d", &number);
    if (number < 0) {
        number = -number;
    }
    temp = number;
    for (int i = temp; i > 0; i /= 10) {
        digit = i % 10;
        if (digit % 2 != 0) {
            sum += digit;
        }
    }
    printf("Sum of odd digits: %d\n", sum);
    return 0;
}
```


## OUTPUT:

![image](https://github.com/user-attachments/assets/6a1c0dd2-66b7-4caa-b2ff-545c69e407e5)





## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
int factorial(int n) {
    int fact = 1;
    for (int i = 1; i <= n; i++) {
        fact *= i;
    }
    return fact;
}
int main() {
    int num;
    printf("Enter a positive integer: ");
    scanf("%d", &num);
    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        int result = factorial(num);
        printf("Factorial of %d is %d\n", num, result);
    }
    return 0;
}
```


## OUTPUT:

![image](https://github.com/user-attachments/assets/ceebd25d-6a85-4b6a-841d-6ba6b9afdc64)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
