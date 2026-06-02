# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M3
# IAPR-3- Module 3 - FoC
## 5. Implementation of one-dimensional array and multidimensional array.
## 6. Implementation of string manipulation.

# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1. Start the program.
2. Read principal amount, rate of interest and months.
3. Pass these values as arguments to function.
4. Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5. Display the result.
6. Stop the program.

## PROGRAM

```
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float rate, int time) {
    float monthlyRate = rate / (12 * 100);
    int months = time * 12;
    float emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);
    printf("EMI = %.2f\n", emi);
}
int main() {
    float principal, rate;
    int time;
    scanf("%f", &principal);
    scanf("%f", &rate);
    scanf("%d", &time);
    calculateEMI(principal, rate, time);
    return 0;
}

```

## OUTPUT
<img width="1039" height="624" alt="Screenshot 2026-06-02 144308" src="https://github.com/user-attachments/assets/6f6d61e2-cdda-48ea-9368-96b20abde78b" />


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully

# EX-12-FIBONACCI-SERIES

## AIM

To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM

1. Start the program.
2. Read number of terms to display.
3. Add the previous two terms and store it in new term.
4. Assign 2nd term to 1st term and 3rd term to 2nd term.
5. Repeat steps 3 and 4 n number of times.
6. Display the result.
7. Stop the program.

## PROGRAM

```
#include <stdio.h>
int main() {
    int n = 6;
    int a = 0, b = 1, c, i;
    printf("Fibonacci series for %d terms:\n", n);
    printf("%d %d ", a, b);
    for(i = 3; i <= n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }
    return 0;
}

```

## OUTPUT
<img width="1036" height="617" alt="Screenshot 2026-06-02 144323" src="https://github.com/user-attachments/assets/c0fded5f-4bca-407b-90be-5bfe5542bccd" />


## RESULT

Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.

# EX-13-ONE-DIMENSIONAL-ARRAY

## AIM

To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM

1. Start the program.
2. Read a variable.
3. Read the array values n number of times.
4. Print the last element.
5. Stop the program.

## PROGRAM

```
#include <stdio.h>
int main() {
    int n, i;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n - 1]);
    return 0;
}

```

## OUTPUT

<img width="1048" height="619" alt="Screenshot 2026-06-02 144337" src="https://github.com/user-attachments/assets/4ebc7195-7419-49a9-bb25-c424e1effde5" />


## RESULT

Thus the program to read n elements as input and print the last element of the array has been executed successfully.

# EX-14-POSITIVE-ARRAY-ELEMENTS

## AIM

To write a C Program to count total number of positive elements in an array.

## ALGORITHM

1. Start the program.
2. Read a variable.
3. Read the array values n number of times.
4. If the array value can be divided by 2 then increment count by 1.
5. Display result.
6. Stop the program.

## PROGRAM

```
#include <stdio.h>
int main() {
    int n, i, count = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(i = 0; i < n; i++) {
        if(arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);
    return 0;
}

```

## OUTPUT

<img width="1035" height="617" alt="Screenshot 2026-06-02 144408" src="https://github.com/user-attachments/assets/7d69ab96-fc8f-4552-ae44-1cae14582192" />


## RESULT

Thus the program to count total number of positive elements in an array has been executed successfully.

# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:

To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:

1. Input the array:
   Read the size of the array.
   Input the elements of the array.
2. Iterate through the array:
   For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3. Replace even elements with 'E':
   If an element is even, replace that element with the character 'E'.
4. Output the updated array:
   Print the updated array after replacements.

## Program:

```
#include <stdio.h>
int main() {
    int n, i;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Array after replacing even elements with 'E':\n");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}

```

## Output:

<img width="1038" height="614" alt="Screenshot 2026-06-02 144429" src="https://github.com/user-attachments/assets/e97190bd-f8b4-4df7-b342-d43d4f7aadcf" />


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.
