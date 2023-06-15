### EX NO : 06
# <p align="center">Operator-Overloading</p>


## Aim:
To write a C# program to pass values through constructors and overload equal operators by checking whether objects are equal using operator overloading. 
 
## Algorithm:
### Step1:
Create a class named program.
### Step 2:
Create two constructors with different arguments to implement operator overloading
### Step 3:
Create boolean operators to check equals and not equal condition and to implement operator overloading.
### Step 4:
Create a Main function
### Step 5:
Create two objects. One without arguments & the other with arguments
### Step 6:
Check whether the objects are equal or not using if-else condition
 
 
 ## Program:
 ```c#
 NAME:VIRGIL JOVITA A
 REG NO:212221240062
 using System;

namespace OperatorOverloading
{
    class program
    {
        public static bool operator ==(program p1, program p2)
        {
            return p1.Equals(p2);
        }
        /*public static bool operator ==(program p3, program p4)
        {
            return p3.Equals(p4);
        }*/

        public static bool operator !=(program p1, program p2)
        {
            return !(p1 == p2);
            //return !(p3 == p4);
        }

        public int p1,p2;
        public program()
        {
            p1 = 45;
            p2 =15;
        }

        public program(int p3, int p4)
        {
            p1 = p3;
            p2 = p4;
        }
        public static void Main()
        {
            program p1 = new program();
            program p2 = p1;

            if (p1 == p2)
            {
               
                Console.WriteLine("both the objects are equal");
            }

            else if (p1 != p2)
            {
                Console.WriteLine("both the objects are not equal");
            }
        }
    }
}

 ```

 
## Output:
![image](ama.png)

 
## Result:
C# program to find the volume of a box using operator overloading is implemented successfully.
