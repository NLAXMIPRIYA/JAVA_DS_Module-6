# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE: 18-09-2026
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Start and initialize the sensor readings array.

2. If the array contains only one element (n == 1), return that element as the minimum.

3. Recursively find the minimum of the first n-1 elements.

4. Compare the last element with the returned minimum and return the smaller value.

5. Stop and display the minimum sensor reading.
  

## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: N Laxmi Priya
RegisterNumber: 212225040196 
*/

public class Main {

    static int findMin(int[] arr, int n) {

        // Base case
        if (n == 1) {
            return arr[0];
        }

        // Recursive call
        int min = findMin(arr, n - 1);

        // Compare last element with minimum
        if (arr[n - 1] < min) {
            return arr[n - 1];
        }

        return min;
    }

    public static void main(String[] args) {

        int[] readings = {80, 72, 95, 65, 88};

        int minimum = findMin(readings, readings.length);

        System.out.println("Minimum reading: " + minimum);
    }
}
```

## Output:


<img width="366" height="160" alt="image" src="https://github.com/user-attachments/assets/70ced448-7412-4dc0-9da3-eba1b5548847" />


## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
