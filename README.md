# Linked-Lists-and-Circle-Vectors
A project exploring the functionalities of two types of lists - Linked Lists and Circle Vectors

This is a project I built in the Data Structures course I am currently taking that explores the use and functionality of two different types of list storage mechanisms that aren't generally built into system/libraries. There are two classes - LinkedList and CircVec - that each have the same functions implemented to match the respective type of list. The two classes offer quicker searching, insertion, deletion, etc of list items and variability in memory without having to shift many items and lower time complexity.

# Features and Functionalities:
Each class features a default constructor, a functions that give size and whether the list is empty, functions that add and remove from the front of the list, functions that add and remove from the back of the list, clear functions, destructors, search based on index or item functions, copy constructors, assignment operators, and a couple unique remove functions to play with the usability of each list.

# Languages, Programs, and Tools
This project was coded in C++ in VisualStudioCode on a WSL: Ubuntu Linux remote window. It utilizes a lot of pointers and memory management in both the LinkedList nodes being pointers and CircVecs being shifted over an underlying array. The project also uses GoogleTest suites to test for common bugs and function errors, and a Makefile for ease of testing and running.

# Process
I first started with the headers of each function I wished to have for the classes in their respective header files, then wrote the GTest cases in separate cpp files. The functions were broken up into a few different parts - core, enhanced, and augmented - that are ordered based on commonality of bugs, ease of understanding and programming, and required functions for a list to work properly versus some more additions to make the lists more useful. I would write the test for a section, then code the functions within that section, then use the written tests to ensure my code worked as intended.

# Challenges
The main challenge with this project was ensuring proper memory management, especially with the LinkedList class. A missed dereference symbol or improper looping could lead to memory leaks, loss of data, segmentation faults, and more unexpected behaviors. The other significant challenge was figuring out how the mapping in the CircVec class worked when it the list itself didn't exactly fit the underlying array and was instead shifted. To help with this, I made a private function that got the index on the array of an item from the index in the list it was in, which helped significantly in getting through that challenge.
