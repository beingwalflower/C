# C
C programs of different concepts,my text book and programming sites

My C notes from the net and my textbook. 
1.Difference between python and c?
2. Name and describe the four basic data types in programming?
3. Draw flowchart while and do-while loop with an example?
4. Explain different arithmetic operators with an example?
5. Explain the body section of c programming?

Introduction of C
HISTORY AND BASIC INTRODUCTION
C programming is a general-purpose, procedural, imperative computer programming language.
 C is the most widely used computer language.
 It keeps fluctuating at number one scale of popularity along with Java programming language, which is also equally popular and most widely used among modern software programmers.
C is a general-purpose programming language which features economy of expression, modern control flow and data structures, and a rich set of operators.
C is not a “very high level” language, nor a “big” one, and is not specialized to any particular area of application. BUt its restrictions and its generality make it more convenient and effective for many tasks than supposedly more powerful languages 
C was originally designed for and implemented on UNIX operating system on DEC PDP-11, by Dennis Ritchie. 
C provides a variety of data types. The fundamental types are characters, integers and floating-point numbers of several sizes. In addition, there is a hierarchy of derived data types created with pointers, arrays, structures and unions. 
Expressions are formed from operators and operands, any expression, including an assignment or function call, can be a statement.
Pointers provide for machine-independent address arithmetic
Why Learn C Programming?
C programming language is a MUST for students and working professionals to become a great Software Engineer especially when they are working in Software Development Domain. I will list down some of the key advantages of learning C Programming:
Easy to learn
Structured language
It produces efficient programs
It can handle low-level activities
It can be compiled on a variety of computer platforms
Facts about C
C was invented to write an operating system called UNIX.
C is a successor of B language which was introduced around the early 1970s.
The language was formalized in 1988 by the American National Standard Institute (ANSI).
The UNIX OS was totally written in C.
Today C is the most widely used and popular System Programming Language.
Most of the state-of-the-art software have been implemented using C.
Today's most popular Linux OS and RDBMS MySQL have been written in C.

Applications of C Programming
C was initially used for system development work, particularly the programs that make-up the operating system. C was adopted as a system development language because it produces code that runs nearly as fast as the code written in assembly language. Some examples of the use of C are -
Operating Systems
Language Compilers
Assemblers
Text Editors
Print Spoolers
Network Drivers
Modern Programs
Databases
Language Interpreters
Utilities
Features of C
C Compilers


An introduction to Flowcharts
What is a Flowchart?
A flowchart is a graphical representation of an algorithm. Programmers often use it as a program-planning tool to solve a problem. It makes use of symbols which are connected among them to indicate the flow of information and processing.
The process of drawing a flowchart for an algorithm is known as “flowcharting”.
Basic Symbols used in Flowchart Designs
Terminal: The oval symbol indicates Start, Stop and Halt in a program’s logic flow. A pause/halt is generally used in a program logic under some error conditions. The terminal is the first and last symbols in the flowchart.

Input/Output: A parallelogram denotes any function of input/output type. Program instructions that take input from input devices and display output on output devices are indicated with parallelogram in a flowchart.

Processing: A box represents arithmetic instructions. All arithmetic processes such as adding, subtracting, multiplication and division are indicated by action or process symbol.

Decision diamond symbol represents a decision point. Decision-based operations such as yes/no question or true/false are indicated by diamond in the flowchart.

Connectors: Whenever the flowchart becomes complex or it spreads over more than one page, it is useful to use connectors to avoid any confusions. It is represented by a circle.

Flow lines: Flow lines indicate the exact sequence in which instructions are executed. Arrows represent the direction of flow of control and relationship among different symbols of the flowchart.

Connectors: when flowcharts become very complex and spread across more than one page, then connectors  are used to connect two flowcharts with each other 
 
Example: Draw a flowchart to input two numbers from the user and display the largest of two numbers






