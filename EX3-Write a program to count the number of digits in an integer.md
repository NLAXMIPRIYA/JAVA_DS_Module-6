# EX3 Write a program to count the number of digits in an integer.
## DATE:
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start and read an integer n.

2. If n is between -9 and 9, return 1 as the base case.

3. Divide n by 10 to remove its last digit.

4. Recursively count the digits of n / 10 and add 1 to the result.

5. Stop and display the total number of digits.  

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: N Laxmi Priya
RegisterNumber:  212225040196
*/

import java.util.Scanner;

public class Main {

    static int countDigits(int n) {

        // Base case
        if (n >= -9 && n <= 9) {
            return 1;
        }

        // Recursive call
        return 1 + countDigits(n / 10);
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter an integer: ");
        int n = sc.nextInt();

        System.out.println("Number of digits: " + countDigits(n));
    }
}
```

## Output:

<img width="365" height="128" alt="image" src="https://github.com/user-attachments/assets/c08fff2f-32f7-4e44-9fed-8c9a51774fb8" />



## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
