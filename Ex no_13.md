## DATE: 28-03-2026

## AIM:
To write a C program to read the elements and print only the odd elements in the 2D array.

## Algorithm
1. **Start** the program.
2. **Declare** a 2D array (e.g., `arr[10][10]`) along with variables for row size ($r$), column size ($c$), and loop counters ($i, j$).
3. **Input** the number of rows and columns, then use nested loops to **Read** the elements into the 2D array.
4. **Use** nested loops again to traverse each element of the array.
5. **Check** if the current element `arr[i][j]` is odd using the condition `arr[i][j] % 2 != 0`.
6. **Print** the element if the condition is true.
7. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    int arr[10][10], r, c, i, j;
    printf("Enter number of rows and columns: ");
    scanf("%d %d", &r, &c);
    printf("Enter elements of the array:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            scanf("%d", &arr[i][j]);
        }
    }
    printf("Odd elements in the 2D array are:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            if (arr[i][j] % 2 != 0) {
                printf("%d ", arr[i][j]);
            }
        }
    }
    printf("\n");
    return 0;
}
```

## Output:
```text
Enter number of rows and columns: 2 2
Enter elements of the array:
10 15
21 30
Odd elements in the 2D array are:
15 21 
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to calculate the **sum of these odd elements** as well?
