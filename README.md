# Area-of-circle
This is a program for calculating area of circle using library of math.h and functions in C programming.


#include <stdio.h>
#include <math.h>
#define PI 3.14

double findsqrt(double n)
{
    return sqrt(n);
}

int main()
{
    int x1, y1, x2, y2;
    printf("Enter absicca of first coordinate:\n");
    scanf("%d", &x1);
    printf("Enter ordinate of first coordinate:\n");
    scanf("%d", &y1);
    printf("Enter absicca of second coordinate:\n");
    scanf("%d", &x2);
    printf("Enter ordinate of second coordinate:\n");
    scanf("%d", &y2);
    int s;
    float r;
    s = (x2 - x1) * (x2 - x1) + (y2 - y1) * (y2 - y1);
    r = findsqrt(s);
    printf("Radius of circle is %f\n", r);
    float Area;
    Area = PI * r * r;
    printf("Area of circle is %f", Area);
    return 0;
}
