# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?

## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm

Start the program.

Declare two 2D arrays, A and B, of the same size.

Initialize Matrix A with all odd numbers and Matrix B with all even numbers.

Create another 2D array C to store the sum of corresponding elements of A and B.

For each element position (i, j): Compute C[i][j] = A[i][j] + B[i][j].
 

## Program:
```
/*
Program to find the nature of resultant matrix.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
    
        int a=sc.nextInt();
        int b=sc.nextInt();
        int[][] row=new int[a][b];
        int[][] col=new int[a][b];
        int[][] res=new int[a][b];
        for(int i=0;i<a;i++){
            for(int j=0;j<b;j++){
                row[i][j]=sc.nextInt();
            }
        }
    
        for(int i=0;i<a;i++){
            for(int j=0;j<b;j++){
                col[i][j]=sc.nextInt();
            }
        }
    
        for(int i=0;i<a;i++){
            for(int j=0;j<b;j++){
                res[i][j]=row[i][j]+col[i][j];
            }
        }
    
        for(int i=0;i<a;i++){
            for(int j=0;j<b;j++){
                System.out.print(res[i][j]);
                if(j<b-1){
                    System.out.print(" ");
                }
            
            }
            System.out.println();
        }
    }
}
```

## Output:

<img width="408" height="602" alt="image" src="https://github.com/user-attachments/assets/45ac3559-3240-4977-be01-dbb09d3e80f1" />




## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
