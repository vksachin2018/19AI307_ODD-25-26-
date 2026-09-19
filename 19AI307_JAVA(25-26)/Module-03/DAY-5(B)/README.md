# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to convert a string to an integer using a wrapper class and perform addition.

## AIM:
To convert string inputs into integers using the wrapper class and perform addition.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Add the two integers.
4.	Display the sum.





## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: GOKUL SACHIN K
RegisterNumber:  212223220025
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String str1 = scanner.next();

        String str2 = scanner.next();

        scanner.close();

        try {
            int num1 = Integer.parseInt(str1);
            int num2 = Integer.parseInt(str2);


            int sum = num1 + num2;
            System.out.println("Sum = " + sum);
        } catch (NumberFormatException e) {
            System.out.println("Invalid input. Please enter a valid number.");
        }
    }
}
```






## OUTPUT:

<img width="1223" height="414" alt="image" src="https://github.com/user-attachments/assets/e11dbc1a-45c7-4d20-9895-e2a3432588c0" />



## RESULT:
The program successfully converts strings to integers and displays their sum.
