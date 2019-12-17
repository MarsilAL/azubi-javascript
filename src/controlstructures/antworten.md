
- what control structures do you know?
- given a loop that prints number from 1 to 5. Implement this with a for loop and a while loop.
- What is a fall-through in context of a switch statement?


_____________________1_______________________________________________________________________________

JavaScript has number of statements that control flow of the program. There are:

conditionals (if-else, switch) that perform different actions depending on the value of an expression,
loops (while, do-while, for, for-in, for-of), that execute other statements repetitively,
jumps (break, continue, labeled statement) that cause a jump to another part of the program.

- - - - -  Conditionals * are control structures that perform different actions depending on the value of an expression.

* * * if-else: * * *

if (condition1) {
    statement1;
} else if (condition2) {
    statement2;
} else {
    statement3;
}


ex:
if (weight <= 60) { category = "light"; } else if (weight > 60 && weight <= 90) {
    category = "middle";
} else {
    category = "heavy";
}

* * * switch * * *
The switch statement is similar to the if-else statement. If all of the branches depend on the value of the same expression, the switch control structure can be used instead of the if-else.

switch (expression) {
    case value1:
        statement1;
        [break;]
    case value2:
        statement2;
        [break;]
    default:
        statement3;
}
When the switch statement is executed, the program attempts to match the value of expression to a case valel. If the value of expression is equal to a case value, the program executes the associated statements. If matching is not found, the program looks for the optional default clause. If it is found, associated statements are executed, if not the program skips all statements within the switch statement.


- - - - - Loops * are control structures that execute other statements repetitively.

* * * while * * *
The while loop repeats the execution of the statement as long as expression evaluates to true. It has the following syntax

while (expression)
    statement;

    ex:
    var counter = 0;
    while (counter &lt;= 5) {
    console.log(counter);
    counter++;
}

* * * do-while * * *
The do-while loop is similar to the while loop. The main difference is that first the statement is executed and then expression is checked.

do {
    statement;
} while (expression);

It means that statement is always executed at least once.

An example:
var counter = 5;
do {
    console.log(counter); // 5 is logged
} while (counter &lt;= 5);

Note that do-while loop must be terminated with a semicolon.

* * * for * * *

The for loop repeats as long as the condition is met. The syntax is as follows:

for (initialExpression; condition; incrementExpression)
    statement;

example:

for (var i = 0; i &lt;= 3; i++) {
    console.log(i);
}
// Output:
// 0
// 1
// 2
// 3
 






 _________________________________2____________________________________________________________
 - given a loop that prints number from 1 to 5. Implement this with a for loop and a while loop.

for (var i = 1; j= 5; i++) {
    console.log(i);
}

________________________________3_____________________________________________________________