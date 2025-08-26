/*
============================================================================
 Title      : Classes and Objects in C++
 
 Aim        : To study and implement Classes and Objects in C++.
 
 Software   : Visual Studio Code (VS Code)
 
============================================================================

Objective:
- To understand the concept of Object-Oriented Programming (OOP).
- To learn how to create and use classes and objects in C++.
- To implement encapsulation by grouping data members and functions together.
- To study the advantages of OOP over traditional Procedural Programming.

============================================================================
Theory:

1. Introduction to Object-Oriented Programming (OOP):
   - OOP is a programming paradigm that organizes code into reusable units called
     "objects", which are created from "classes".
   - It focuses on representing real-world entities using objects, combining both
     data (attributes) and functions (behaviors).

2. What is a Class?
   - A class in C++ is a user-defined data type that acts as a blueprint
     for creating objects.
   - It defines data members (variables) and member functions (methods) 
     that operate on the data.
   - Example: 
       class Car {
           string color;
           int speed;
           void start();
       };

   - Here, Car is a class with properties (color, speed) and behavior (start).

3. What is an Object?
   - An object is an instance of a class.
   - While the class defines the structure, the object holds real data.
   - Example:
       Car car1, car2;
     Here car1 and car2 are two objects created from the Car class.

4. Importance of Classes and Objects:
   - Classes and objects help in modeling real-world problems.
   - Example: A "Student" class may have name, roll number, and marks 
     as data members, and methods like setData() and displayData().

5. Features of Classes and Objects:
   a) Encapsulation:
      - Data and functions are bound together inside a class.
      - Prevents direct access to internal details, ensuring data security.
   b) Abstraction:
      - Hides complex implementation details and shows only the necessary features.
      - Example: We use the 'cout' object without worrying about how it works internally.
   c) Reusability:
      - Once created, a class can be used to make multiple objects.
      - Reduces redundancy and improves modularity.
   d) Modularity:
      - Large problems can be divided into small classes and objects,
        making the program more manageable and maintainable.
   e) Data Hiding:
      - By using access specifiers (private, public, protected), data security can be ensured.

6. Access Specifiers in Classes:
   - public    → members accessible from anywhere.
   - private   → members accessible only within the class.
   - protected → members accessible within the class and derived classes.

7. Difference Between Class and Object:

   | Feature            | Class                            | Object                     |
   |--------------------|----------------------------------|----------------------------|
   | Definition         | Blueprint for creating objects   | Instance of a class        |
   | Memory Allocation  | No memory is allocated           | Memory is allocated        |
   | Example            | class Student { ... };           | Student s1, s2;            |

8. Real-Life Analogy:
   - Think of a "class" as a blueprint of a house.
   - The blueprint defines structure and design, but it’s not a real house.
   - When you build a house based on the blueprint, that house is an "object".
   - Similarly, in C++, a class is just a plan, and objects are real usable instances.

============================================================================
 Program: Demonstration of Classes and Objects in C++
============================================================================
*/

#include <iostream>
using namespace std;

// Class definition
class Student {
    // Data members (attributes)
    string name;
    int rollNo;
    float marks;

public:
    // Member function to set values (behaviors)
    void setData(string n, int r, float m) {
        name = n;
        rollNo = r;
        marks = m;
    }

    // Member function to display values
    void displayData() {
        cout << "Name: " << name << endl;
        cout << "Roll No: " << rollNo << endl;
        cout << "Marks: " << marks << endl;
    }
};

// Main function
int main() {
    // Creating objects of Student class
    Student s1, s2;

    // Setting values using objects
    s1.setData("Ishika", 101, 88.5);
    s2.setData("Rahul", 102, 92.0);

    // Displaying values using objects
    cout << "Student 1 Details:" << endl;
    s1.displayData();

    cout << "\nStudent 2 Details:" << endl;
    s2.displayData();

    return 0;
}


SAMPLE OUTPUT:

     Traversal of an array-
               Original array:
               10 20 30 40 50 
               Traversed array:
               50 40 30 20 10 

    Character printing of strings:
              Enter a string:
              Hello 
              Characters of string entered are:
              H
              e
              l
              l
              o

    Basic pointer arithematic:
             Data type: int.
             Value of a: 2
             Initial address of a: 0x7ffe08ddab8c
             Incremented address of a: 0x7ffe08ddab90

             Data type: bool.
             Value of b: 1
             Initial address of b: 1
             Incremented address of b: 2

             Data type: double
             Value of c: 10.5
             Initial address of c: 0x7ffe08ddab80
             Incremented address of c: 0x7ffe08ddab88

             Data type: float.
             Value of d: 23
             Initial address of d: 0x7ffe08ddab7c
             Incremented address of d: 0x7ffe08ddab80

    Addition & Subraction using pointer:
            The difference between the values at index 4 and 2 is:20
            The addition of the values of array at index 4 and 2 is:80

            
============================================================================
 Conclusion:
- A class is a user-defined data type that contains variables and functions.
- An object is an instance of a class that holds real values.
- Classes and objects are the foundation of Object-Oriented Programming (OOP).
- They provide encapsulation, abstraction, modularity, and reusability in C++.
- Using classes and objects makes programs easier to design, understand,
  maintain, and extend for complex real-world applications.
============================================================================


