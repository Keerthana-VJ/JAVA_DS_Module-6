# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE: 05.08.2025
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Read the number of elements n and input all n integers into an array arr.
2. Start the recursive function getMin(arr, 0, n) to find the minimum element.
3. Inside the recursive function, check if the current index i is the last index (i == n−1).If yes, return arr[i] as the minimum.
4. Otherwise, recursively call getMin(arr, i+1, n) to find the minimum of the remaining elements.
5. Compare the current element arr[i] with the minimum of the rest and return the smaller value.   

## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: KEERTHANA V
RegisterNumber: 212223220045
*/
```
```
import java.util.*;

public class Main {
    static int getMin(int[] arr, int i, int n) {
        return (n == 1) ? arr[i] : Math.min(arr[i], getMin(arr, i + 1, n - 1));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.println(getMin(arr, 0, n));
    }
}

```

## Output:

<img width="579" height="295" alt="image" src="https://github.com/user-attachments/assets/4fb43a0a-180c-4718-afd7-5dec1c1de12f" />


## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
