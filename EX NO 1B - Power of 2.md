
# EX 1B Power of 2
## **DATE: 10-08-2025**

## AIM:
To write a Java program to for given constraints.Given an integer n, return true if it is a power of two. Otherwise, return false.

An integer n is a power of two, if there exists an integer x such that n == 2x.

## Algorithm
1. Start the program.
2. Read the integer value **n** from the user.
3. If **n ≤ 0**, return false (because powers of 2 are always positive).
4. Use a loop to check whether **n** becomes 1 when repeatedly divided by 2.
5. If n becomes 1, display **true**; otherwise display **false**.

---

## Program:
```
/*
Developed by: ARCHANA S
Register Number:  212223040019
*/
import java.util.Scanner;

public class Solution {

    public boolean isPowerOfTwo(int n) {
        if(n==1) return true;
        long i=1;
        while((i<<1)<=n){
            if(i<<1 == n) return true;
            i = i<<1;
        }
        return false;
     
     
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Solution sol = new Solution();
        int n = scanner.nextInt();

        boolean result = sol.isPowerOfTwo(n);
        System.out.println(result);

        scanner.close();
    }
}

```

## Output:
<img width="1264" height="242" alt="image" src="https://github.com/user-attachments/assets/9ead7ad4-b02e-405e-9e35-b2f149fa3e67" />

---

## **Result:**

The program was successfully implemented and the expected output was verified.

---