Following is the basic structure of a C program.
Documentation
Consists of comments, some description of the program, programmer name and any other useful points that can be referenced later.




Link
Provides instruction to the compiler to link function from the library function.




Definition
Consists of symbolic constants.




Global declaration
Consists of function declaration and global variables.




main( )
{

}


Every C program must have a main() function which is the starting point of the program execution.




Subprograms
User-defined functions.

Let’s explore the sections with an example.
Write a program to print the area of a circle.
In the following example, we will find the area of a circle for a given radius 10cm.
Formula
The formula to compute the area of a circle is πr2 where π is PI = 3.1416 (approx.) and r is the radius of the circle.
Let’s write the C code to compute the area of the circle.
/**
 * file: circle.c
 * author: yusuf shakeel
 * date: 2010-11-25
 * description: a program to find the area of a circle
 *              using the radius r
 */
#include <stdio.h>
#define PI 3.1416
float area(float r);
int main(void)
{
  float r = 10;
  printf("Area: %.2f", area(r));
  return 0;
}
float area(float r) {
    return PI * r * r;
}
The above code will give the following output.
Area: 314.16
Different sections of the above code
Documentation
This section contains a multi-line comment describing the code.
/**
 * file: circle.c
 * author: yusuf shakeel
 * date: 2010-11-25
 * description: a program to find the area of a circle
 *              using the radius r
 */
In C, we can create single line comment using two forward slashes// and we can create multi-line comment using /* */.
Comments are ignored by the compiler and are used to write notes and document code.
Link
This section includes header file.
#include <stdio.h>
We are including the stdio.h input/output header file from the C library.
Definition
This section contains constant.
#define PI 3.1416
In the above code, we have created a constant PI and assigned 3.1416 to it.
The #define is a preprocessor compiler directive which is used to create constants. We generally use uppercase letters to create constants.
Global declaration
This section contains a function declaration.
float area(float r);
We have declared an area function which takes a floating number (i.e., number with decimal parts) as an argument and returns floating number.
main( ) function
This section contains the main() function.
int main(void)
{
  float r = 10;
  printf("Area: %.2f", area(r));
  return 0;
}
This is the main() function of the code. Inside this function, we have created a floating variable r and assigned 10 to it.
Then we have called the printf() function. The first argument contains "Area: %.2f" which means we will print floating number having only 2 decimal places. In the second argument, we are calling the area() function and passing the value of r to it.
Subprograms
This section contains a subprogram, an area() function that is called from the main() function.
float area(float r) {
    return PI * r * r;
}
This is the definition of the area() function. It receives the value of radius in variable r and then returns the area of the circle using the following formula PI * r * r
 
C/C++ Header File
Let’s have a look at these Header files in C and C++:.A header file is a file with extension .h which contains C function declarations and macro definitions to be shared between several source files. There are two types of header files: the files that the programmer writes and the files that come with your compiler.
Your request to use a header file in your program by including it with the C preprocessing directive #include like you have seen the inclusion of stdio.h header file, which comes along with your compiler.
Including a header file is equal to copying the content of the header file but we do not do it because it will be error-prone and it is not a good idea to copy the content of a header file in the source files, especially if we have multiple source files in a program.
A simple practice in C or C++ programs is that we keep all the constants, macros, system-wide global variables, and function prototypes in the header files and include that header file wherever it is required.
Include Syntax
Both the user and the system header files are included using the preprocessing directive #include. It has the following two forms −
#include <file>
 
This form is used for system header files. It searches for a file named 'file' in a standard list of system directories. You can prepend directories to this list with the -I option while compiling your source code.
#include "file"
 
This form is used for header files of your own program. It searches for a file named 'file' in the directory containing the current file. You can prepend directories to this list with the -I option while compiling your source code.
 
