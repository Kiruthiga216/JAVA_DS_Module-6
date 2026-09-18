# Ex2 Count how many times a number appears in an array recursively.

## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm

Start the program.

Read the number of elements and store them in an array.

Get the number to be counted from the user.

Define a recursive function countOccurrences() that returns how many times the number appears.

Use base and recursive conditions to count occurrences.

Display the result.

Stop the program



## Program:
```
/*
Program Count how many times a number appears in an array recursively.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.Scanner;

public class CountOccurrencesRecursive {
    static int countOccurrences(int arr[], int n, int key) {
        if (n == 0)
            return 0;
        return (arr[n - 1] == key ? 1 : 0) + countOccurrences(arr, n - 1, key);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();
        int arr[] = new int[n];
        System.out.println("Enter the elements:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();
        System.out.print("Enter number to count: ");
        int key = sc.nextInt();
        System.out.println("The number " + key + " appears " + countOccurrences(arr, n, key) + " times.");
        sc.close();
    }
}
```

## Output:

<img width="812" height="451" alt="image" src="https://github.com/user-attachments/assets/c7659032-8afb-4ade-8d83-983c8b5fe2dd" />




## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
