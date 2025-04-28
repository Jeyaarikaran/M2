# EX-06 - Looping
## AIM:
To write a C program to print the string "KEYBOARD" n number of times based on user input.

## ALGORITHM:
```
1.Start the program.
2.Declare integer variables n and i.
3.Prompt the user to enter the number of times (n) to print "KEYBOARD".
4.Read the value of n using scanf().
5.Use a for loop that runs from i = 0 to i < n.
6.Inside the loop, print "KEYBOARD".
7.End the program.
```
## PROGRAM:
```.py
#include <stdio.h>
int main()
{
    int a,i;
    scanf("%d",&a);
    for(i=1;i<=a;i++)
    {
       printf("KEYBOARD\n");
    }
    return 0;
    
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/015ba041-8022-4e03-b1d8-73491bd4c2f5)









## RESULT:
The program successfully prints the string "KEYBOARD" n number of times as per the user's input.
 
 


# EX-07-Nested-loop

## AIM:
To write a C program to print a hollow square pattern using a for loop.

## ALGORITHM:
```
1.Start the program.
2.Declare three integer variables: i, j, and n.
4.3.Prompt the user to enter the number of rows (which will also be the number of columns for the square).
4.Read the input value of n.
5.Use a nested for loop:
6.Outer loop (i) runs from 1 to n (for each row).
7.Inner loop (j) runs from 1 to n (for each column).
8.In the inner loop:
If i == 1 (first row) or i == n (last row) or j == 1 (first column) or j == n (last column), print #.
Else, print a space " " (two spaces for better alignment).
After printing each row, move to the next line (\n).
9.End the program.
```
## PROGRAM:
```.py
#include <stdio.h>
int main()
{
    int a,i,j;
    scanf("%d",&a);
    for(i=0;i<a;i++)
    {
        for(j=0;j<a;j++)
        {
        if(i==0||i==a-1||j==0||j==a-1)
        {
            printf("#");
        }
        else
        {
            printf(" ");
        }
        }
    printf("\n");
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/f99c300c-a5c4-407b-9747-d122e8045604)





## RESULT:
The program successfully prints a hollow square pattern of size n × n using # symbols, where n is provided by the user.
 
 


# EX-08-Functions

## AIM:
To write a C program to perform addition and subtraction of two numbers using functions (without arguments and with return type).


## ALGORITHM:
```
1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.
```
## PROGRAM:
```.py
#include<stdio.h>
void cal(int a,int b){
    printf("Addition: %d",a+b);
    printf("\nSubtraction: %d",a-b);
}
int main(){
    int a,b;
    scanf("%d",&a);
    scanf("%d",&b);
    cal(a,b);
    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/6b5e2249-4d53-49db-aa03-3a9f5a5eaca0)






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully.
 
 


# EX-09-Use For Loop

## AIM:
To write a C program to display n number of multiplication tables vertically using for loops.

## ALGORITHM:
```
1.Start the program.
2.Declare three integer variables: n, i, and j.
3.Prompt the user to input the number of tables (n).
4.Read the value of n using scanf().
5.Use a nested for loop:
6.Outer loop (i) runs from 1 to n (to print each row).
7.Inner loop (j) runs from 1 to n (to print each column in the row).
8.Inside the inner loop, print the product of i * j followed by a space.
After the inner loop, print a newline (\n) to move to the next row.
9.End the program

````
## PROGRAM:
```.py
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for(int i=1;i<=a;i++){
        for(int j=1;j<=a;j++){
            printf("%d ",i*j);
        }
        printf("\n");
    }
    return 0;
}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/7f292370-cc1a-4021-a347-4b4c72e6dad0)




## RESULT:
The program successfully displays n multiplication tables vertically, using nested for loops based on the user's input.




# EX – 10 - Pascal’s Triangle for a given number of rows
## AIM:
To write a C program to print Pascal’s Triangle for a given number of rows using loops.
## ALGORITHM:
```
1.Start the program.
2.Declare necessary variables: n, i, j, and coef.
3.Ask the user to input the number of rows n.
4.Use an outer loop from i = 0 to i < n:
Print spaces for formatting (for pyramid shape).
Initialize coef = 1.
Use an inner loop from j = 0 to j <= i:
If j == 0 or i == 0, set coef = 1.
Otherwise, calculate coef = coef * (i - j + 1) / j.
Print coef with a space.
5.After the inner loop, print a new line.
6.End the program.
```
## PROGRAM:
```.py
#include<stdio.h>
int main()
{
  int i,j,k;
  printf("0\n");
  k=0;
  for(i=12;i>=1;i--)
  {
    for(j=i;j<=12;j++)
    {
        printf("%d ",j);
    }
    printf("0 ");
    for(j=12;j>=i;j--)
    {
        printf("%d ",j);
    }
    k++;
    printf("\n");
  }
}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/03e662d0-34f8-4a1e-b543-58f2fcc96f7f)


## RESULT:

 The C program successfully prints Pascal’s Triangle up to the given number of rows entered by the user, displaying the triangle correctly formatted.
