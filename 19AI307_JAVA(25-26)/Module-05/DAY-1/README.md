# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)

## AIM:

To write a Java program to demonstrate chaining of streams using BufferedReader on top of InputStreamReader on top of System.in for reading user input.

## ALGORITHM :
1. Start the program. 

2. Create a BufferedReader object using InputStreamReader(System.in).
  
3. Read the user’s name using readLine() 

4. Read the user’s age using readLine() and convert it to integer using Integer.parseInt().

5.  Display the entered user details.

6.   Stop the program. 





## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: GOKUL SACHIN K
RegisterNumber:  212223220025
*/
```

## SOURCE CODE:

```
import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.io.IOException;

public class Main {
    public static void main(String[] args) throws IOException {

        BufferedReader br = new BufferedReader(
                                new InputStreamReader(System.in));

        String name = br.readLine();
        int age = Integer.parseInt(br.readLine());

        System.out.println("--- User Details ---");
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}
```





## OUTPUT:
<img width="481" height="382" alt="image" src="https://github.com/user-attachments/assets/2a54383a-5d16-483f-8349-d1a1777df567" />



## RESULT:
The program successfully demonstrates chaining of streams in Java using BufferedReader, InputStreamReader, and System.in to read input from the user and display the entered details.
