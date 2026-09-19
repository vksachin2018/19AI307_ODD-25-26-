# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a java program for determine the priority and name of the current thread.

## AIM:
To write a Java program to determine and display the name and priority of the current thread.

## ALGORITHM :
1.	Start the program.

2. Import required classes (Scanner).

3. Read thread name from the user.

4. Get the current thread using Thread.currentThread().

5. Set the thread name using setName().

6. Retrieve and display thread priority using getPriority().

7. Retrieve and display thread name using getName().

8. Print the thread object details.

9. End the program.




## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: GOKUL SACHIN K
RegisterNumber:  212223220025
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String threadName = sc.nextLine();

        Thread t = Thread.currentThread();
        t.setName(threadName);

        System.out.println("Priority of Thread: " + t.getPriority());
        System.out.println("Name of Thread: " + t.getName());
        System.out.println(t);

        sc.close();
    }
}
```






## OUTPUT:
<img width="564" height="178" alt="image" src="https://github.com/user-attachments/assets/149ba57b-db7e-4982-966b-ceb434297053" />



## RESULT:
The Java program successfully determines and displays the current thread’s name and priority using the Thread class.
