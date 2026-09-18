# Ex2 Count how many times a number appears in an array recursively.
## DATE: 18-09-2026
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1. Start and initialize the array and the target number.

2. If n == 0, return 0 as the base case.

3. Recursively count the occurrences of the target in the first n-1 elements.

4. If the last element equals the target, increment the count by 1; otherwise, return the existing count.

5. Stop and display the total number of occurrences.  

## Program:
```
/*
Program Count how many times a number appears in an array recursively.
Developed by: N Laxmi Priya
RegisterNumber:  212225040196
*/

public class Main {

    static int countOccurrences(int[] arr, int n, int target) {

        // Base case
        if (n == 0) {
            return 0;
        }

        // Recursive call
        int count = countOccurrences(arr, n - 1, target);

        // Check the last element
        if (arr[n - 1] == target) {
            return count + 1;
        }

        return count;
    }

    public static void main(String[] args) {

        int[] arr = {2, 5, 3, 5, 7, 5, 8};
        int target = 5;

        int result = countOccurrences(arr, arr.length, target);

        System.out.println("Occurrences: " + result);
    }
}
```

## Output:

<img width="369" height="162" alt="image" src="https://github.com/user-attachments/assets/e02deb3c-2738-4202-be7d-c56d1c68e5e1" />


## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
