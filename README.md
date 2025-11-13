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
      int m,n;
      scanf("%d %d",&m,&n);
      for (int i=m;i<=n;i++)
      {
          if(i%2==0)
          {
              printf("%d ",i);
          }
      }
     

    return 0;
}
```

## OUTPUT:
<img width="1833" height="850" alt="image" src="https://github.com/user-attachments/assets/48ac45c2-3021-41ac-aff5-a6080034a2da" />











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

int main() {
    int i, j, n;

    printf("Enter the number of rows: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        for (j = 1; j <= i; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}
```

## OUTPUT:
<img width="1918" height="903" alt="image" src="https://github.com/user-attachments/assets/29ad02d1-0632-42b6-87ac-2b048eb22851" />






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


void add(int a,int b)
{
    int sum=a+b;
    int diff=a-b;
    printf("The sum of a and b is %d\n",sum);
    printf("The Diffrence of a and b is %d\n",diff);
    
}

int main() {

     int a,b;
     scanf("%d %d",&a,&b);
     add(a,b);

    return 0;
}
```


## OUTPUT:
<img width="1821" height="891" alt="image" src="https://github.com/user-attachments/assets/387196d0-5e4e-4d91-9068-91420354e5b2" />







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
int a,sum=0,rem,count=0,temp;
     scanf("%d",&a);
     temp=a;
     
     while(temp!=0)
     {
         temp=temp/10;
         count++;
     }
         for (int i=0;i<count;i++)
     {
         rem=a%10;
         if(rem%2!=0)
         {
             sum+=rem;
         }
         a=a/10;
     }
     printf("The sum of odd digits in the number is %d",sum);
        return 0;
}
```


## OUTPUT:
<img width="1918" height="900" alt="image" src="https://github.com/user-attachments/assets/94ab4d1f-d5f9-4076-b3fd-c59cfa64b09a" />





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
void fact(int n)
{
    int fac=1,i;
    for(i=1;i<=n;i++)
    {
        fac=fac*i;
    }
    printf("Factorail value of n is %d\n",fac);
}
int main() {

   int a;
   printf("Enter value:");
   scanf("%d",&a);
  fact(a);
        return 0;
}
```


## OUTPUT:
<img width="1913" height="907" alt="image" src="https://github.com/user-attachments/assets/4b73cac9-e184-4305-9585-7d182c3822a2" />


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
