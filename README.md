# EX-11-EMI-CALCULATOR

NAME- AANANDHA KANNAN.S

REG NO : 212224040003

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>

void calculateEMI(float principal, float rate, int time) {
    float r = rate / (12 * 100);
    float emi;
    emi = (principal * r * pow(1 + r, time)) / (pow(1 + r, time) - 1);
    printf("Calculated EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;

    printf("Enter Principal Amount: ");
    scanf("%f", &principal);

    printf("Enter Annual Rate of Interest (in %%): ");
    scanf("%f", &rate);

    printf("Enter Time (in months): ");
    scanf("%d", &months);

    calculateEMI(principal, rate, months);

    return 0;
}

```


## OUTPUT

![image](https://github.com/user-attachments/assets/4312deab-2624-4d6e-a752-c2a907f3cdcc)






## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, first = 0, second = 1, next, i;

    printf("Enter the number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci Series: ");
    for(i = 0; i < n; i++) {
        if(i <= 1)
            next = i;
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/779065ab-b7c2-41c8-9742-b294e85a1b3b)



## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int arr[n];
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("%d\n", arr[n-1]);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/daa57fb4-ff23-4f94-8694-cde30d91043c)




## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, count = 0;
    scanf("%d", &n);

    int arr[n];
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if(arr[i] > 0) {
            count++;
        }
    }

    printf("%d\n", count);
    return 0;
}

```



## OUTPUT

![image](https://github.com/user-attachments/assets/db295d0b-68fc-4f72-82b0-59ee8393e5dc)






## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the arr#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int arr[n];
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for(int i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            // Replace even element with ASCII code of 'E'
            arr[i] = 'E';
        }
    }

    for(int i = 0; i < n; i++) {
        if(arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    printf("\n");

    return 0;
}
ay.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:


## Output:
 ![image](https://github.com/user-attachments/assets/03843471-a819-45bd-afdc-9d0cdf9c553c)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



