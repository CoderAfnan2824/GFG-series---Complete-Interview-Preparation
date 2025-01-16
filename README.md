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

Integer.parseInt(str) will convert string value into the int type.

4. Advanced
Biginteger is a class in java which stores large values. BigInteger class is present in java.math.* library.
Syntax:
BigInteger c=new BigInteger("5325");
Let's say 'a' is int type, then c=BigInteger.valueOf(a);

You can perform operation on BigInteger as below:
a.add(b);  a.subtract(b);  multiplay divide remainder
a.compareTo(b): will return 0,+1,-1 based on a and b values

BigInteger to other datatype conversion:
int a=A.intValue();
long b=B.longValue();
String s=S.toString();

a.isProbablePrime(1) will return check for prime bigInteger value. The '1' in bracket is certainity. 1 means 100% check if 'a' is prime or not
a.nextProbablePrime() will return next prime after 'a'

Methods of BigInteger
BigInteger abs​(): This method returns a BigInteger whose value is the absolute value of this BigInteger.
BigInteger gcd​(BigInteger val): This method returns a BigInteger whose value is the greatest common divisor of abs(this) and abs(val).
BigInteger max​(BigInteger val): This method returns the maximum of this BigInteger and val.
BigInteger min​(BigInteger val): This method returns the minimum of this BigInteger and val.
BigInteger mod​(BigInteger m): This method returns a BigInteger whose value is (this mod m).
BigInteger modPow​(BigInteger exponent, BigInteger m): This method returns a BigInteger whose value is (thisexponent mod m).
BigInteger negate​(): This method returns a BigInteger whose value is (-this).
BigInteger or​(BigInteger val): This method returns a BigInteger whose value is (this | val).
BigInteger pow​(int exponent): This method returns a BigInteger whose value is (thisexponent).
BigInteger shiftLeft​(int n): This method returns a BigInteger whose value is (this << n).
BigInteger shiftRight​(int n): This method returns a BigInteger whose value is (this >> n).
BigInteger sqrt​(): This method returns the integer square root of this BigInteger.

=======================================================================================================
PROGRAMMING - ADVANCED:

1. Lambda expression: It's a function without name and class. They are implemented using functional interface.
With lambda expression, you don't need to create a child class to implement that method, you can create directly.
Use curly braces for multi line statements.

2. Functional interface: It's an interface that contains exactly one abstract method and may contain other methods.

3. Stream: It's a pipeline of functions for which the input will be array, collections or stream of variables(even numbers, prime numbers,etc)
Stream has 3 parts: source, intermediaries and terminal
Lets say l is a list, implementing stream on 'l' is
l.stream
.filter(x->x%2==0)
.filter(x>10)
.foreach(system.out::println);

4.Method reference: Method references in Java 8 are a shorthand notation of a lambda expression to call a method. They provide an easy-to-read and concise way to refer to methods without executing them. Method reference can be implemented on both static n instance methods, even constructors

// Lambda expression
(args) -> ClassName.staticMethod(args)

// Method reference
ClassName::staticMethod

==========================================================CLASSES N OBJECTS====================================================================================
1. CLASS n OBJECTS:
Class is a blueprint/prototype from which real life entities(obj) are created.

Object has 3 parts: state(members), behavior(method) and Identity(unique name);

2. ENCAPSULATION: It is the hiding/restricting of data members/methods using access-modifiers.

Example: Suppose, you create a date class in which you declare a variable. Other teams use that class to get date. Now you want to modify layout of date, you can modify the variable. But if you had declared that variable as public, it's impossible as others might be using that variable. TO avoid, that kind of errors, we declared it as private.

3. ACCESS MODIFIERS: There are 4 types. Always try to use as strict as possible access modifier
private: Within the class( only methods of that class can access the members)
default: When you don't specify anything; is accessible only in the package(the folder which contains all classes n interfaces)
protected: Within the package and all the child classes of other packages
public: accessible everywhere 
A child class can modify access to less strict. But error occurs if more strictness is added.
Ex: if child class modify access to private from public, error occurs.

Encapsulation is defined as the wrapping up of data under a single unit. It's also called as data-hiding.


4. 'this' reference: It is a special reference in OOPs. It is used in classes to point to current object & it's members. You can call the constructor using this as this(0, 3);
example: p.setX(2).setY(3)
point setX(int x){
    this.x=x;
    return this;
  }

5. 'final' keyword: It's a state which can't modify it's behavior once it is assigned.
variable: can't be modified once assigned
method: can't be overridden(child class can't modify the method) 
class: A class can't have subclasses/ child classes
object: Final in objects prevent new reference after initialization
final String p=new String("Afnan");
p=new String("Adnan);  here we will get error as we are providing new reference

6. 'static': static members can be accessed without creating objects. They are shared among objects.
static methods cannot access non-static members. But non-static methods can access static members.
static methods cannot have access to 'this' reference.

7. constructor: It's method with class name and no return type. When we define one constructor, it's our responsibility to define all constructors.

8. Inheritance: This is a concept in which class can derive properties from base class.
super(): is used to call the constructor of base class. It's used to access parent member in derived class.
Object class: It's the root class in java from which all classes are inherited. clone(), equals(), hashcode(), toString() are few methods of object class.

Types of Inheritance:
single: B -> A
multilevel: c -> B -> A
Heirarchical: (B - C - D) -> A
Multiple inheritance: C -> (A - B) : not allowed in java. can be done using functional interface
Hybrid: D -> (B - C) -> A

9. Polymorphism: It's a concept of having many forms.
There are 2 types: compile/static and run/dynamic
a. static: sum(a, b), sum(a,b,c) sum(string s,string s2)
Method overloading takes place in above as same name method is used. only return type change does not cause method overloading. Automatic conversion takes place when method with exact datatype is not found.

b. dynamic: print() from base class is different to print() from derived class
Method overriding occurs at run time. An object is referred at run time. so method overriding helps in assigning appropriate method to each class objects.

static methods are not overridden.
Ex: static print() method is present in base n derived class. 
But base b=new derived, b.print() will be called from base class. overriding doesn't takes place.

A base class can refer to a derived class object, but reverse is not possible
base b=new derived();  -> correct
derived d=new base();  -> this is wrong

10. Abstraction: It's concept of later implementation of a method. You define method in abstract class or interface and implement in immediate derived classes. Data Abstraction is the property by virtue of which only the essential details are displayed to the user.
You can't create an object/instance of abstract class. But you can create reference of abstract class.

A class can be abstract without an abstract method. This is done to prevent object creation.
If a subclass doesn't implement abstract method, then the subclass must also be declared abstract.

11. Interface: 
All members are public static final. no other access modifier allowed except default n public.
Multiple inheritance allowed using interfaces; A class can implement multiple interfaces; An interface can extend multiple interfaces.
Interface base{}
Derived implements base{}


Difference between inheritance n abstract class:
Interfaces cannot have constructors.
All methods are public static final in interfaces.
Multiple inheritance allowed in interfaces.

Encapsulation is data hiding(information hiding) while Abstraction is detail hiding(implementation hiding).












