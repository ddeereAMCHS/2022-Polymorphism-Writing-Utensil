# Polymorphism WritingUtensil

## Due: Tue 10/3 at 11:59 PM

- Create a WritingUtensil class
- The WritingUtensil class should have the following data members:
  - The brand
  - The color
- Write a default constructor
- Write a parameterized constructor that sets all two data members
- Write getter and setter methods for each data member
- Write a toString method that returns the color and brand of the WritingUtensil separated by a space
- Write a write method that takes a String as a parameter and prints it to the screen
  - Each call to the write method should start on a new line
- - - - - - - - - - - -
- Create a Pen class that is a subclass of the WritingUtensil class
- The class should have the following private data members in addition to its inherited members:
  - The thickness
  - The ink level (default value is 50)
  - The status of whether the pen is clicked or not
- Write a default constructor
- Write a parameterized constructor that sets all five data members
- Write getter and setter methods for each data member specific to the Pen class
- Write a click method that toggles the status of whether the pen is clicked or not
- Override the toString method to return the thickness of the Pen followed by the color and brand of the Pen separated by a space followed by the word "pen"
- Override the write method to adhere to the following conditions
  - the Pen can only write if it is clicked
    - if the Pen cannot write, nothing should be printed to the screen
  - the Pen can only write as many characters as it has ink for
    - each character (including spaces) requires 1 ink to write
  - decrease the ink level of the Pen after writing
- - - - - - - - - - - -
- Create a Marker class that is a subclass of the WritingUtensil class
- The class should have the following private data members in addition to its inherited members:
  - The tip type
- Write a default constructor
- Write a parameterized constructor that sets all three data members
- Write getter and setter methods for each data member specific to the Marker class
- Override the toString method to return the tip type followed by the color and brand of the Marker separated by a space followed by the word "marker"
- Override the write method to adhere to the following conditions
  - If the tip type is "chisel", the Marker will write in all uppercase
  - If the tip type is "fine", the Marker will write in all lowercase
- - - - - - - - - - - -
- Create a program called `WritingTester.java`
- Create an ArrayList of WritingUtensil objects
- Prompt the user for a filename
- Read in the data from that file and create an object with that data using the parameterized constructor
  - Each line will contain the data for one object
- Add the object to the ArrayList
- Prompt the user for another filename
- Read each line into an ArrayList of Strings
- Print each WritingUtensil object
- For each WritingUtensil object in the ArrayList
  - Print the object
  - Call the write method for each line from the list of Strings
  - Print a blank line

***Example Input:***\
objects1.txt\
lines1.txt\
***Example Contents of objects1.txt:***\
WritingUtensil; Papermate; gray\
Pen; Pilot; blue; 0.7; 50; clicked\
Marker; Crayola; green; chisel\
Pen; Papermate; orange; 0.5; 100; clicked\
Marker; Sharpie; black; fine\
***Example Contents of lines1.txt:***\
Hello there\
I've got a bad feeling about this\
May the Force be with you\
***Example Output:***\
gray Papermate\
Hello there\
I've got a bad feeling about this\
May the Force be with you\
\
0.7 blue Pilot pen\
Hello there\
I've got a bad feeling about this\
May th\
\
chisel green Crayola marker\
HELLO THERE\
I'VE GOT A BAD FEELING ABOUT THIS\
MAY THE FORCE BE WITH YOU\
\
0.5 orange Papermate pen\
Hello there\
I've got a bad feeling about this\
May the Force be with you\
\
fine black Sharpie marker\
hello there\
i've got a bad feeling about this\
may the force be with you