1. #include<stdio.h>  (Standard input-output header)
Used to perform input and output operations in C like scanf() and printf().
2. #include<string.h> (String header)
Perform string manipulation operations like strlen and strcpy.
3. #include<conio.h> (Console input-output header)
Perform console input and console output operations like clrscr() to clear the screen and getch() to get the character from the keyboard.
4. #include<stdlib.h> (Standard library header)
Perform standard utility functions like dynamic memory allocation, using functions such as malloc() and calloc().
5. #include<math.h> (Math header )
Perform mathematical operations like sqrt() and pow(). To obtain the square root and the power of a number respectively.
6. #include<ctype.h>(Character type header)
Perform character type functions like isaplha() and isdigit(). To find whether the given character is an alphabet or a digit respectively.
7. #include<time.h>(Time header)
Perform functions related to date and time like setdate() and getdate(). To modify the system date and get the CPU time respectively.
8. #include<assert.h> (Assertion header)
It is used in program assertion functions like assert(). To get an integer data type in C/C++ as a parameter which prints stderr only if the parameter passed is 0.
9. #include<locale.h> (Localization header)
Perform localization functions like setlocale() and localeconv(). To set locale and get locale conventions respectively.
10. #include<signal.h> (Signal header)
Perform signal handling functions like signal() and raise(). To install a signal handler and to raise the signal in the program respectively
11. #include<setjmp.h> (Jump header)
Perform jump functions.
12. #include<stdarg.h> (Standard argument header)
Perform standard argument functions like va_start and va_arg(). To indicate the start of the variable-length argument list and to fetch the arguments from the variable-length argument list in the program respectively.
13. #include<errno.h> (Error handling header)
Used to perform error handling operations like errno(). To indicate errors in the program by initially assigning the value of this function to 0 and then later changing it to indicate errors.
 
