# EX3 Write a program to count the number of digits in an integer.
## DATE:17-09-2026
## AIM:
To write a program to count the number of digits in an integer

## Algorithm
1. Start the program.
2. Declare an integer variable n and count = 0.
3. Read the integer number n from the user.
4. If n is 0, then the count of digits is 1.
5. Otherwise, Repeat the steps while n is not equal to 0. Divide n by 10. Increment count by 1.
6. Display the value of count.
7. Stop the program. 

## Program:
```
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
```

## Output:
<img width="619" height="238" alt="image" src="https://github.com/user-attachments/assets/2578b19a-e8d1-4ce8-83c7-5c6f3065d81b" />



## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
