# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).

## AIM:
To implement a Composition relationship in Java where a Library contains multiple Book objects, and each Book is created inside the Library, meaning Books cannot exist independently.

## ALGORITHM :
1. Start the program.

2. Create a Library object.

3. Read number of books n.

4. Read title and author for each book.

5. Create Book objects inside Library and add them to a list.

6. Display all books in the Library.

7. End the program.




## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: GOKUL SACHIN K
RegisterNumber:  212223220025
*/
```

## SOURCE CODE:

```
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {

            String title = sc.nextLine();
            String author = sc.nextLine();

            library.addBook(title, author);
        }

        library.showBooks();

        sc.close();
    }
}

class Book {

    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {

    private List<Book> books = new ArrayList<>();

    public void addBook(String title, String author) {

        Book book = new Book(title, author);

        books.add(book);
    }

    public void showBooks() {

        System.out.println("Books in Library:");

        for (Book book : books) {
            System.out.println("- " + book.getDetails());
        }
    }
}
```





## OUTPUT:

<img width="746" height="414" alt="image" src="https://github.com/user-attachments/assets/0550a18a-be97-4a07-9062-58af95c60b84" />


## RESULT:
Thus the program to implement the composition was executed successfully.
