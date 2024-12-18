# GFG-series---Complete-Interview-Preparation
This repo contains problems and course summary for each topics

1. JAVA LANGUAGE
   1.1 INTRODUCTION, OPERATORS AND DATATYPES
   
Java has JDK which generates bytecode for each platform. So it’s platform independent unlike c/c++.
Java Advantages: independent, no pointer, automatic garbage collection, portable(write once, use anytime)
Java is statically typed language: means we have to declare variable datatype unlike python. So this is fast

Java setup:
JDK, IDE, classpath: it’s a rootpath where all projects are stored which will be used in java software

 ![image](https://github.com/user-attachments/assets/9c180656-942a-41ef-88de-8be358a1a460)


JVM generates bytecode
Dev tools contains debugger. Compiler, document generator etc 

MAIN method:

![image](https://github.com/user-attachments/assets/54be66c9-fcb8-4cc9-a7bc-55db424a845d)

By convention, the name of the main class(a class which contain the main method) should match the name of the file that holds the program

Variables:
There are 3 types of variables:
•	Local Variables: defined within a block or method or constructor
•	Instance Variables
	As instance variables are declared in a class, these variables are created when an object of the class is created and destroyed when the object is destroyed.
	Unlike local variables, we may use access specifiers for instance variables. If we do not specify any access specifier then the default access specifier will be used.
	Initilisation of Instance Variable is not mandatory. Its default value is 0
	Instance Variable can be accessed only by creating objects

•	Static Variables
	we can only have one copy of a static variable per class irrespective of how many objects we create.
	Initilisation of Static Variable is not mandatory. Its default value is 0

 ![image](https://github.com/user-attachments/assets/7b1034a2-4ebb-46bb-a2e4-f91784348ebd)

Convention in java: camelCase for variables like intValueData
Use Caps for constant like MAX_INT = 342313, PIE = 3.14
For float, use value as m=3.14f or typecast with float; else it will throw an error as all fractional values are of double datatype

Non-primitive:
They are always just references. They are stored in heap(used for dynamic programming). All variables of nonprimitive has default values when defined

Wrapper Class:

![image](https://github.com/user-attachments/assets/1cdb84c5-7362-4b0a-96e6-b3a492e7f05a)

Every primitive has non-primitive wrapper class.
Non-primitive type wrapper classes are practically used in java applications. Primitive types are used for efficient purposes.

AUTO-BOXING:
conversion of primitive to wrapper class type is autoboxing. Reverse is known as auto-UNBOXING

Type Conversion:

![image](https://github.com/user-attachments/assets/8b0f7ad9-29aa-493c-908c-cdcbb2130d78)

Narrowing:

![image](https://github.com/user-attachments/assets/96c6247d-9bf2-4d25-b119-fd34a6e45c8e)

Operators associativity:

 ![image](https://github.com/user-attachments/assets/eab5ab12-0666-40ec-b436-7c4811cf7f2f)

Input:
Java input can be read by 2 ways:
1.	Bufferedreader 2. Scanner(easy)

![image](https://github.com/user-attachments/assets/03a84530-0455-4ada-ac6c-b593d138e6b3)

Buffered reader: Used for larger input and in multithreading
 
Scanner:

![image](https://github.com/user-attachments/assets/0d74ebd2-f3fb-4d7c-93fb-0bf0e8511e14)

JAVA OUTPUT:
Print(): print text
Println(): print text and then add new line
Format(): print formatted text in place of placeholders
Placeholders: %d for int, %c for char, %s for string, %f for float

 ![image](https://github.com/user-attachments/assets/e80010ac-04ca-4bb7-ab0e-3d08ccbab1b0)


For float, %5.2f means 5 dgitis and 2 decimals for float value

COMMAND line arguments can be used to build utility such as calculator, or csv file app, etc
Escape sequences: \t, \b, \n, \r, \f, \\, \”
Precedence: z=x=y is equal to x=y then z=x because of right side precedence
Short circuiting: in &&, || there is one case where condition is not checked

Bitwise operation:

  ![image](https://github.com/user-attachments/assets/f1cddabe-25a7-4ccb-9e25-69f57fd38c3f)

Left shift operation:
X<<1: 2 will be multiplied ‘1’ time to x
X<<4: 2 will be multiplied ‘4’ times to x

Right shift operation:
X>>3: x will be divided ‘3’ times by 2 and leading values will be filled with ones
x>>>3: x will be divided ‘3’ times by 2 and leading values will be zeroes instead of one


2.	Loops , functions, control statements

If else used to control conditions in below:

 ![image](https://github.com/user-attachments/assets/1a6c9d65-33f4-40e5-8aa4-44161d79ba01)


Switch: for multi branch case, use switch over ifelse for more readability.

 ![image](https://github.com/user-attachments/assets/7217ccb4-08e5-425f-8f36-107e9e46664d)


Without break, the control goes to each case and end at default.
We don’t need break at default.
Default runs when any of the above case is missed.

LEAP YEAR is a year which has 28 days in february and it comes once in 4 years. Example: 
Any of Below 2 rules must apply 

 ![image](https://github.com/user-attachments/assets/47b05529-8034-48a9-9668-143f83fcdcb8)


LOOPS Below are applications

![image](https://github.com/user-attachments/assets/acb85b8f-aaa6-47bf-844f-2df78cd7a7d5)
 

For LOOP
For(initialization;condition check; loop variable change)
For(  ;  ;  ) is an infinite loop
For(  ;true;) is also an infinite loop
For(;;;); print(n) this will print only once as ; will end for before print statement


Enhanced for Loop: It is used traversal of collections/objects
This loop can only read and can’t modify the elements
for (String x:array)
        {
            System.out.println(x);
        }


WHILE
While(condition){
Statement
}
While(true)  and while(condition);{statement} both are infinite loop statements

DO WHILE:   This will run statement at least once and then check the condition
Do{
statement
}while();


FOR VS WHILE
For is used for fixed structure
While is used for dynamic structure where condition changes with time

BREAK n CONTINUE:  Used with if statement in the loops
Break: It will stop the loop and goes to next statement after the loop
Continue: It will skip the iteration i.e., it skips all lines below continue statement within the loop and goes to next iteration


Methods:
A method is a collection of statements that perform some specific task 
All primitives are passed by values i.e., as a copy
All non-primitives are passed by references

 ![image](https://github.com/user-attachments/assets/d57d1989-daf4-4dd7-a66e-bad513b4db01)


Access Modifier
•	Modifier-: Defines the access type of the method i.e., from where it can be accessed in your application. In Java, there are 4 types of access specifiers:
o	public: accessible in all the classes in your application.
o	protected: accessible within the class in which it is defined and in its subclass(es)
o	private: accessible only within the class in which it is defined.
o	default (declared/defined without using any modifier): accessible within the same class and the package within which its class is defined.

![Uploading image.png…]()


Math.log10(1000) will return 3
Math.log10(100000) will return 5
Math.max(n1,n2) will return max value between n1 and n2




