# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE:17-09-2026
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
1. Start the program.
2. Declare two 2D arrays, A and B, of the same size.
3. Initialize Matrix A with all odd numbers and Matrix B with all even numbers.
4. Create another 2D array C to store the sum of corresponding elements of A and B.
5. For each element position (i, j): `Compute C[i][j] = A[i][j] + B[i][j].`  

## Program:
```
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
```

## Output:
<img width="467" height="614" alt="image" src="https://github.com/user-attachments/assets/3060b837-8702-49d3-b79a-dbf022157a75" />



## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