An operator is a symbol that tells the compiler to perform specific mathematical or logical functions. C language is rich in built-in operators and provides the following types of operators −
Arithmetic Operators
Relational Operators
Logical Operators
Bitwise Operators
Assignment Operators
Misc Operators
We will, in this chapter, look into the way each operator works.
Arithmetic Operators
The following table shows all the arithmetic operators supported by the C language. Assume variable A holds 10 and variable B holds 20 then −
Show Examples
Operator
Description
Example
+
Adds two operands.
A + B = 30
−
Subtracts second operand from the first.
A − B = -10
*
Multiplies both operands.
A * B = 200
/
Divides numerator by de-numerator.
B / A = 2
%
Modulus Operator and remainder of after an integer division.
B % A = 0
++
Increment operator increases the integer value by one.
A++ = 11
--
Decrement operator decreases the integer value by one.
A-- = 9
Relational Operators
The following table shows all the relational operators supported by C. Assume variable A holds 10 and variable B holds 20 then −
Show Examples
Operator
Description
Example
==
Checks if the values of two operands are equal or not. If yes, then the condition becomes true.
(A == B) is not true.
!=
Checks if the values of two operands are equal or not. If the values are not equal, then the condition becomes true.
(A != B) is true.
>
Checks if the value of the left operand is greater than the value of the right operand. If yes, then the condition becomes true.
(A > B) is not true.
<
Checks if the value of the left operand is less than the value of the right operand. If yes, then the condition becomes true.
(A < B) is true.
>=
Checks if the value of the left operand is greater than or equal to the value of the right operand. If yes, then the condition becomes true.
(A >= B) is not true.
<=
Checks if the value of the left operand is less than or equal to the value of the right operand. If yes, then the condition becomes true.
(A <= B) is true.
Logical Operators
Following table shows all the logical operators supported by C language. Assume variable A holds 1 and variable B holds 0, then −
Show Examples
Operator
Description
Example
&&
Called Logical AND operator. If both the operands are non-zero, then the condition becomes true.
(A && B) is false.
||
Called Logical OR Operator. If any of the two operands are non-zero, then the condition becomes true.
(A || B) is true.
!
Called Logical NOT Operator. It is used to reverse the logical state of its operand. If a condition is true, then Logical NOT operator will make it false.
!(A && B) is true.
Bitwise Operators
Bitwise operator works on bits and performs the bit-by-bit operation. The truth tables for &, |, and ^ is as follows −
p
q
p & q
p | q
p ^ q
0
0
0
0
0
0
1
0
1
1
1
1
1
1
0
1
0
0
1
1
Assume A = 60 and B = 13 in binary format, they will be as follows −
A = 0011 1100
B = 0000 1101
-----------------
A&B = 0000 1100
A|B = 0011 1101
A^B = 0011 0001
~A = 1100 0011
The following table lists the Bitwise operators supported by C. Assume variable 'A' holds 60 and variable 'B' holds 13, then −
Show Examples
Operator
Description
Example
&
Binary AND Operator copies a bit to the result if it exists in both operands.
(A & B) = 12, i.e., 0000 1100
|
Binary OR Operator copies a bit if it exists in either operand.
(A | B) = 61, i.e., 0011 1101
^
Binary XOR Operator copies the bit if it is set in one operand but not both.
(A ^ B) = 49, i.e., 0011 0001
~
Binary Ones Complement Operator is unary and has the effect of 'flipping' bits.
(~A ) = ~(60), i.e,. -0111101
<<
Binary Left Shift Operator. The left operands value is moved left by the number of bits specified by the right operand.
A << 2 = 240 i.e., 1111 0000
>>
Binary Right Shift Operator. The left operands value is moved right by the number of bits specified by the right operand.
A >> 2 = 15 i.e., 0000 1111
Assignment Operators
The following table lists the assignment operators supported by the C language −
Show Examples
Operator
Description
Example
=
Simple assignment operator. Assigns values from right side operands to left side operand
C = A + B will assign the value of A + B to C
+=
Add AND assignment operator. It adds the right operand to the left operand and assigns the result to the left operand.
C += A is equivalent to C = C + A
-=
Subtract AND assignment operator. It subtracts the right operand from the left operand and assigns the result to the left operand.
C -= A is equivalent to C = C - A
*=
Multiply AND assignment operator. It multiplies the right operand with the left operand and assigns the result to the left operand.
C *= A is equivalent to C = C * A
/=
Divide AND assignment operator. It divides the left operand with the right operand and assigns the result to the left operand.
C /= A is equivalent to C = C / A
%=
Modulus AND assignment operator. It takes modulus using two operands and assigns the result to the left operand.
C %= A is equivalent to C = C % A
<<=
Left shift AND assignment operator.
C <<= 2 is same as C = C << 2
>>=
Right shift AND assignment operator.
C >>= 2 is same as C = C >> 2
&=
Bitwise AND assignment operator.
C &= 2 is same as C = C & 2
^=
Bitwise exclusive OR and assignment operator.
C ^= 2 is same as C = C ^ 2
|=
Bitwise inclusive OR and assignment operator.
C |= 2 is same as C = C | 2
Misc Operators ↦ size & ternary
Besides the operators discussed above, there are a few other important operators including size and? : supported by the C Language.
Show Examples
Operator
Description
Example
sizeof()
Returns the size of a variable.
sizeof(a), where a is an integer, will return 4.
&
Returns the address of a variable.
&a; returns the actual address of the variable.
*
Pointer to a variable.
*a;
? :
Conditional Expression.
If Condition is true? then value X: Otherwise value Y
Operators Precedence in C
Operator precedence determines the grouping of terms in an expression and decides how an expression is evaluated. Certain operators have higher precedence than others; for example, the multiplication operator has higher precedence than the addition operator.
For example, x = 7 + 3 * 2; here, x is assigned 13, not 20 because operator * has higher precedence than +, so it first gets multiplied with 3*2 and then adds into 7.
Here, operators with the highest precedence appear at the top of the table, those with the lowest appear at the bottom. Within an expression, higher precedence operators will be evaluated first.
Show Examples
Category
Operator
Associativity
Postfix
() [] -> . ++ - -
Left to right
Unary
+ - ! ~ ++ - - (type)* & sizeof
Right to left
Multiplicative
* / %
Left to right
Additive
+ -
Left to right
Shift
<< >>
Left to right
Relational
< <= > >=
Left to right
Equality
== !=
Left to right
Bitwise AND
&
Left to right
Bitwise XOR
^
Left to right
Bitwise OR
|
Left to right
Logical AND
&&
Left to right
Logical OR
||
Left to right
Conditional
?:
Right to left
Assignment
= += -= *= /= %=>>= <<= &= ^= |=
Right to left
Comma
,
Left to right
 
