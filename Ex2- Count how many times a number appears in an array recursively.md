# Ex2 Count how many times a number appears in an array recursively.
## DATE:17-09-2026
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1. Start the program.  
2. Read the number of elements and store them in an array.  
3. Get the number to be counted from the user.  
4. Define a recursive function `countOccurrences()` that returns how many times the number appears.  
5. Use base and recursive conditions to count occurrences.  
6. Display the result.  
7. Stop the program.

## Program:
```
/*
Program Count how many times a number appears in an array recursively.
Developed by: KANDUKURI GOUTHAM
RegisterNumber: 212223110019
*/

import java.util.Scanner;
public class CountOccurrences {
    public static int countOccurrences(int[] arr, int n, int target) {
        int count=0;
        for(int i:arr){
            if(i==target){
                count++;
            }
        }
        return count;
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int size = scanner.nextInt();
        if (size <= 0) {
            System.out.println("Invalid array size. Must be positive.");
            return;
        }
        int[] arr = new int[size];
        for (int i = 0; i < size; i++) {
            arr[i] = scanner.nextInt();
        }
        int target = scanner.nextInt();
        int count = countOccurrences(arr, size, target);
        System.out.println("The number " + target + " appears " + count + " time(s) in the array.");
        scanner.close();
    }
}
```

## Output:
<img width="1267" height="628" alt="image" src="https://github.com/user-attachments/assets/0268bf95-3074-4c06-9390-d7b383956949" />



## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
