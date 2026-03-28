## DATE: 28-03-2026

## AIM:
To write a C program to delete the first element in an array.

## Algorithm
1. **Start** the program.
2. **Declare** an array and a variable `n` for the number of elements.
3. **Read** the elements of the array from the user.
4. **Shift** all elements one position to the left, starting from the second element (index 1) to the last element (index $n-1$), effectively overwriting the first element.
5. **Decrement** the size of the array by 1 ($n = n - 1$).
6. **Display** the updated array.
7. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    int arr[100], n, i;
    printf("Enter number of elements in array: ");
    scanf("%d", &n);
    printf("Enter elements: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    if (n > 0) {
        for (i = 0; i < n - 1; i++) {
            arr[i] = arr[i + 1];
        }
        n--;
        printf("Array after deleting first element: ");
        for (i = 0; i < n; i++) {
            printf("%d ", arr[i]);
        }
    } else {
        printf("Array is empty.");
    }
    printf("\n");
    return 0;
}
```

## Output:
```text
Enter number of elements in array: 5
Enter elements: 10 20 30 40 50
Array after deleting first element: 20 30 40 50 
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to delete an element at a **specific index** instead of just the first one?
