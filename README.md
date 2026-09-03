# Calculator-c
C programming Calculator

#include <stdio.h>
int main()
    {
        float num1, num2, sum;
        char operatorp;

        printf("=====calculator=====\n");
        printf("Enter first number: ");
        scanf("%f", &num1);

        printf("Enter operator (+, -, *, /): ");
        scanf(" %c", &operatorp);

        printf("Enter second number: ");
        scanf("%f", &num2);

        switch (operatorp)
        {
            case '+':
                sum = num1 + num2;
                printf("The sum is: %.2f\n",sum);
                break;

            case '-':
                sum = num1 - num2:
                printf("The difference is: %.2f\n",sum);
                break;
            case '*':
                sum = num1 * num2;
                printf("The product is: %.2f\n",sum);
            break;

            case '/':
                if (num2 !=0)
                {
                    sum = num1 / num2;
                    printf("The quotient is: %.2f\n",sum);
                }
                else
                {
                    printf("Error: Division by zero is not allowed.\n");
                }
                break;
        }
    }
