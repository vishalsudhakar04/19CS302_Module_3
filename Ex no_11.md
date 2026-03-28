EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.

DATE: 28-03-2026

AIM:

To write a C Program to convert a given decimal value to binary using function without arguments with return type.

Algorithm

Start the program.

Define a function decimalToBinary() that returns a long integer.

Inside the function, declare variables for the decimal number, remainder, binary result, and place value.

Prompt the user to enter a decimal number within the function.

Use a loop to divide the number by 2, storing the remainders to construct the binary equivalent.

Return the calculated binary value to the main function.

Display the returned binary value in the main function.

Stop the program.

Program:

#include <stdio.h>

long decimalToBinary() {
    int n, remainder;
    long binary = 0, i = 1;
    printf("Enter a decimal number: ");
    scanf("%d", &n);
    while (n != 0) {
        remainder = n % 2;
        n /= 2;
        binary += remainder * i;
        i *= 10;
    }
    return binary;
}

int main() {
    long bin;
    bin = decimalToBinary();
    printf("Binary value: %ld\n", bin);
    return 0;
}


Output:

Enter a decimal number: 10
Binary value: 1010


Result:

Thus the program was executed and the output was verified successfully.
