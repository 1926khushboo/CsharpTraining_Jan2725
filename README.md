using System;

class Book
{
    // Define properties
    public string Title { get; set; }
    public string Author { get; set; }
    public int Year { get; set; }

    // Define constructor
    public Book(string title, string author, int year)
    {
        Title = title;
        Author = author;
        Year = year;
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Prompt the user to enter book details
        Console.WriteLine("Enter book's title:");
        string title = Console.ReadLine();

        Console.WriteLine("Enter book's author:");
        string author = Console.ReadLine();

        Console.WriteLine("Enter book's year:");
        int year = Convert.ToInt32(Console.ReadLine());

        // Create an instance of the Book class
        Book book = new Book(title, author, year);

        // Print book details with the desired format
        Console.WriteLine();
        Console.WriteLine("Book Title: " + book.Title);
        Console.WriteLine("Book Author: " + book.Author);
        Console.WriteLine("Book Year: " + book.Year);
    }
}
Output:Enter book's title:
Enter book's author:
Enter book's year:

Book Title: The Great Gatsby
Book Author: F. Scott Fitzgerald
Book Year: 1925
