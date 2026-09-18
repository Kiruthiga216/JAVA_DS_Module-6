# EX3 Write a program to count the number of digits in an integer.

## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm

Start the program.

Declare an integer variable n and count = 0.

Read the integer number n from the user.

If n is 0, then the count of digits is 1.

Otherwise, Repeat the steps while n is not equal to 0. Divide n by 10. Increment count by 1.

Display the value of count.

Stop the program.

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num, count = 0;

        System.out.print("Enter an integer: ");
        num = sc.nextInt();

        if (num == 0) {
            count = 1;
        } else {
            while (num != 0) {
                num = num / 10;
                count++;
            }
        }

        System.out.println("Number of digits: " + count);
        sc.close();
    }
}
```

## Output:

<img width="596" height="192" alt="image" src="https://github.com/user-attachments/assets/b5e039ba-18b8-4505-87ea-6903ea6752c0" />




## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
