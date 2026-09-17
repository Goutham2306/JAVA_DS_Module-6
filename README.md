EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
DATE:17-09-2026
AIM:

To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Algorithm

    Start the program.
    Read the number of elements and store them in an array.
    Define a recursive function findMin() that compares elements to find the minimum.
    Base condition: If the array has one element, return that element.
    Recursive step: Compare the last element with the minimum of the rest of the array and return the smaller one.
    Display the minimum value.
    Stop the program.

Program:

/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: KANDUKURI GOUTHAM
RegisterNumber: 212223110019
*/

import java.util.*;

public class Main {
    static int getMin(int[] arr, int i, int n) {
        if (i == n - 1) {
            return arr[i];
        }
        int minRest = getMin(arr, i + 1, n);
        return Math.min(arr[i], minRest);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.println(getMin(arr, 0, n));
    }
}

Output:
image
Result:

Thus the JAVA program to find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully.

Ex2 Count how many times a number appears in an array recursively.
DATE:17-09-2026
AIM:

To write a Java program to Count how many times a number appears in an array recursively.
Algorithm

    Start the program.
    Read the number of elements and store them in an array.
    Get the number to be counted from the user.
    Define a recursive function countOccurrences() that returns how many times the number appears.
    Use base and recursive conditions to count occurrences.
    Display the result.
    Stop the program.

Program:

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

Output:
image
Result:

Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.

EX3 Write a program to count the number of digits in an integer.
DATE:17-09-2026
AIM:

To write a program to count the number of digits in an integer
Algorithm

    Start the program.
    Declare an integer variable n and count = 0.
    Read the integer number n from the user.
    If n is 0, then the count of digits is 1.
    Otherwise, Repeat the steps while n is not equal to 0. Divide n by 10. Increment count by 1.
    Display the value of count.
    Stop the program.

Program:

/*
Program to to count the number of digits in an integer
Developed by: KANDUKURI GOUTHAM
RegisterNumber: 212223110019
*/

import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n=sc.nextInt();
        String a=String.valueOf(n);
        int count=0;
        for(int i=0;i<a.length();i++){
            count++;
        }
        System.out.println("Number of digits: " + count);
    }
}

Output:
image
Result:

Thus, the Java program to to count the number of digits in an integer is implemented successfully.

Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
DATE:17-09-2026
AIM:

To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.
Algorithm

    Start the program.
    Declare two 2D arrays, A and B, of the same size.
    Initialize Matrix A with all odd numbers and Matrix B with all even numbers.
    Create another 2D array C to store the sum of corresponding elements of A and B.
    For each element position (i, j): Compute C[i][j] = A[i][j] + B[i][j].

Program:

/*
Program to ind the nature of resultant matrrix.
Developed by: KANDUKURI GOUTHAM
RegisterNumber: 212223110019
*/
import java.util.*;
class prog{
    public static void main(String[] args){
    Scanner sc=new Scanner(System.in);
    int r=sc.nextInt();
    int co=sc.nextInt();
    int[][] a=new int[r][co];
    int[][] b=new int[r][co];
    int[][] c=new int[r][co];
    for(int i=0;i<r;i++){
        for(int j=0;j<co;j++){
            a[i][j]=sc.nextInt();
        }
    }
    for(int i=0;i<r;i++){
        for(int j=0;j<co;j++){
            b[i][j]=sc.nextInt();
        }
    }
    for(int i=0;i<r;i++){
        for(int j=0;j<co;j++){
            c[i][j]=a[i][j]+b[i][j];
        }
    }
    for(int i=0;i<r;i++){
        for(int j=0;j<co;j++){
            System.out.print(c[i][j]+" ");
        }
        System.out.println(" ");
    }
    }
}

Output:
image
Result:

Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.

Ex5
Count Inversions in an Array
DATE: 17-09-2026
AIM:

To write a Java program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Algorithm

    Start the program.
    Declare an array arr[] and a variable count = 0 to store the number of inversions.
    Read the array elements from the user.
    For each pair of elements (arr[i], arr[j]), check if arr[i] > arr[j] and i < j.
    If the above condition is true, increment the inversion count.
    Continue until all pairs are checked.
    Display the total number of inversions found in the array and stop the program.

Program:

/*
Program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: KANDUKURI GOUTHAM
RegisterNumber: 212223110019
*/

import java.util.Scanner;

public class CountInversions {
    public static int mergeSortAndCount(int[] arr, int left, int right) {
        int count = 0;
        if (left < right) {
            int mid = (left + right) / 2;
            count += mergeSortAndCount(arr, left, mid);
            count += mergeSortAndCount(arr, mid + 1, right);
            count += mergeAndCount(arr, left, mid, right);
        }
        return count;
    }

    private static int mergeAndCount(int[] arr, int left, int mid, int right) {
        int[] leftArr = new int[mid - left + 1];
        int[] rightArr = new int[right - mid];

        for (int i = 0; i < leftArr.length; i++) leftArr[i] = arr[left + i];
        for (int i = 0; i < rightArr.length; i++) rightArr[i] = arr[mid + 1 + i];

        int i = 0, j = 0, k = left, swaps = 0;

        while (i < leftArr.length && j < rightArr.length) {
            if (leftArr[i] <= rightArr[j]) {
                arr[k++] = leftArr[i++];
            } else {
                arr[k++] = rightArr[j++];
                swaps += (leftArr.length - i); // Count inversions
                
            }
       
        }

        while (i < leftArr.length) arr[k++] = leftArr[i++];
        while (j < rightArr.length) arr[k++] = rightArr[j++];

        return swaps;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) arr[i] = sc.nextInt();
        System.out.println(mergeSortAndCount(arr, 0, n - 1));
    }
}

Output:
image
Result:

Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j is implemented successfully.