In programming, loops are used to repeat a block of code until a specified condition is met.
C programming has three types of loops:
for loop
while loop
do...while loop
We will learn about for loop in this tutorial. In the next tutorial, we will learn about while and do...while loop.

for Loop
The syntax of the for loop is:
for (initializationStatement; testExpression; updateStatement)
{
   // statements inside the body of the loop
}

How for loop works?
The initialization statement is executed only once.
Then, the test expression is evaluated. If the test expression is evaluated to false, the for loop is terminated.
However, if the test expression is evaluated to true, statements inside the body of for loop are executed, and the update expression is updated.
Again the test expression is evaluated.
This process goes on until the test expression is false. When the test expression is false, the loop terminates.
To learn more about test expression (when the test expression is evaluated to true and false), check out relational and logical operators.

for loop Flowchart


Example 1: for loop
// Print numbers from 1 to 10
#include <stdio.h>
 
int main() {
 int i;
 
 for (i = 1; i < 11; ++i)
 {
   printf("%d ", i);
 }
 return 0;
}
while loop
The syntax of the while loop is:
while (testExpression)
{
   // statements inside the body of the loop
}

How while loop works?
The while loop evaluates the test expression inside the parenthesis ().
If the test expression is true, statements inside the body of while loop are executed. Then, the test expression is evaluated again.
The process goes on until the test expression is evaluated to false.
If the test expression is false, the loop terminates (ends).
To learn more about test expression (when the test expression is evaluated to true and false), check out relational and logical operators.

Flowchart of while loop


Example 1: while loop
// Print numbers from 1 to 5
 
#include <stdio.h>
int main()
{
   int i = 1;
  
   while (i <= 5)
   {
       printf("%d\n", i);
       ++i;
   }
 
   return 0;
}
Output
1
2
3
4
5

Here, we have initialized i to 1.
When i is 1, the test expression i <= 5 is true. Hence, the body of the while loop is executed. This prints 1 on the screen and the value of i is increased to 2.
Now, i is 2, the test expression i <= 5 is again true. The body of the while loop is executed again. This prints 2 on the screen and the value of i is increased to 3.
This process goes on until i becomes 6. When i is 6, the test expression i <= 5 will be false and the loop terminates.

do...while loop
The do..while loop is similar to the while loop with one important difference. The body of do...while loop is executed at least once. Only then, the test expression is evaluated.
The syntax of the do...while loop is:
do
{
  // statements inside the body of the loop
}
while (test expression);

How do...while loop works?
The body of do...while loop is executed once. Only then, the test expression is evaluated.
If the test expression is true, the body of the loop is executed again and the test expression is evaluated.
This process goes on until the test expression becomes false.
If the test expression is false, the loop ends.

Flowchart of do...while Loop


Example 2: do...while loop
// Program to add numbers until the user enters zero
 
#include <stdio.h>
int main()
{
   double number, sum = 0;
 
   // the body of the loop is executed at least once
   do
   {
       printf("Enter a number: ");
       scanf("%lf", &number);
       sum += number;
   }
   while(number != 0.0);
 
   printf("Sum = %.2lf",sum);
 
   return 0;
}
Output
Enter a number: 1.5
Enter a number: 2.4
Enter a number: -3.4
Enter a number: 4.2
Enter a number: 0
Sum = 4.70

