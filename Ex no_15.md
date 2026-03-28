## DATE: 28-03-2026

## AIM:
To write a C program that reads a one-dimensional array of integers and replaces all even elements with the character 'E'.

## Algorithm
1. **Start** the program.
2. **Declare** an integer array (e.g., `arr[100]`) and a variable `n` for the number of elements.
3. **Read** the size of the array and the elements from the user.
4. **Iterate** through the array using a `for` loop:
    * Check if the current element is even using the condition `arr[i] % 2 == 0`.
    * If even, print the character 'E' instead of the number.
    * If odd, print the original integer.
5. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    int arr[100], n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter the elements: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Updated sequence: ");
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    printf("\n");
    return 0;
}
```

## Output:
```text
Enter the number of elements: 5
Enter the elements: 10 11 12 13 14
Updated sequence: E 11 E 13 E 
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to perform this replacement within the array itself using a **char array** to store the results?
