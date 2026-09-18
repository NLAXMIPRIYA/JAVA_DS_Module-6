# Ex5 Count Inversions in an Array
## DATE:
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm
1. Start and read the array elements.
2. Set count = 0 to store the number of inversions.
3. Compare every element arr[i] with the elements after it using arr[j].
4. If i < j and arr[i] > arr[j], increment count.
5. Stop and display the total number of inversions.  

## Program:
```
/*
Program toto Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: 
RegisterNumber:  
*/
import java.util.Scanner;

public class Main {

    static int countInversions(int[] arr) {
        int count = 0;

        for (int i = 0; i < arr.length; i++) {
            for (int j = i + 1; j < arr.length; j++) {

                if (arr[i] > arr[j]) {
                    count++;
                }
            }
        }

        return count;
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int result = countInversions(arr);

        System.out.println("Number of inversions: " + result);
    }
}
```

## Output:


<img width="374" height="109" alt="image" src="https://github.com/user-attachments/assets/b5b3dea6-a9f7-4177-bf34-9dc8171ab6f8" />



## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
