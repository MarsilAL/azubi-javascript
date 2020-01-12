•	Datatypes
A- what datatypes do exist in the programming language JavaScript? List them!
1- String 2- Number 3- Boolean 4- Null 5- Undefined 6- Symbol 7- BigInt 8- Object 9- Function
________________________________________
1- String:
In JavaScript, there are 3 types of quotes.
Double quotes: "Hello". Single quotes: 'Hello'. Backticks: Hello. Double and single quotes are “simple” quotes. There’s practically no difference between them in JavaScript.
Backticks are “extended functionality” quotes. They allow us to embed variables and expres-sions into a string by wrapping them in ${…}
2- Numbers:
The number type represents both integer and floating point numbers.
There are many operations for numbers, e.g. multiplication *, division /, addition +, subtraction -, and so on.
Besides regular numbers, there are so-called “special numeric values” which also belong to this data type: Infinity, -Infinity and NaN.
3- Boolean:
The boolean type has only two values: true and false.
4- Null:
It’s just a special value which represents “nothing”, “empty” or “value unknown”.
5- Undefined:
The meaning of undefined is “value is not assigned”. declared, but not assigned.
6- Symbol:
!!! A Symbol is a unique and immutable primitive value and may be used as the key of an Ob-ject property. !!!
7- BigInt: for really big numbers for integer values larger than 2(53) or less than -2(53)
8- Object:
All other types are called “primitive” because their values can contain only a single thing (be it a string or a number or whatever). In contrast, objects are used to store collections of data and more complex entities.

B- what does coersion mean? Give me an example!
Type coercion is the process of converting value from one type to another
(such as string to number, object to boolean, and so on)

•	Control structures
•	what control structures do you know?
•	given a loop that prints number from 1 to 5. Implement this with a for loop and a while loop.
•	What is a fall-through in context of a switch statement?
1__________________________________________________________
JavaScript has number of statements that control flow of the program. There are:
conditionals (if-else, switch) that perform different actions depending on the value of an expression, loops (while, do-while, for, for-in, for-of), that execute other state-ments repetitively, jumps (break, continue, labeled statement) that cause a jump to another part of the program.
•	
o	
	
	
	Conditionals * are control structures that perform different actions depending on the value of an ex-pression.
•	
o	
	if-else: * * *
if (condition1) { statement1; } else if (condition2) { statement2; } else { statement3; }
ex: if (weight <= 60) { category = "light"; } else if (weight > 60 && weight <= 90) { category = "middle"; } else { category = "heavy"; }
•	
o	
	switch * * * The switch statement is similar to the if-else state-ment. If all of the branches depend on the value of the same ex-pression, the switch control structure can be used instead of the if-else.
switch (expression) { case value1: statement1; [break;] case value2: statement2; [break;] default: statement3; } When the switch statement is executed, the program attempts to match the value of expression to a case valel. If the value of expression is equal to a case value, the program executes the associated statements. If matching is not found, the program looks for the optional default clause. If it is found, associated statements are executed, if not the program skips all statements within the switch statement.
•	
o	
	
	
	Loops * are control structures that execute other statements repetitively.
•	
o	
	while * * * The while loop repeats the execution of the statement as long as expression evaluates to true. It has the following syn-tax
while (expression) statement;
ex:
var counter = 0;
while (counter &lt;= 5) {
console.log(counter);
counter++;
}
•	
o	
	do-while * * * The do-while loop is similar to the while loop. The main difference is that first the statement is executed and then expression is checked.
do { statement; } while (expression);
It means that statement is always executed at least once.
An example: var counter = 5; do { console.log(counter); // 5 is logged } while (counter <= 5);
Note that do-while loop must be terminated with a semicolon.
•	
o	
	for * * *
The for loop repeats as long as the condition is met. The syntax is as follows:
for (initialExpression; condition; incrementExpression) statement;
example:
for (var i = 0; i <= 3; i++) { console.log(i); } // Output: // 0 // 1 // 2 // 3
2___________________________
•	given a loop that prints number from 1 to 5. Implement this with a for loop and a while loop.
Ex: while loop :
var x = 1
while (x <= 5) {
    console.log(x);
    x = x + 1
}
Ex: for loop :
for (var i = 1; i = 5; i++) {
    console.log(i);
}

3_____________________________
The switch statement evaluates an expression, matching the expression's value to a case clause, and executes statements associated with that case, as well as statements in cases that follow the matching case.



•	Arrays
1.	what operations would you do with a list of elements? List them!

2.	why do you think is this true typeof [] == "object"?  Ja
What makes an object an object in classical programming?
an object instantiates a class.

•	¬¬¬¬¬¬¬¬¬¬¬¬¬ Objects
1.	write a function in three different programming languages that returns the sum of two numbers, which have been given to the function as an argument.
JAVA:
    public class TwoNum{
        public static void main(String[] args) {
            int first = 10;
            int second = 20;
            int sum = first + second;
            System.out.println("The sum is: " + sum);
        }
    }
Python
num1 = 1.5
num2 = 6.3
sum = float(num1) + float(num2)
print('The sum of {0} and {1} is {2}'.format(num1, num2, sum))

C#
  public class functionsum
    {
        public static int Sum(int num1, int num2)
        {
            int total;
            total = num1 + num2;
            return total;
        }
     
        public static void Main()
        {        
            Console.Write("Enter two numbers: ");
            int number1 = 3;
            int number2 = 5;
            Console.WriteLine("\nThe sum of two numbers is : {0} \n", Sum(number1, number2));
     
            Console.ReadLine();
        }
    }
2.	explain variable shadowing
shadowing: declared two different values for a same variable.
Var a=5;
Console.log(“Variable value at global scope:”,a);
    Function func(){
Var a=50;
Console.log(“Variable value at local scope:”,a);
}
	In the above code, we’ve declared two different values for a same variable “a”. Since, variable “a” was declared with a new value inside Func(), system will fetch that value for any operations performed inside that particular scope irrespective of global value.

•	Scope
1.	What is the difference between declaration and definition?
declaration is giving a prototype like simply a name . definition is associating the task or the meaning with the prototype.

How does this relate to the concept of 'hoisting'. Explain!
Hoisting is JavaScript's default behavior of moving declarations to the top.
a variable can be declared after it has been used.

What is hoisting
Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution.
What scopes does javascript use?
Global scope
Local scope

•	Prototypes
	What types of languages do you know. Try to find 3 groups. Procedural Programming Language. ... Functional Programming Language. ... Object-oriented Programming Language. ... Scripting Pro-gramming Language. ... Logic Programming Langu-age. ...
•	What are the main concepts of an object-oriented programming language?
Objects Classes Data abstraction Data Encapsulation Inheritance Polymorphism Over-loading
•	every property of an js-object has to be stored in memory. Open your favorite browser and try to analyse the memory footprint of a website.

