## DATE: 28-03-2026

## AIM:
To write a C program to check whether the given number is prime or not using a function with arguments and without a return type.

## Algorithm
1. **Start** the program.
2. **Define** a function `checkPrime(int n)` that accepts an integer as an argument.
3. **In the main function**, read an integer `num` from the user.
4. **Call** the `checkPrime` function by passing `num` as the argument.
5. **Inside the function**:
    * Initialize a flag or counter.
    * Loop from 2 to $n/2$.
    * If `n` is divisible by any number in the loop, it is not prime.
6. **Print** the result (Prime or Not Prime) directly from the function.
7. **Stop** the program.

## Program:
```c
#include <stdio.h>

void checkPrime(int n) {
    int i, isPrime = 1;
    if (n <= 1) {
        isPrime = 0;
    } else {
        for (i = 2; i <= n / 2; i++) {
            if (n % i == 0) {
                isPrime = 0;
                break;
            }
        }
    }
    if (isPrime == 1) {
        printf("%d is a prime number.\n", n);
    } else {
        printf("%d is not a prime number.\n", n);
    }
}

int main() {
    int num;
    printf("Enter a positive integer: ");
    scanf("%d", &num);
    checkPrime(num);
    return 0;
}
```

## Output:
**Case 1:**
```text
Enter a positive integer: 7
7 is a prime number.
```

**Case 2:**
```text
Enter a positive integer: 10
10 is not a prime number.
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to optimize this by checking up to the **square root** of the number instead?
