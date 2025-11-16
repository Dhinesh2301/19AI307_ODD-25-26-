# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Maintain two int variables a and b, read their initial values from user. Use synchronized block to swap them and print swapped values.

## AIM:


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: DHINESH R
RegisterNumber: 212223220019 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class SwapUsingSynchronized {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        Object lock = new Object();

        synchronized (lock) {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
        sc.close();
    }
}
```


## OUTPUT:
<img width="457" height="390" alt="image" src="https://github.com/user-attachments/assets/2fb44153-47e4-4ac3-8872-e321e221fc56" />



## RESULT:
Therefore the program successfully swaps two integers within a synchronized block, ensuring safe and controlled access.

