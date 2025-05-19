EX-21-POINTERS
## Name: Renick Fabian Rajesh
## Reg no: 212224230227
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
```
#include <stdio.h>
int main() 
{
    float num = 23.65;   
    float *ptr = &num;   
    printf("Before: %.2f\n", *ptr);

    *ptr = 25.0;         
    printf("After: %.2f\n", *ptr);
    return 0;
}
```
## OUTPUT:
 	
![image](https://github.com/user-attachments/assets/6629efb4-71a6-4fa7-8958-8b934b0fb721)

## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
```
#include <stdio.h>
int product(int n) 
{
    if (n == 1)
        return 1;
    return n * product(n - 1);
}
int main() {
    printf("%d", product(12));
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/e1d93814-b7e8-442b-8006-c84576a6fe29)

           
## RESULT:

Thus the program has been executed successfully.
 
 


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int rows, cols;
    printf("Enter number of rows and columns: ");
    scanf("%d %d", &rows, &cols);
    int matrix[10][10]; 
    printf("Enter elements of the matrix:\n");
    for(int i = 0; i < rows; i++) {
        for(int j = 0; j < cols; j++) {
            scanf("%d", &matrix[i][j]);
        }
    }
    for(int i = 0; i < rows; i++) {
        int sum = 0;
        for(int j = 0; j < cols; j++) {
            sum += matrix[i][j];
        }
        printf("Sum of row %d = %d\n", i + 1, sum);
    }
    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/00f02d38-31da-4c76-9d39-595fafee5954)

 ## RESULT

 Thus the program has been executed successfully.


# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:
```
#include <stdio.h>
#include <string.h>
int main() {
    char str[100];
    int rows;
    printf("Enter a string: ");
    scanf("%s", str);
    printf("Enter number of rows: ");
    scanf("%d", &rows);
    int len = strlen(str);
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < len; j++) {
            printf("%c ", str[j]);
        }
        printf("\n");
    }
    return 0;
}
```
 ## OUTPUT

![image](https://github.com/user-attachments/assets/1b07c739-0bcf-4eab-b6a6-6275b5255765)
 

## RESULT

Thus the C program to String process executed successfully
 

 
.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    int arr[6];
    int *ptr = arr;
    printf("Enter 6 integers:\n");
    for(int i = 0; i < 6; i++) {
        scanf("%d", (ptr + i)); 
    }
    printf("The array elements are:\n");
    for(int i = 0; i < 6; i++) {
        printf("%d ", *(ptr + i)); 
    }

    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/19773d74-d723-45f2-802f-da9db61233e5)
 

## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


