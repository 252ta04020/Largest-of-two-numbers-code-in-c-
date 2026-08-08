#include <stdio.h>

int main() {
    double num1, num2;

    // Prompt user for input
    printf("Enter two numbers: ");
    
    // Read the inputs and verify successful parsing
    if (scanf("%lf %lf", &num1, &num2) != 2) {
        printf("Error: Invalid input. Please enter numeric values.\n");
        return 1; 
    }

    // Compare and display the result
    if (num1 > num2) {
        printf("%.2lf is the largest number.\n", num1);
    } else if (num2 > num1) {
        printf("%.2lf is the largest number.\n", num2);
    } else {
        printf("Both numbers are equal (%.2lf).\n", num1);
    }

    return 0;
}
