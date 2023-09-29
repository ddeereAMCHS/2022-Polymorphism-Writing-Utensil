# Inheritance Book

## Due: Tue 9/26 at 11:59 PM

- Create a Book class
- The class should have the following private data members:
  - Title
  - Author
  - Number of pages
- Write a default constructor
- Write a parameterized constructor that sets all three data members
- Write getter and setter methods for each data member
- Write a toString method that returns the title and the author with the word "by" in between them
  - Ex. The Cat in the Hat by Dr. Seuss
- - - - - - - - - - - -
- Create a Textbook class that is a subclass of the Book class
- The class should have the following private data members in addition to its inherited members:
  - edition
- Write a default constructor
- Write a parameterized constructor that sets all four data members
- Write getter and setter methods for each data member specific to the Textbook class
- Override the toString method to return the title and the author with the word "by" in between them followed by the edition number
  - Ex. Calculus by Tom Smith, ed. 1
- - - - - - - - - - - -
- Create a Novel class that is a subclass of the Book class
- The class should have the following private data members in addition to its inherited members:
  - genre
- Write a default constructor
- Write a parameterized constructor that sets all four data members
- Write getter and setter methods for each data member specific to the Novel class
- - - - - - - - - - - -
- Create a program called `BookTester.java`
- Prompt the user for a filename
- Read in the data from that file and create a Textbook object with that data using the parameterized constructor
- Prompt the user for another filename
- Read in the data from that file and create a Novel object with that data using the parameterized constructor
- Print the Textbook object
- Print the Novel object

***Example Input:***\
textbook1.txt\
novel1.txt\
***Example Output:***\
Calculus by Tom Smith, ed. 1\
The Cat in the Hat by Dr. Seuss
