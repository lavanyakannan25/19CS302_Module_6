# EX 27 Write a C program to check given input is even or odd using calloc().
## DATE:
## AIM:
To Write a C program to check given input is even or odd using calloc().
## Algorithm
1. Start.
2. Declare an integer pointer ptr.
3. Allocate memory for one integer using calloc().
4. Check if memory allocation is successful.
 If ptr == NULL, display "Memory allocation failed" and stop.
6. Read a number and store it in the allocated memory location (*ptr).
7. Check whether the number is divisible by 2.
  If *ptr % 2 == 0, display "The number is Even".
8. Otherwise, display "The number is Odd".
9. Free the allocated memory using free(ptr).  

## Program:
```
#include <stdio.h>
#include <stdlib.h>
int main() {
    int *num;
    num = (int *)calloc(1, sizeof(int));
    if (num == NULL) {
        printf("Memory allocation failed.\n");
        return 1;
    }
    scanf("%d", num);
    if (*num % 2 == 0) {
        printf("%d is Even Number\n", *num);
    } else {
        printf("%d is Odd Number\n", *num);
    }
    free(num);
    return 0;
}
```

## Output:
<img width="1145" height="550" alt="Screenshot (58)_12660" src="https://github.com/user-attachments/assets/f960e05c-de43-4b73-aeb4-6431d9dce3fc" />




## Result:
Thus the program was executed and the output was verified successfully.
