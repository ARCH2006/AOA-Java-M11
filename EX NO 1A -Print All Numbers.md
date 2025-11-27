# **EX 1A Print All Numbers**

## **DATE: 8-08-2025**

## **AIM:**

To write a Java program that takes an integer input N from the user and prints all the numbers from 1 to N, separated by spaces, on a single line.

---

## **Algorithm**

1. Start the program.
2. Read the integer value N from the user.
3. Check whether N is greater than 0.
4. If N > 0, use a loop to print numbers from 1 to N.
5. Stop the program.

---

## **Program:**

```java
/*
Program to implement Print All Numbers from 1 to N
Developed by: ARCHANA S
Register Number: 212223040019
*/
import java.util.*;

public class PrintNumbers {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        for(int i =1;i<=n;i++){
            System.out.print(i + (i<n ? " ":""));
        }
    }
    
}
```

---

## **Output:**

<img width="1023" height="203" alt="image" src="https://github.com/user-attachments/assets/8d92cb0d-4969-4def-9f4f-27b00df274ab" />

---

## **Result:**

The program successfully prints all the numbers from 1 to N.

---
