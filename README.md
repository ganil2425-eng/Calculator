# Calculator
This project made in C programing language

#include <stdio.h>

int main() 
{
    int choice;
    int a, b;
    float x, y;

    printf("===========MENU===========\n");
    printf("1.Addition\n");
    printf("2.Subtraction\n");
    printf("3.Multiplication\n");
    printf("4.Division\n");
    printf("5.Remainder\n");
    printf("_____________________\n");

    printf("Enter your choice: ");
    scanf("%d", &choice);

    switch(choice)
    {
        case 1:
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Answer: %d", a + b);
            break;

        case 2:
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Answer: %d", a - b);
            break;

        case 3:
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Answer: %d", a * b);
            break;

        case 4:
            printf("Enter two numbers: ");
            scanf("%f %f", &x, &y);
            if(y != 0)
                printf("Answer: %.2f", x / y);
            else
                printf("Division by zero not allowed");
            break;

        case 5:
            printf("Enter two numbers: ");
            scanf("%d %d", &a, &b);
            printf("Answer: %d", a % b);
            break;

        default:
            printf("Invalid choice");
    }

    return 0;
}
