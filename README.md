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
    int M, N;
    printf("Enter the value of M: ");
    scanf("%d", &M);

    printf("Enter the value of N: ");
    scanf("%d", &N);
    printf("Even numbers from %d to %d are:\n", M, N);
    for (int i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }

    return 0;
}


```
## OUTPUT:



![446450589-02a5e5a5-5795-4153-b233-ef449c82ecb0](https://github.com/user-attachments/assets/c0651839-8ee7-4d00-a477-2f47201312f3)







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

#include <stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    for(int i=n;i>=1;i--)
    {
        for(int j=0;j<i;j++)
        printf("*");
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:



![438805595-e44ea667-1394-406e-99ed-b45453966187](https://github.com/user-attachments/assets/81e336bb-fc89-479c-81bc-7aca11f56cad)


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
#include <stdio.h>

void add(int a, int b) {
    int result = a + b;
    printf("Addition of %d and %d is: %d\n", a, b, result);
}

void subtract(int a, int b) {
    int result = a - b;
    printf("Subtraction of %d and %d is: %d\n", a, b, result);
}

int main() {
    int num1, num2;
    printf("Enter two numbers:\n");
    scanf("%d %d", &num1, &num2);
    add(num1, num2);
    subtract(num1, num2);

    return 0;
}

```

## OUTPUT:


![446452190-d0770a31-8a81-4a2c-81b1-8f6996742438](https://github.com/user-attachments/assets/6aa9d954-9bb4-4703-9edb-34f37b89feaa)




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
    int M, N, sum = 0;

    scanf("%d %d", &M, &N);

    if (M >= 1 && N <= 100 && N > M) {
        for (int i = M; i <= N; i++) {
            if (i % 2 != 0) {
                sum += i;
            }
        }
        printf("Sum = %d\n", sum);
    } else {
        printf("Invalid Range\n");
    }

    return 0;
}
```

## OUTPUT:

![438807823-1636546f-b433-4322-8386-116daff8916e](https://github.com/user-attachments/assets/4f48d99a-1369-45ae-84ad-b1e8b990199f)



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
#include<stdio.h>
#include<math.h>
int fact(int n);
int main()
{    
    int n;
    scanf("%d",&n);
    printf("Factorial value is: %d ",fact(n));
    return 0;
}
int fact(int n)
{
    int i,fact=1;
    
    for(i=1; i<=n; i++)
    {
        fact=fact*i;
The program correctly computes the factorial of a given number using a separate function and displays the result.

## OUTPUT:




![438809777-ae346899-8587-483c-b583-a5cc932ee38b](https://github.com/user-attachments/assets/a40e797c-702c-4daa-8776-540c6006e003)






## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 




