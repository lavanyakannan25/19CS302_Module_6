# EX 28 C program to add two distances in feet and inches using structure
## DATE:
## AIM:
To write a C program to add two distances in feet and inches using structure
## Algorithm
1. Start.
2. Define a structure Distance with members feet and inches.
3. Declare three structure variables: d1, d2, and sum.
  Read the first distance (d1).
  Read the second distance (d2).
4. Add feet and inches separately:
  sum.feet = d1.feet + d2.feet
  sum.inches = d1.inches + d2.inches
5. If sum.inches >= 12:
  Add sum.inches / 12 to sum.feet
  Set sum.inches = sum.inches % 12
6. Display the total distance.
7. Stop.

## Program:
```
#include <stdio.h>
struct Distance {
    int feet;
    int inches;
};
int main() {
    struct Distance d1, d2, total;
    scanf("%d %d", &d1.feet, &d1.inches);
    scanf("%d %d", &d2.feet, &d2.inches);
    total.feet = d1.feet + d2.feet;
    total.inches = d1.inches + d2.inches;
    if (total.inches >= 12) {
        total.feet += total.inches / 12;
        total.inches = total.inches % 12;
    }
    printf("Total distance- Feet: %d, Inches: %d\n", total.feet, total.inches);
    return 0;
}
```

## Output:
<img width="1225" height="376" alt="Screenshot (59)_25808" src="https://github.com/user-attachments/assets/ef765c2d-4eb5-4a7c-a8d2-434b2e93b6a0" />



## Result:
Thus the program was executed and the output was verified successfully.
