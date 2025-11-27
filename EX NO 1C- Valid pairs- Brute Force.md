# **EX 1C Valid Pairs using Brute Force Approach**

## **DATE: 21-08-2025**

## **AIM:**

To write a Java program that counts the number of valid pairs (i, j) such that **i < j** and
**|nums[i] – nums[j]| = k**, using the brute force method.

---

## **Algorithm**

1. Start the program.
2. Read the value of **n** and then read **n** elements into the array.
3. Read the value of integer **k**.
4. Use two nested loops to compare every pair (i, j) where **i < j**.
5. Count the pair if the absolute difference equals **k**, then print the result.

---

## **Program:**

```java
/*
Program to count valid pairs using Brute Force Approach
Developed by: ARCHANA S
Register Number: 212223040019
*/
import java.util.Scanner;
import java.util.*;
public class CountPairsWithDifference {
    public static int countKDifference(int[] nums, int k) {
        
        Map<Integer,Integer> map = new HashMap<>();
        int res = 0;
        
        for(int i = 0;i< nums.length;i++){
            if(map.containsKey(nums[i]-k)){
                res+= map.get(nums[i]-k);
            }
            if(map.containsKey(nums[i]+k)){
                res+= map.get(nums[i]+k);
            }
            map.put(nums[i],map.getOrDefault(nums[i],0)+1);
        }
        
        
        return res;
    }   
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] nums = new int[n];
        for (int i = 0; i < n; i++) {
            nums[i] = sc.nextInt();
        }
        int k = sc.nextInt();
        int result = countKDifference(nums, k);
        System.out.println(result);
        sc.close();
    }
}

```

---

## **Output:**

<img width="1020" height="326" alt="image" src="https://github.com/user-attachments/assets/df467aa7-c18b-4c75-9cbd-7897dc9ef9a2" />


## **Result:**

The program was successfully implemented and the expected output was verified.

---
