# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:A
In a gaming lounge, there is only one master console power switch that controls all gaming consoles. Whenever a player turns on any console, it internally triggers the master power. The master switch must ensure only one instance is ever created, regardless of how many times it's accessed, to prevent power fluctuations.

Every time a player accesses the master switch, it logs an access count. Since the switch is Singleton, the count should increment globally and reflect shared state.

## AIM:
To implement the Singleton design pattern in Java to ensure only a single instance of a MasterPowerSwitch class controls global access tracking across multiple players.

## ALGORITHM :
1. Start the program and initialize a Scanner object to capture user inputs.

2. Define a class MasterPowerSwitch with a private constructor to prevent direct outside instantiation.

3. Provide a static method getInstance() that instantiates the class only once and returns the shared instance.

4. Read the total number of players followed by each individual player's name using a loop structure.

5. Retrieve the single instance of the switch using MasterPowerSwitch.getInstance() and increment the global counter.

6. Print the player's name along with the globally shared access count and stop the program




## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: GOKUL SACHIN K
RegisterNumber:  212223220025
*/
```

## SOURCE CODE:


```
import java.util.*;

class MasterPowerSwitch {

    private static MasterPowerSwitch instance;
    private int accessCount = 0;

    private MasterPowerSwitch() {
    }

    public static MasterPowerSwitch getInstance() {
        if (instance == null) {
            instance = new MasterPowerSwitch();
        }
        return instance;
    }

    public int logAccess() {
        accessCount++;
        return accessCount;
    }
}

public class prog {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {

            String player = sc.nextLine();

            MasterPowerSwitch power = MasterPowerSwitch.getInstance();

            int count = power.logAccess();

            System.out.println(player + 
                " accessed Master Power Switch. Total accesses so far: " 
                + count);
        }

        sc.close();
    }
}
```




## OUTPUT:


<img width="943" height="192" alt="image" src="https://github.com/user-attachments/assets/d4007cee-6de8-4f2e-a480-a5e48c3ea95e" />

## RESULT:
Thus the program to implement SDP was executed successfully.
