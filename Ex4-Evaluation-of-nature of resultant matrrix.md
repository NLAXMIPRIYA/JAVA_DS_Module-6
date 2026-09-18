# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE: 18-09-2026
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
1. Start and read the dimensions of the matrices.
2. Read Matrix A containing odd numbers and Matrix B containing even numbers.
3. Add corresponding elements: C[i][j] = A[i][j] + B[i][j].
4. Display the resulting matrix.
5. Stop and conclude that the resulting matrix contains only odd numbers, because Odd + Even = Odd. 

## Program:
```
/*
Program to ind the nature of resultant matrrix.
Developed by: N Laxmi Priya
RegisterNumber:  212225040196

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int rows = sc.nextInt();
        int cols = sc.nextInt();

        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        int[][] C = new int[rows][cols];

        // Read Matrix A
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                A[i][j] = sc.nextInt();
            }
        }

        // Read Matrix B
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                B[i][j] = sc.nextInt();
            }
        }

        // Matrix Addition
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                C[i][j] = A[i][j] + B[i][j];
            }
        }

        // Display Result
        System.out.println("Resulting Matrix:");

        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                System.out.print(C[i][j] + " ");
            }
            System.out.println();
        }

        System.out.println("Nature: Odd");
    }
}
*/
```

## Output:


<img width="358" height="236" alt="image" src="https://github.com/user-attachments/assets/72f58e1f-1c3b-4b9b-a320-82cacd45d34e" />


## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