Output
1 2 3 4 5 6 7 8 9 10
i is initialized to 1.
The test expression i < 11 is evaluated. Since 1 less than 11 is true, the body of for loop is executed. This will print the 1 (value of i) on the screen.
The update statement ++i is executed. Now, the value of I will be 2. Again, the test expression is evaluated to true, and the body of for loop is executed. This will print 2 (value of i) on the screen.
Again, the update statement ++i is executed and the test expression i < 11 is evaluated. This process goes on until i becomes 11.
When i becomes 11, i < 11 will be false, and the for loop terminates.
Arrays a kind of data structure that can store a fixed-size sequential collection of elements of the same type. An array is used to store a collection of data, but it is often more useful to think of an array as a collection of variables of the same type.
Instead of declaring individual variables, such as number0, number1, ..., and number99, you declare one array variable such as numbers and use numbers[0], numbers[1], and ..., numbers[99] to represent individual variables. A specific element in an array is accessed by an index.
All arrays consist of contiguous memory locations. The lowest address corresponds to the first element and the highest address to the last element.

Declaring Arrays
To declare an array in C, a programmer specifies the type of the elements and the number of elements required by an array as follows −
type arrayName [ arraySize ];

This is called a single-dimensional array. The arraySize must be an integer constant greater than zero and type can be any valid C data type. For example, to declare a 10-element array called balance of type double, use this statement −
double balance[10];

Here balance is a variable array which is sufficient to hold up to 10 double numbers.
Initializing Arrays
You can initialize an array in C either one by one or using a single statement as follows −
double balance[5] = {1000.0, 2.0, 3.4, 7.0, 50.0};

The number of values between braces { } cannot be larger than the number of elements that we declare for the array between square brackets [ ].
If you omit the size of the array, an array just big enough to hold the initialization is created. Therefore, if you write −
double balance[] = {1000.0, 2.0, 3.4, 7.0, 50.0};

You will create exactly the same array as you did in the previous example. Following is an example to assign a single element of the array −
balance[4] = 50.0;

The above statement assigns the 5th element in the array with a value of 50.0. All arrays have 0 as the index of their first element which is also called the base index and the last index of an array will be total size of the array minus 1. Shown below is the pictorial representation of the array we discussed above −

Accessing Array Elements
An element is accessed by indexing the array name. This is done by placing the index of the element within square brackets after the name of the array. For example −
double salary = balance[9];

The above statement will take the 10th element from the array and assign the value to salary variable. The following example Shows how to use all the three above mentioned concepts viz. declaration, assignment, and accessing arrays −
Live Demo
#include <stdio.h>
 
int main () {

   int n[ 10 ]; /* n is an array of 10 integers */
   int i,j;
 
   /* initialize elements of array n to 0 */         
   for ( i = 0; i < 10; i++ ) {
      n[ i ] = i + 100; /* set element at location i to i + 100 */
   }
   
   /* output each array element's value */
   for (j = 0; j < 10; j++ ) {
      printf("Element[%d] = %d\n", j, n[j] );
   }
 
   return 0;
}
When the above code is compiled and executed, it produces the following result −
Element[0] = 100
Element[1] = 101
Element[2] = 102
Element[3] = 103
Element[4] = 104
Element[5] = 105
Element[6] = 106
Element[7] = 107
Element[8] = 108
Element[9] = 109

Arrays in Detail
Arrays are important to C and should need a lot more attention. The following important concepts related to array should be clear to a C programmer −
Sr.No.
Concept & Description
1
Multi-dimensional arrays
C supports multidimensional arrays. The simplest form of the multidimensional array is the two-dimensional array.
2
Passing arrays to functions
You can pass to the function a pointer to an array by specifying the array's name without an index.
3
Return array from a function
C allows a function to return an array.
4
Pointer to an array
You can generate a pointer to the first element of an array by simply specifying the array name, without any index

