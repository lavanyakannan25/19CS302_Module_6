# EX 30 write a program to display the class timings using enumeration
## DATE:
## AIM:
write a program to display the class timings using enumeration?

## Algorithm
1. Start.
2. Define an enumeration for class timings (FIRST, SECOND, THIRD, FOURTH).
3. Assign the class timings to enumeration constants.
4. Display each class timing using its enumeration name.
5. Stop.

## Program:
```
#include <stdio.h>
enum ClassHours {
    First = 8,
    Second,
    Third,
    Fourth,
    Fifth
};
int main() {
    printf("Class Timings\n");
    printf("First Hour = %d am\n", First);
    printf("second Hour = %d am\n", Second);
    printf("Third Hour = %d am\n", Third);
    printf("Fourth Hour = %d am\n", Fourth);
    printf("Fifth Hour = %d pm\n", Fifth);  
    return 0;
}
```

## Output:
<img width="952" height="372" alt="Screenshot (60)_18375_1935" src="https://github.com/user-attachments/assets/e45ff4bf-60ca-4d47-9c5d-f5c555bd1846" />


## Result:
Thus the program was executed and the output was verified successfully.
