# EX 26 write a C program to find area of a circle and perimeter of a circle using pointer 
## DATE:
## AIM:
write a C program to find area of a circle and perimeter of a circle using pointer 
## Algorithm
1. Start.
2. Declare float variables radius, area, perimeter.
3. Declare pointer variables *r, *a, *p.
4. Assign addresses:
 r = &radius
 a = &area
 p = &perimeter
5. Read the radius of the circle.
6. Calculate area using the pointer:
 *a = 3.14 * (*r) * (*r)
7. Calculate perimeter (circumference) using the pointer:
 *p = 2 * 3.14 * (*r)
8. Display the area and perimeter.
9. Stop. 

## Program:
```
#include <stdio.h>
#define PI 3.14
void calculate(float *radius, float *area, float *perimeter) {
    *area = PI * (*radius) * (*radius);
    *perimeter = 2 * PI * (*radius);
}
int main() {
    float radius, area, perimeter;
    scanf("%f", &radius);
    calculate(&radius, &area, &perimeter);
    printf("Area of Circle = %.2f\n", area);
    printf("Perimeter of Circle = %.2f\n", perimeter);

    return 0;
}
```

## Output:

<img width="1439" height="400" alt="Screenshot (57)_13059" src="https://github.com/user-attachments/assets/f3d0ede1-6205-48d4-89ef-3766a25539c4" />



## Result:
Thus the program was executed and the output was verified successfully.
