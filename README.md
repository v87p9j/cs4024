java c
ITEC 2610 Object-Oriented Programming 
Section E, Fall 2024 
Assignment 2 
To submit: 
Prepare a single  .zip file containing all the source files (.java files, NOT .class files). Submit this file through Moodle.
/******************************************************************
Marking Template:
Style. (variable naming, indentation,  Layout)           /5
Comments                                                             /5
Proper use of listeners
(by inspection of source code)                               /15
Code Compiles?                                                     (yes/no)
Correct layout  (shape and fixed size)                      /6
Proper error handling(3 errors)                               /15
Successful execution of test cases (18)                   /54
Total   /100
According to this template the maximum mark you can get for code that does not compile is 25/100.
*******************************************************************/
Details 
Write a Java application which implements a four operation calculator, as shown below:

The calculator will work as follows:
1.   The scrollable text area will show each digit as entered.
2.   Decimal numbers are allowed, and you must ensure that only one decimal symbol is entered for each number (you decide what the behavior. of the calculator should be if the user breaks this rule, but it must be controlled by your program).
3.   When an operator (‘+’, ‘-‘, ‘/’, or ‘*’) is clicked, the operator should be displayed after the last digit entered, and subsequent numbers should be displayed on a new line.
4.   After entering a sequence of number-operator-number the user can click: a.   ‘=’, in which case the calculator must display:
i.   the ‘=’ symbol after the last digit of the second number  
ii.   the result of the operation, on a new line
iii.   anything else entered after the ‘=’ symbol is part of a new calculation, and must be displayed on a separate line
For example, the user clicks “123.45+456.2=1” . The screen should look like this:
123.45+            ← entered by user
456.2=              ← entered by user
579.65              ← calculated  displayed by your program
1                       ← beginning of a new calculation, entered by user
b.   any new operator, in which case the calculator must assume an implicit ‘=’ and:
i.   display an ‘=’ sign after the last number
ii.   display the result of the代 写ITEC 2610 Object-Oriented Programming Section E, Fall 2024 Assignment 2Java
代做程序编程语言 previous operation on a new line, followed by the second operator


iii.   treat the result as the first number of a new calculation, and display the new operator right after it
iv.   allow the user to enter a new number
For example, the user clicks “123.45+456.2/5=” . The most reasonable interpretation is that the user wants the first two
numbers added, and the sum divided by 5. The screen should look like this:
123.45+              ← entered by user
456.2=                ← 456.2 entered by user, ‘=’ added by the program
579.65/               ← 579.65 calculated by program, ‘/’ entered by user
5=                       ← new calculation, entered by user
115.93                ← calculated by your program
5.   When the user enters two or more consecutive operators, write an error message  in the text area stating that operator ‘x’ has been ignored. The message should be on a separate line, and everything else following should be on a new line.
6.   When the user clicks “Clear Last” the calculator should delete the last character displayed on the screen from the screen. Further behavior. of your calculator should reflect the deletion (for example “12+ClearLast-5” should execute a subtraction, not an addition; ). When clicked after ‘=’, Clear Last should have no effect. 
7.   When the user clicks “Clear All” the calculator should erase everything in the text area and start again with a new calculation.
Other requirements:
1.   The layout must match the image above.
2.   You must combine listeners where possible (hint: you don’t need a separate listener for every button).
3.   If you decide to issue error messages, they should be displayed in the text area.
4.   The window size should be fixed.
5.   Your application must protect against illegal operations (such as division by 0).
Please make sure you test at least the following scenarios, using both integer and decimal numbers:
1.   Each individual single operation (4 tests)
2.   Chained operations, both of the same kind (as in x+y+z) and different kinds (as in x+y-z/u) – 2 tests, plus 1 test with all 4 operators
3.   Every error condition (successive operators, division by 0, multiple decimal points) – 3 tests
4.   Behavior. of the clear buttons (8 tests), after
a.   digit entry 
b.   fisrt operator entry
c.   second operator entry triggering a calculation
d.   ‘=’ symbol







         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
