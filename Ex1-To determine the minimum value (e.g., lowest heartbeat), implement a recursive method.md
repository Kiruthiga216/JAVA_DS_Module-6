# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm

Start the program.

Read the number of elements and store them in an array.

Define a recursive function findMin() that compares elements to find the minimum.

Base condition: If the array has one element, return that element.

Recursive step: Compare the last element with the minimum of the rest of the array and return the smaller one.

Display the minimum value.

Stop the program.


## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;

public class Main {
    static int getMin(int[] arr, int i, int n) {
        if (i == n - 1) {
            return arr[i];
        }
        int minRest = getMin(arr, i + 1, n);
        return Math.min(arr[i], minRest);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.println(getMin(arr, 0, n));
    }
}
```

## Output:



## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
