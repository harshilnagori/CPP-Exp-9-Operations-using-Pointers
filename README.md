# CPP-Exp-9-Operations-using-Pointers
# Harshil Nagori
# 24070123046
Collection of programs that involve understanding the basic concepts of pointers, advantages of pointers over arrays, ease of iteration.
Declaring a Pointer

#include <iostream>
using namespace std;

int main(){
    int n = 140;
    int *d = &n;
    cout<<"Value of n: "<<n<<endl;
    cout<<"Value of d: "<<d<<endl;
    cout<<"Pointer dereferencing: "<< *d<<endl;
    cout<<"Address of n :"<<&n<<endl;
    cout<<"Address of pointer d :"<<&d<<endl;

    return 0;
}

Value of n: 140
Value of d: 0x7ffce3d645fc
Pointer dereferencing: 140
Address of n :0x7ffce3d645fc
Address of pointer d :0x7ffce3d645f0

Sample output:

    Pointers of different datatypes and incrementing :

INT COLUMN
Value of pointer: 0x7ffeecce914c
Dereferencing: 140
Address of n: 0x7ffeecce914c
Incrementing pointer: 0x7ffeecce9150
Dereferencing: 1

FLOAT COLUMN
Value of pointer: 0x7ffeecce9148
Dereferencing: 14
Address of f: 0x7ffeecce9148
Incrementing pointer: 0x7ffeecce914c
Dereferencing: 1.96182e-43

DOUBLE COLUMN
Value of pointer: 0x7ffeecce9140
Dereferencing: 40
Address of d: 0x7ffeecce9140
Incrementing pointer: 0x7ffeecce9148
Dereferencing: 2.97621e-312

BOOL COLUMN
Value of pointer: 0x7ffeecce913f
Dereferencing: 1
Address of b: 0x7ffeecce913f
Incrementing pointer: 0x7ffeecce9140
Dereferencing: 0

Enter the number of elements (1-20) :
10

Enter element 0	44

Enter element 1	1004

Enter element 2	235

Enter element 3	123

Enter element 4	567

Enter element 5	34

Enter element 6	8

Enter element 7	3

Enter element 8	77

Enter element 9	44
Array: 	44	1004	235	123	567	34	8	3	77	44

    Basic Arithematic Operation on pointers:

Sum :1140
Difference :860
Multiplication :140000
Division :7

Enter 1 for Maximum number, 0 for Minimum number: 0
Minimum: 0

    Finding a number from an array of numbers :

Enter the number you want to search :45
Oops, Didn't find the number!!

Enter the number you want to search :56
The searched number's index is 9

    Finding the Sum and Average of the array elements :

Enter the number of elements (1-20) :
7

Enter element 0	7

Enter element 1	14

Enter element 2	21

Enter element 3	28

Enter element 4	35

Enter element 5	42

Enter element 6	49
Array :	7	14	21	28	35	42	49
Sum : 196
Average : 28

