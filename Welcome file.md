---


---

<h1 id="unit-iii-control-flow-functions">UNIT III CONTROL FLOW, FUNCTIONS</h1>
<p><strong>Conditionals: Boolean values and operators, conditional (if), alternative (if-else), chained conditional (if-elif-else); Iteration: state, while, for, break, continue, pass; Fruitful functions: return values, parameters, local and global scope, function composition, recursion; Strings: string slices, immutability, string functions and methods, string module; Lists as arrays. Illustrative programs: square root, gcd, exponentiation, sum an array of numbers, linear search, binary search</strong></p>
<h2 id="key-terms">KEY TERMS</h2>
<h4 id="operators">Operators</h4>
<p><em>Operators</em> are the constructs which can manipulate the value of operands.</p>
<h4 id="control-flow-statements"><strong>Control flow statements:</strong></h4>
<p><em>Control statements</em> in python are used to control the order of execution of the program based on the values and logic.</p>
<h4 id="repetition-statements"><strong>Repetition Statements</strong></h4>
<p><em>Repetition statements</em> are called loops, and are used to repeat the same code multiple times in succession.</p>
<h4 id="functions">Functions</h4>
<p>A <em>function</em> is a block of code which only runs when it is called.</p>
<h4 id="fruitful-functions">Fruitful functions</h4>
<p>The <em>functions</em> which return any value are called as <em>fruitful functions</em>.</p>
<h4 id="strings">Strings</h4>
<p><em>Strings</em> are arrays of bytes representing Unicode characters.</p>
<h2 id="conditionals">3.1. CONDITIONALS:</h2>
<h3 id="boolean-values-and-operators">3.1.1 BOOLEAN VALUES AND OPERATORS:</h3>
<ul>
<li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" disabled=""> A Boolean expression is an expression that is either true or  false.</li>
<li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" disabled=""> Converting Boolean to integer, the value is always 0 for false and 1 for  true</li>
<li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" disabled=""> Converting integer to Boolean, the value is True for all integers except  zero</li>
<li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" disabled=""> Python type is <strong>bool</strong>.</li>
</ul>

<table>
<thead>
<tr>
<th>Boolean Expression</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td>x != y</td>
<td>x is not equal to y</td>
</tr>
<tr>
<td>x &gt; y</td>
<td>x greater than y</td>
</tr>
<tr>
<td>x&lt;y</td>
<td>x less than y</td>
</tr>
<tr>
<td>x&lt;=y</td>
<td>x less than or equal to</td>
</tr>
<tr>
<td>x&gt;=y</td>
<td>x greater than or equal to</td>
</tr>
</tbody>
</table><h3 id="boolean-and-logical-operators">Boolean and Logical operators</h3>
<h3 id="and-operator">1. <em>and</em> Operator:</h3>

<table>
<thead>
<tr>
<th>Op1</th>
<th>Op2</th>
<th>Op1 and Op2</th>
</tr>
</thead>
<tbody>
<tr>
<td>TRUE</td>
<td>TRUE</td>
<td>TRUE</td>
</tr>
<tr>
<td>TRUE</td>
<td>FALSE</td>
<td>FALSE</td>
</tr>
<tr>
<td>FALSE</td>
<td>TRUE</td>
<td>FALSE</td>
</tr>
<tr>
<td>FALSE</td>
<td>FALSE</td>
<td>FALSE</td>
</tr>
</tbody>
</table><h3 id="or-operator">1. <em>or</em> Operator:</h3>

<table>
<thead>
<tr>
<th>Op1</th>
<th>Op2</th>
<th>Op1 or Op2</th>
</tr>
</thead>
<tbody>
<tr>
<td>TRUE</td>
<td>TRUE</td>
<td>TRUE</td>
</tr>
<tr>
<td>TRUE</td>
<td>FALSE</td>
<td>TRUE</td>
</tr>
<tr>
<td>FALSE</td>
<td>TRUE</td>
<td>TRUE</td>
</tr>
<tr>
<td>FALSE</td>
<td>FALSE</td>
<td>FALSE</td>
</tr>
</tbody>
</table><h3 id="example-1-“and”-operator">Example 1: “and” operator</h3>
<pre><code>   A python program to display the National holidays.
   For example:
       January 26-Republic day
       August 15-Indepependance day 
       October 2-Gandhi Jayanthi*
   If user input is other than the given condition,Error will be displayed as “Invalid input”.

		    print("Enter Month and Day")
			month=input()
			day=int(input())
			if(month =="january" and day ==26):
				print ("republic day")
			elif(month =="august" and day ==15):
				print ("independence day")
			elif(month =="october" and day ==2):
				print ("Gandhi Jayanthi")
			else:
				print ("invalid input")
</code></pre>
<h3 id="example-1-“or”-operator">Example 1: “or” operator</h3>
<pre><code>Number of days in a month varies from 30 to 31 days. 
Write a python program to read the name of the month and display corresponding days. 
If he input is other than the given month, then display error message as “Invalid”.

    import sys
	month=input()
	if(month=="may" or month=="july" or month=="august"):
		 print ("31")
	elif(month=="jun"):
		 print ("30")
	else:
		 print ("invalid")`
</code></pre>
<h3 id="operators-1">3.1.2. OPERATORS</h3>
<ul>
<li>
<p>Each built-in data types come with its set of operators.</p>
</li>
<li>
<p>Operators are the constructs which can manipulate the value of  operands.</p>
</li>
<li>
<p>They are generally classified into binary and unary operators based on the number of arguments.</p>
</li>
<li>
<p>Binary operators require two operands</p>
</li>
<li>
<p>Python language supports the following types of  operators.</p>
<ol>
<li>Arithmetic  Operators</li>
<li>Comparison (Relational) Operators</li>
<li>Assignment  Operators</li>
<li>Logical  Operators</li>
<li>Membership  Operators</li>
<li>Identity  Operators</li>
</ol>
</li>
</ul>
<h3 id="i-arithmetic-operators">i) Arithmetic operators</h3>
<ul>
<li>Arithmetic  operators  are  used  to  perform  mathematical  operations  like  addition,  subtraction,  Multiplication</li>
<li>Assume variable ‘<em>a’</em> holds 10 and variable ‘<em>b</em>’ holds 20  then the following table shows the result of arithmetic operators.</li>
</ul>

<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td>+ Addition</td>
<td>Adds values on either side of the operator.</td>
<td>a + b = 30</td>
</tr>
<tr>
<td>-Subtraction</td>
<td>Subtracts right hand operand from left hand operand.</td>
<td>a – b = -10</td>
</tr>
<tr>
<td>* Multiplication</td>
<td>Multiplies values on either side of the operator</td>
<td>a * b = 200</td>
</tr>
<tr>
<td>/ Division</td>
<td>Divides left hand operand by right hand operand</td>
<td>b / a = 2</td>
</tr>
<tr>
<td>% Modulus</td>
<td>Divides left hand operand by right hand operand and returns remainder</td>
<td>b % a = 0</td>
</tr>
<tr>
<td>** Exponent</td>
<td>Performs exponential (power) calculation on operators</td>
<td>a**b =10 to the power 20</td>
</tr>
<tr>
<td>// Floor Division</td>
<td>The division of operands where the result is the quotient in which the digits after the decimal point are removed. But if one of the operands is negative, the result is floored, i.e., rounded away from zero (towards negative infinity) −</td>
<td>9//2 = 4 and 9.0//2.0 = 4.0, -11//3 = -4, -11.0//3 = -4.0</td>
</tr>
</tbody>
</table><h3 id="ii-comparison-operators">(ii)	Comparison Operators</h3>
<p>•	These operators compare the values on either sides of them and decide the relation among them. They are also called Relational operators.<br>
•	The result of these operators is a Boolean value (True / False)<br>
•	Assume variable a holds 10 and variable b holds 20, then</p>

<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td>== Equal</td>
<td>If the values of two operands are equal, then the condition becomes true.</td>
<td>(a == b) is not true.</td>
</tr>
<tr>
<td>!= Not Equal</td>
<td>If values of two operands are not equal, then condition becomes true.</td>
<td>(a != b) is true.</td>
</tr>
<tr>
<td>&gt; Greater than</td>
<td>If the value of left operand is greater than the value of right operand, then condition becomes true.</td>
<td>(a &gt; b) is not true.</td>
</tr>
<tr>
<td>&lt;</td>
<td>If the value of left operand is less than the value of right operand, then condition becomes true.</td>
<td>(a &lt; b) is true.</td>
</tr>
<tr>
<td>&gt;=</td>
<td>If the value of left operand is greater than or equal to the value of right operand, then condition becomes true.</td>
<td>(a &gt;= b) is not true.</td>
</tr>
<tr>
<td>&lt;=</td>
<td>If the value of left operand is less than or equal to the value of right operand, then condition becomes true.</td>
<td>(a &lt;= b) is true.</td>
</tr>
</tbody>
</table><h3 id="iii-assignment--and-compound-operators">(iii)	Assignment  and Compound Operators</h3>
<p>•	Used to assign values to variables<br>
•	Compound operator performs arithmetic operation and then assigns the value<br>
•	Assume variable a holds 10 and variable b holds 20, then</p>

<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td>= Assignment</td>
<td>Assigns values from right side operands to left side operand</td>
<td>c = a + b assigns value of a + b into c</td>
</tr>
<tr>
<td>+= Add &amp; Assign</td>
<td>It adds right operand to the left operand and assign the result to left operand</td>
<td>c += a is equivalent to c = c + a</td>
</tr>
<tr>
<td>-= Subtract &amp; Assign</td>
<td>It subtracts right operand from the left operand and assign the result to left operand</td>
<td>c -= a is equivalent to c = c - a</td>
</tr>
<tr>
<td>*= Multiply and Assign</td>
<td>It multiplies right operand with the left operand and assign the result to left operand</td>
<td>c *= a is equivalent to c = c * a</td>
</tr>
<tr>
<td>/= Divide and Assign</td>
<td>It divides left operand with the right operand and assign the result to left operand</td>
<td>c /= a is equivalent to c = c / ac /= a is equivalent to c = c / a</td>
</tr>
<tr>
<td>%= Modulus &amp; Assign</td>
<td>It takes modulus using two operands and assign the result to left operand</td>
<td>c %= a is equivalent to c = c % a</td>
</tr>
<tr>
<td>**= Exponent &amp; Assign</td>
<td>Performs exponential (power) calculation on operators and assign value to the left operand</td>
<td>c ** = a is equivalent to c = c ** a</td>
</tr>
</tbody>
</table><h3 id="iv-logical-operators">iv) Logical Operators</h3>
<p>•	There are following logical operators supported by Python language. Assume variable a holds 10 and variable b holds 20 then<br>
•	Used to reverse the logical state of its operand.<br>
•	There are following logical operators supported by Python language. Assume variable a holds 10 and variable b holds 20 then –</p>

<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td><em>and</em> Logical AND</td>
<td>If both the operands are true then condition becomes true.</td>
<td>(a and b) is true.</td>
</tr>
<tr>
<td><em>or</em> Logical OR</td>
<td>If any of the two operands are non-zero then condition becomes true.</td>
<td>(a or b) is true.</td>
</tr>
<tr>
<td><em>not</em> Logical NOT</td>
<td>Used to reverse the logical state of its operand.</td>
<td>Not(a and b) is false.</td>
</tr>
</tbody>
</table><h3 id="v-membership-operators">v) Membership Operators</h3>
<p>•	Python’s membership operators test for membership in a sequence, such as strings, lists, or tuples.<br>
•	There are two membership operators as explained below –</p>

<table>
<thead>
<tr>
<th>Operator</th>
<th>Descrription</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td>in</td>
<td>True if value/variable is found in the sequence</td>
<td>5 in numlist, returns true if 5 is in the numlist.</td>
</tr>
<tr>
<td>not in</td>
<td>True if value/variable is not found in the sequence</td>
<td>5 in numlist, returns false if 5 is not in the numlist.</td>
</tr>
</tbody>
</table><h3 id="vi-identity-opertors">vi) Identity Opertors</h3>
<p>•	‘is’ operator – Evaluates to true if the variables on either side of the operator point to the same object and false otherwise.<br>
•	‘is not’ operator – Evaluates to false if the variables on either side of the operator point to the same object and true otherwise.</p>

<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td>is</td>
<td>Evaluates to true if the variables on either side of the operator point to the same object and false otherwise.</td>
<td>x is y, here is results in 1 if id(x) equals id(y).</td>
</tr>
<tr>
<td>is not</td>
<td>Evaluates to false if the variables on either side of the operator point to the same object and true otherwise.</td>
<td>x is not y, here is not results in 1 if id(x) is not equal to id(y).</td>
</tr>
</tbody>
</table><h3 id="conditional-statements">3.1.3	CONDITIONAL STATEMENTS</h3>
<p>•	In programming language conditional statements are used to perform different computations or actions depending on whether a condition evaluates to true or false<br>
•	The conditions use comparisons and arithmetic expressions with variables<br>
•	The expressions are evaluated to Boolean values True or False</p>
<p>Available conditional statements in python are</p>
<ol>
<li>if statement</li>
<li>If…else statement</li>
<li>If…elif…else statement</li>
<li>Nested if statement</li>
</ol>
<p><strong>Rules for conditional statements:</strong><br>
•	The colon(:) is required at the end of the condition<br>
•	The body of the if statement is indicated by the indentation(four spces are used for indentation)<br>
•	Python interprets non-zero values as true and 0 as false</p>
<h3 id="‘if’--statement-conditional-statement">1. ‘if’  STATEMENT (CONDITIONAL STATEMENT)</h3>
<p>•	Sometimes we want to execute a code or a block of code only if a certain condition is satisfied.<br>
•	the program evaluates the condition and will execute statement(s) only if the condition is True.<br>
•	If the condition is False, the statement(s) is not executed.<br>
•	In Python, the body of the if statement is indented.<br>
•	Python interprets non-zero values as True. None and 0 are interpreted as False.</p>
<p><strong>Syntax</strong></p>
<blockquote>
<pre><code> if (test expression/condition):
  	 statement(s)
</code></pre>
<p><strong>Example</strong><br>
Python program to check whether a person is eligible for vote.</p>
</blockquote>
<pre><code>	print("Enter Your age")
	n=int(input()) 
	if(n&gt;=18):
		print("Eligible for voting") 
</code></pre>
<h3 id="‘if...else’-statementalternative-conditional-statement">2. ‘if…else’ STATEMENT(ALTERNATIVE CONDITIONAL STATEMENT)</h3>
<p>•	The if…else statement evaluates test expression and will execute body of if only when test condition is True.<br>
•	If the condition is False, body of else is executed. Indentation is used to separate the blocks.</p>
<p><strong>Syntax of if…else</strong></p>
<pre><code>if (test expression/condition) : 
	Body of if
</code></pre>
<p><strong>Example 1</strong></p>
<pre><code> Python program to checks if the number is positive or negative
num = 3
if num &gt;= 0: 
	print("Positive or Zero")
else:
	print("Negative number")
</code></pre>
<p><strong>Example 2:</strong></p>
<pre><code>print("Enter a number")
num=int(input())
if(num%2)==0: 
   print("Even Number")
else:
    print("Odd Number")
</code></pre>
<h3 id="‘if...elif...else’chained-conditional-statement">3. ‘if…elif…else’(CHAINED CONDITIONAL STATEMENT)</h3>
<p>•	The elif is short for else if. It allows us to check for multiple expressions.<br>
•	If the condition for if is False, it checks the condition of the next elif block and so on.<br>
•	If all the conditions are False, body of else is executed.<br>
•	Only one block among the several if…elif…else blocks is executed according to the condition.<br>
•	The if block can have only one else block. But it can have multiple elif blocks.</p>
<p><strong>Syntax of if…elif…else</strong></p>
<pre><code>if (test expression/condition):
	Body of if
elif (test expression/condition):
	Body of elif
else:
	Body of else
</code></pre>
<p><strong>Example 1:</strong></p>
<pre><code>	Python program to check if the number is positive or negative or zero

	num = 3.4 
	if num &gt; 0:
		print("Positive number") 
	elif num == 0:
		print("Zero") 
	else: 
		print("Negative number")
</code></pre>
<p><strong>Example 2:</strong></p>
<pre><code> n=int(input("Enter a number between seven and ten"))
if(n==7):
    print("heptagon") 
elif(n==8):
    print("octogon") 
elif(n==9):
    print("nanogon") 
elif(n==10):
    print("decagon")
else:
    print("input should be from 7 to 10")
</code></pre>
<h3 id="nested-conditional">4. NESTED CONDITIONAL</h3>
<p>•	A conditional statement defined inside another conditional statement is called nested conditional statement.<br>
•	Any number of these statements can be nested inside one another.<br>
•	Indentation is the only way to figure out the level of nesting.<br>
•	Similarly,  alternative and chained conditionals can also be nested</p>
<p><strong>Example 1</strong></p>
<pre><code>Python program to check if the number is positive or negative or zero using nested if.

num = float(input("Enter a number: ")) 
if num &gt;= 0:
    if num == 0:
        print("Zero")
    else:
        print("Positive number") 
else:
    print("Negative number")
</code></pre>
<h2 id="repetition-structureloopingiterative-statements">3.2. REPETITION STRUCTURE/LOOPING/ITERATIVE STATEMENTS</h2>
<p>•	‘for ‘ Statement<br>
•	‘while’ Statement</p>
<h3 id="‘for’-loop">3.2.1. ‘for’ LOOP</h3>
<p>•	The for loop in Python is used to iterate over a sequence (list, tuple, string) or other iterable<br>
objects.<br>
•	Iterating over a sequence is called traversal.<br>
•	val is the variable that takes the value of the item inside the sequence on each iteration.<br>
•	Loop continues until we reach the last item in the sequence.<br>
•	The body of for loop is separated from the rest of the code using indentation.</p>
<p><strong>Syntax of for Loop</strong></p>
<pre><code>for val in sequence:
	Body of for
</code></pre>
<p>Example: Python for Loop<br>
Python Program to find the sum of all numbers stored in a list</p>
<pre><code>Code:
#number list
numbers = [6, 5, 3, 8, 4, 2, 5, 4, 11]
sum = 0
for val in numbers:
    sum = sum+val 
print("The sum is", sum)
</code></pre>
<h3 id="‘while’-loop">3.2.2. ‘while’ LOOP:</h3>
<p>•	In while loop, test expression is checked first.<br>
•	The body of the loop is entered only if the test expression evaluates to True. After one iteration, the test expression is checked again. This process continues until the test_expression evaluates to False.<br>
•	In Python, the body of the while loop is determined through indentation.<br>
•	Body starts with indentation and the first unintended line marks the end.<br>
•	Python interprets any non-zero value as True. None and 0 are interpreted as False.</p>
<p><strong>Syntax</strong></p>
<pre><code>	while test_expression:
		Body of while
</code></pre>
<p><strong>Example:</strong></p>
<pre><code> Python program using while Loop to add natural numbers upto n 
Code:
	n = int(input("Enter a number: "))
	sum = 0
	i= 1
	while i &lt;= n:
	    sum = sum + i 
	    i = i+1
	print("The sum is", sum)
</code></pre>
<p>In the above program, the test expression will be True as long as our counter variable i is less than or equal to n (10 in our program).</p>
<p><strong>while loop with else</strong><br>
•	An optional else block with while loop can also be used.<br>
•	The else part is executed if the condition in the while loop evaluates to False.<br>
•	The while loop can be terminated with a break statement.</p>
<p><strong>Example:</strong></p>
<pre><code>Python program to illustrate the use of else statement with the while loop

Code:
counter = 0
while counter &lt; 3: 
	print("Inside loop")
	counter = counter + 1 
else:
	print("Inside else")
</code></pre>
<p>•	A counter variable to print the string inside loop three times.<br>
•	On the forth iteration, the condition in while becomes False. Hence, the else part is executed.</p>
<p>**Difference between while and for loop **</p>

<table>
<thead>
<tr>
<th>while loop</th>
<th>for loop</th>
</tr>
</thead>
<tbody>
<tr>
<td>Indefinite loop</td>
<td>Definite loop</td>
</tr>
<tr>
<td>The exit condition will be evaluated again and execution resumes from the top(repeatedly executes a set of code)</td>
<td>The for is to iterate over a sequence (List, Tuple and dictionary etc)</td>
</tr>
</tbody>
</table><h3 id="unconditional-statements">3.2.3. UNCONDITIONAL STATEMENTS</h3>
<p>•	Unconditional statements are used in the situations, there is a need to exit the loop completely when an external condition is triggered or there may be a situation to skip a part of the code and start the next execution.<br>
•	Python provide the following statements</p>
<blockquote>
<pre><code>     i.   Break
     ii.  Continue
     iii. Pass
</code></pre>
</blockquote>
<p>•	In Python, break and continue statements can alter the flow of a normal loop.<br>
•	Loops iterate over a block of code until test expression is false, to terminate the current iteration or even the whole loop without checking test expression.<br>
•	The break and continue statements are used in these cases.</p>
<p><strong>(i) Python break statement</strong></p>
<p>•	The break statement terminates the loop containing it.<br>
•	Control of the program flows to the statement immediately after the body of the loop.<br>
•	If break statement is inside a nested loop (loop inside another loop), break will terminate the innermost loop.</p>
<p>Syntax of break</p>
<pre><code>break
</code></pre>
<p><strong>Example 1:</strong></p>
<pre><code>	Python program to illustrate break statement inside loop
Code:

for val in "string":
	if val == "i":
		 	break
	print(val)  
print("The end")
</code></pre>
<p><strong>Example 2:</strong></p>
<pre><code>Python program to demonstrate break
Code:

i=1
while i&lt;=10:
	print(i)
	if(i==5):
		break
print(“completed”)
</code></pre>
<p><strong>(ii)	Python continue statement</strong></p>
<p>•	The continue statement is used to skip the rest of the code inside a loop for the current iteration only.<br>
•	Loop does not terminate but continues on with the next iteration.</p>
<p><strong>Syntax of Continue</strong></p>
<pre><code>continue
</code></pre>
<p><strong>Example 1:</strong></p>
<pre><code>Python Program to show the use of continue statement inside loops
Code:
for val in "string": 
	if val == "i":
		continue 
		print(val)
print("The end")
</code></pre>
<p>•	This program is same as the above example except the break statement has been replaced with continue.<br>
•	continue with the loop, if the string is “i”, not executing the rest of the block. Hence, we see in our output that all the letters except “i” gets printed.</p>
<p><strong>Example 2:</strong></p>
<pre><code>Python Program to show the use of continue statement inside loops
Code:
n=int(input())
for i in range(0,n):
	a=int(input()) 
	if(a&lt;0):
		continue
</code></pre>
<p><strong>(iii)	Pass STATEMENT</strong><br>
•	It is used when a statement is required syntactically but you do not want any command or code to execute.<br>
•	The pass statement is a null operation; nothing happens when it executes. The pass is also useful in places where your code will eventually go, but has not been written yet.</p>
<p>Syntax of pass</p>
<pre><code>pass
</code></pre>
<p><strong>Example 1:</strong></p>
<pre><code>Python program to illustrate pass

Code:
for letter in 'Python': 
	if letter == 'h': 
		pass
		print 'This is pass block' 
    print 'Current Letter :',letter 
print "Good bye!"
</code></pre>
<p><strong>Example 2:</strong></p>
<pre><code>for num in [20, 11, 9, 66, 4, 89, 44]:
    if num%2 == 0:
        pass
    else:
        print(num)
</code></pre>
<h2 id="fruitful-functions-return-values-parameters-local-and-global-scope-function-composition-recursion">3.3. FRUITFUL FUNCTIONS: RETURN VALUES, PARAMETERS, LOCAL AND GLOBAL SCOPE, FUNCTION COMPOSITION, RECURSION</h2>
<h3 id="functions-1">3.3.1. Functions</h3>
<p>•	Function is a group of statements that together perform a task.<br>
•	A function is a block of organized, reusable code that is used to perform a single, related action.<br>
Defining a Function<br>
Simple rules to define a function in Python.<br>
•	Function blocks begin with the keyword def followed by the function name and parentheses ( ).<br>
•	Any input parameters or arguments should be placed within these parentheses. You can also define parameters inside these parentheses.<br>
•	The first statement of a function can be an optional statement - the documentation string of the function or docstring.<br>
•	The code block within every function starts with a colon (:) and is indented.<br>
•	The statement return [expression] exits a function, optionally passing back an expression to the caller. A return statement with no arguments is the same as return none.</p>
<p><strong>Syntax</strong></p>
<pre><code>def functionname( parameters ): 
	"function_docstring"
	function body
	return [expression]
</code></pre>
<p><strong>Creating a function</strong></p>
<pre><code>def my_function(): 
	print("Hello from a function")
</code></pre>
<p><strong>Calling a Function</strong><br>
To call a function, use the function name followed by parenthesis.</p>
<p><strong>Example:</strong></p>
<pre><code>def my_function(): 
	print("Hello from a function") 
my_function()
</code></pre>
<p><strong>Parameters</strong></p>
<p>•	Information can be passed to functions as parameter.<br>
•	Parameters are specified after the function name, inside the parentheses. You can add as many parameters as you want, just separate them with a comma.<br>
•	The following example has a function with one parameter (fname). When the function is called, we pass along a first name, which is used inside the function to print the full name:</p>
<p><strong>Example:</strong></p>
<pre><code>def my_function(fname): 
	print(fname + " Refsnes")

#main function
my_function("Emil") 
my_function("Tobias") 
my_function("Linus")
</code></pre>
<p><strong>Default Parameter Value</strong></p>
<p>•	The following example shows how to use a default parameter value.<br>
•	If we call the function without parameter, it uses the default value:</p>
<p><strong>Example:</strong></p>
<pre><code>def my_function(country = "Norway"): 
	print("I am from " + country)

#main function
my_function("Sweden") 
my_function("India") 
my_function() 
my_function("Brazil")
</code></pre>
<h3 id="return-values">3.3.2	Return Values</h3>
<p>•	The statement return [expression] exits a function, optionally passing back an expression to the caller. A return statement with no arguments is the same as return None.<br>
•	All the above examples are not returning any value. You can return a value from a function as follows</p>
<pre><code># Function definition is here 
def sum( arg1, arg2 ):
	# Add both the parameters and return them." 
	total = arg1 + arg2
	print("Inside the function : ", total)
	return total;

# Now you can call sum function 
total = sum( 10, 20 );
print("Outside the function : ", total)
</code></pre>
<p><strong>Example 2:</strong></p>
<pre><code>def my_function(x):
	return 5 * x
#function calling statements
print(my_function(3)) 
print(my_function(5)) 
print(my_function(9))
</code></pre>
<h3 id="function-arguments">3.3.3 Function Arguments</h3>
<p>The following types of formal arguments:</p>
<p>•	Required arguments<br>
•	Keyword arguments<br>
•	Default arguments<br>
•	Variable-length arguments</p>
<p><strong>Required arguments</strong><br>
•	Required arguments are the arguments passed to a function in correct positional order.<br>
•	The number of arguments in the function call should match exactly with the function definition.</p>
<p><strong>Example</strong></p>
<pre><code>#Function definition where str is the required argument
def display(str): 
	print str

#main script
str=”hello”
display(str)
</code></pre>
<p><strong>Keyword arguments</strong><br>
•	Keyword arguments are related to the function calls.<br>
•	When keyword arguments in a function call, the caller identifies the arguments by the parameter name.<br>
•	This allows you to skip arguments or place them out of order because the Python interpreter is able to use the keywords provided to match the values with parameters.</p>
<p><strong>Example</strong></p>
<pre><code>def display(str,integer,float1):
	print(“The string is:”,str) 
	print(“The integer is:”,integer) 
	print(“The float is:”,float1)

#Main script-Fucntion calling with keyword arguments
display(float=58.62,str=”hello”,int=28)
</code></pre>
<p><strong>Default arguments</strong><br>
•	A default argument is an argument that assumes a default value if a value is not provided in<br>
the function call for that argument.<br>
•	The following example gives an idea on default arguments, it prints default age if it is not passed</p>
<pre><code>def printinfo( name, age = 35 ):
	"This prints a passed info into this function"
	print("Name: ",name)
	print("Age ",age)
	return
#Calling printinfo function 
printinfo(age=50, name="miki" )
printinfo(name="miki")
</code></pre>
<p><strong>Variable-length arguments</strong><br>
•	Variable length argument make function calls with many(arbitary).<br>
•	These arguments are called variable-length arguments and are not named in the function definition, unlike required and default arguments.</p>
<p><strong>Syntax:</strong></p>
<pre><code>def functionname([formal_args,] *var_args_tuple ):
	"function_docstring"
	function body
	return [expression]
</code></pre>
<p>An asterisk (*) is placed before the variable name that holds the values of all non keyword variable arguments. This tuple remains empty if no additional arguments are specified during the function call.</p>
<p><strong>Example 1</strong></p>
<pre><code>	def printinfo( arg1, *vartuple ):
	    "This prints a variable passed arguments" 
	    print("Output is:")
	    print(arg1)
	    for var in vartuple: 
	        print(var)
	    return

	printinfo( 10 )
	printinfo( 70, 60, 50 )
</code></pre>
<h3 id="scope-of-variables">3.3.4. Scope of Variables</h3>
<p>•	All variables in a program may not be accessible at all locations in that program. This depends on where you have declared a variable.<br>
•	The scope of a variable determines the portion of the program where you can access a particular identifier.<br>
•	There are two basic scopes of variables in Python −<br>
•	Global variables<br>
•	Local variables</p>
<p><strong>Global vs. Local variables</strong></p>
<p>•	Variables that are defined inside a function body have a local scope, and those defined outside have a global scope.<br>
•	This means that local variables can be accessed only inside the function in which they are declared, whereas global variables can be accessed throughout the program body by all functions.<br>
•	When you call a function, the variables declared inside it are brought into scope.</p>
<p><strong>Example 1</strong></p>
<pre><code>	total = 0; # This is global variable. 
	def sum( arg1, arg2 ):
	# Add both the parameters and return them."
		total = arg1 + arg2; # Here total is local variable. 
		print("Inside the function local total : ", total)
		return total;
	# Calling sum function 
	sum( 10, 20 );
	print("Outside the function global total : ", total)
</code></pre>
<h3 id="function-composition-or-anonymous-functions">3.3.5. Function composition or Anonymous Functions</h3>
<p>•	Function composition is the way of combining the functions<br>
•	These functions are called anonymous because they are not declared in the standard manner by using the def keyword. You can use the lambda keyword to create small anonymous functions.<br>
•	Lambda forms can take any number of arguments but return just one value in the form of an expression. They cannot contain commands or multiple expressions.<br>
•	An anonymous function cannot be a direct call to print because lambda requires an expression<br>
Syntax</p>
<pre><code>lambda [arg1 [,arg2,.....argn]]:expression
</code></pre>
<p><strong>Example 1:</strong></p>
<pre><code># Function definition is here
sum = lambda arg1, arg2: arg1 + arg2;
# Now you can call sum as a function 
print("Value of total : ", sum( 10, 20 ))
print("Value of total : ", sum( 20, 20 ))
</code></pre>
<h3 id="recursive-function">3.3.6. Recursive Function:</h3>
<p>•	Recursion is the process of the function call by itself.<br>
•	In Python, a function can call other functions. It is even possible for the function to call itself. These type of construct are termed as recursive functions.<br>
•	Example - recursive function to find the factorial of an integer.</p>
<p>Factorial of a number is the product of all the integers from 1 to that number. For example, the factorial of 6 (denoted as 6!) is 1<em>2</em>3<em>4</em>5*6 = 720.</p>
<p><strong>Example 1:</strong></p>
<pre><code>def calc_factorial(x):
"""This is a recursive function
to find the factorial of an integer""" 
	if x == 1:
		return 1 
	else:
		return (x * calc_factorial(x-1)) 

#Main Script
num = 4
print("The factorial of", num, "is",calc_factorial(num))
</code></pre>
<p>•	In the above example, calc_factorial() is a recursive functions as it calls itself.<br>
•	This function with a positive integer, it will recursively call itself by decreasing the number.<br>
•	Each function call multiples the number with the factorial of number 1 until the number is equal to one. This recursive call can be explained in the following steps.</p>
<p>calc_factorial(4)	# 1st call with 4</p>
<ul>
<li>calc_factorial(3)	# 2nd call with 3</li>
<li>3 * calc_factorial(2)	# 3rd call with 2</li>
<li>3 * 2	* calc_factorial(1)	# 4th call with 1</li>
<li>3	* 2	* 1	# return from 4th call as number=1</li>
<li>3	* 2		# return from 3rd call</li>
<li>6			# return from 2nd call<br>
# return from 1st call</li>
</ul>
<p>•	Our recursion ends when the number reduces to 1. This is called the base condition.<br>
•	Every recursive function must have a base condition that stops the recursion or else the function calls itself infinitely.</p>
<p><strong>Advantages of recursion</strong></p>
<ol>
<li>Recursive functions make the code look clean and elegant.</li>
<li>A complex task can be broken down into simpler sub-problems using recursion.</li>
<li>Sequence generation is easier with recursion than using some nested iteration.</li>
</ol>
<p><strong>Disadvantages of recursion</strong></p>
<ol>
<li>Sometimes the logic behind recursion is hard to follow through.</li>
<li>Recursive calls are expensive (inefficient) as they take up a lot of memory and time.</li>
<li>Recursive functions are hard to debug.</li>
</ol>
<h2 id="strings-1">3.4. STRINGS</h2>
<p>A string is a sequence of characters. You can access the characters one at a time with the bracket operator:</p>
<pre><code>fruit = 'banana'
letter = fruit[1]
</code></pre>
<p>The second statement selects character number 1 from fruit and assigns it to letter. The expression in brackets is called an index. The index indicates which character in the sequence you want (hence the name). Always index starts from 0. The value of the index has to be an integer. Otherwise you get:</p>
<pre><code>letter = fruit[1.5]
TypeError: string indices must be integers, not float
</code></pre>
<h3 id="len">3.4.1. len()</h3>
<p>len is a built-in function that returns the number of characters in a string:</p>
<pre><code>fruit = 'banana'
print(len(fruit)) #Output is 6
</code></pre>
<p>To get the last letter of a string, you might be tempted to try something like this:</p>
<pre><code>length = len(fruit)
last = fruit[length]
print(last)

# Causes following output
IndexError: string index out of range	
</code></pre>
<p>The reason for the IndexError is that there is no letter in ‘banana’ with the index 6. Since we started counting at zero, the six letters are numbered 0 to 5. To get the last character, you have to subtract 1 from length:</p>
<pre><code>last = fruit[length-1]
print(last)  #dispalys a
</code></pre>
<p>Alternatively, you can use negative indices, which count backward from the end of the string. The expression fruit[-1] yields the last letter, fruit[-2] yields the second to last,<br>
and so on.</p>
<h3 id="string-slices">3.4.2. String slices</h3>
<p>A segment of a string is called a slice. Selecting a slice is similar to selecting a character:</p>
<pre><code>str = 'Monty Python'
print(str[0:5])      #Prints Monty
print(str[6:12]      #Prints Python
</code></pre>
<p>The operator [n:m] returns the part of the string from the “n-eth” character to the “m-eth” character, including the first but excluding the last.<br>
If you omit the first index (before the colon), the slice starts at the beginning of the string. If you omit the second index, the slice goes to the end of the string:</p>
<pre><code>fruit = 'banana'
print(fruit[:3])  #Prints 'ban'
print(fruit[3:]   #Prints 'ana'
</code></pre>
<p>If the first index is greater than or equal to the second the result is an empty string, represented by two quotation marks:</p>
<pre><code>fruit = 'banana'
print(fruit[3:3]) #Prints ' '
</code></pre>
<p>An empty string contains no characters and has length 0, but other than that, it is the same as any other string.</p>
<h3 id="strings-are-immutable">3.4.3. Strings are immutable</h3>
<p>It is tempting to use the [] operator on the left side of an assignment, with the intention of changing a character in a string. For example:</p>
<pre><code>greeting = 'Hello, world!'
greeting[0] = 'J'
#Causes following output
TypeError: 'str' object does not support item assignment
</code></pre>
<p>The “object” in this case is the string and the “item” is the character you tried to assign. For now, an object is the same thing as a value, but we will refine that definition later. An item is one of the values in a sequence.<br>
The reason for the error is that strings are immutable, which means you can’t change an existing string. The best you can do is create a new string that is a variation on the original:</p>
<pre><code>greeting = 'Hello, world!'
new_greeting = 'J' + greeting[1:]
print(new_greeting)       #Prints Jello, world!
</code></pre>
<p>This example concatenates a new first letter onto a slice of greeting. It has no effect on the original string.</p>
<h3 id="string-methods">3.4.4. String methods</h3>
<p>A method is similar to a function—it takes arguments and returns a value—but the syntax is different. For example, the method upper takes a string and returns a new string with all uppercase letters:<br>
Instead of the function syntax upper(word), it uses the method syntax word.upper().</p>
<pre><code>word = 'banana'
new_word = word.upper()
print(new_word)    #Prints BANANA
</code></pre>
<p>This form of dot notation specifies the name of the method, upper, and the name of the string to apply the method to, word. The empty parentheses indicate that this method<br>
takes no argument.<br>
A method call is called an invocation; in this case, we would say that we are invoking upper on the word.<br>
As it turns out, there is a string method named find that is remarkably similar to the function we wrote:</p>
<pre><code> word = 'banana'
 index = word.find('a')
 print(index)    #Prints 1
</code></pre>
<p>In this example, we invoke find on word and pass the letter we are looking for as a parameter.</p>
<h4 id="i-find-method">(i) find method</h4>
<p>Actually, the find method is more general than our function; it can find substrings, not just characters:</p>
<pre><code>word = 'banana'
print(word.find('na'))    #Prints 2
</code></pre>
<p>It can take as a second argument the index where it should start:</p>
<pre><code>word = 'banana'
print(word.find('na', 3))   # Prints 4
</code></pre>
<p>And as a third argument the index where it should stop:</p>
<pre><code>name = 'bob'
print(name.find('b', 1, 2))   #Prints -1
</code></pre>
<p>This search fails because b does not appear in the index range from 1 to 2 (not including 2).</p>
<h4 id="ii-string-comparison">(ii) String comparison</h4>
<p>The relational operators work on strings. To see if two strings are equal:</p>
<pre><code>if(word == 'banana'):
	print('All right, bananas.')
</code></pre>
<p>Other relational operations are useful for putting words in alphabetical order:</p>
<pre><code>if(word &lt; 'banana'):
	print('Your word,' + word + ', comes before banana.')
elif(word &gt; 'banana'):
	print('Your word,' + word + ', comes after banana.')
else:
	print('All right, bananas.')
</code></pre>
<p>Python does not handle uppercase and lowercase letters the same way that people do. All the uppercase letters come before all the lowercase letters, so:Your word, Pineapple, comes before banana.<br>
A common way to address this problem is to convert strings to a standard format, such as all lowercase, before performing the comparison. Keep that in mind in case you have to defend yourself against a man armed with a Pineapple.</p>
<h4 id="iii-indexing">(iii) Indexing</h4>
<p>Individual characters in a string can be accessed using subscript([ ]) operator. The expression in bracket is called as Index.</p>
<h4 id="iv-traversing-a-string">(iv) Traversing a String</h4>
<p>A string can be traversed by accessing characters from one index to another.</p>

<table>
<thead>
<tr>
<th>P</th>
<th>Y</th>
<th>T</th>
<th>H</th>
<th>O</th>
<th>N</th>
</tr>
</thead>
<tbody>
<tr>
<td>0</td>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td>5</td>
</tr>
<tr>
<td>-6</td>
<td>-5</td>
<td>-4</td>
<td>-3</td>
<td>-2</td>
<td>-1</td>
</tr>
</tbody>
</table><h3 id="string-module">3.4.4 . String module</h3>
<p>•	The string module consists of number of useful constants,classes and functions<br>
•	These functions are used to manipulate strings<br>
•	Some constants are defined in string module are:</p>
<ol>
<li>string.ascii_lowercase<br>
Refers all lower case letters. Example: a-z</li>
<li>string.ascii_uppercase<br>
Refers all upper case letters. Example: A-Z 3.string.digits<br>
Refer digits from 0-9 4.string.uppercase<br>
A string that has all the characters that are considered upper case letters Example: A-Z<br>
5.string.whitespace<br>
A string that has all characters that are considered white space like space,tab etc<br>
Example: Hello world Hai Ajay<br>
Output: HelloworldHaiAjay</li>
</ol>
<p><strong>Example:</strong><br>
Program that use different string methods</p>
<pre><code>str=”welcome to the world of python”
print(“uppercase=”,str.upper( )) 
print(“lowercase=”,str.lower( )) 
print(“split=”,str.split( )) 
print(“join=”,’-‘.join(str.split( )))
print(“replace=”,str.replace(“python”,”java” )) 
print(“count of o=”,str.count(‘o’ ))
print(“find of =”,str.find(“of”))
</code></pre>
<h3 id="example-programs">3.4.5. Example Programs:**</h3>
<p>**1.	Traversing a string **</p>
<pre><code>message=”hello!” 
index=0
for i in message:
	print(“message[“,/index,”]=”,i) index+=1
</code></pre>
<p><strong>2.	String operations</strong></p>
<pre><code>str=”Hello This is python” 
i=2
print(str[i]) 
print(str[i*3+1]) 
</code></pre>
<p><strong>3.	Concatenate two strings</strong></p>
<pre><code>str1=”hello” str2=”world” 
str3=str1+str2
print(“the string is:”,str3)
</code></pre>
<p><strong>4.	Append a string</strong></p>
<pre><code>Str=”Hello” 
N=raw_input() 
Str+=n;
print(str)
</code></pre>
<p><strong>5.String slices</strong></p>
<p>•	A substring of a string is called a slice<br>
•	A slice operation is used to refer the subpart of strings<br>
•	The subset of a string can be taken from string by using [ ] operator<br>
<strong>Example 1: Positive Indexing/Slicing</strong></p>
<pre><code>str=”python” 
print(“str[1:5]=”,str[1:5])
print(“str[:6]=”,str[:6])
print(“str[1:]=”,str[1:])
print(“str[:]=”,str[:])
print(“str[1:20]=”,str[1:20])
</code></pre>
<p><strong>Example 2: Negative Indexing/Slicing</strong></p>
<pre><code>str=”python” print(“str[-1]=”,str[-1])
print(“str[-6]=”,str[-6])
print(“str[-2:]=”,str[-2:])
print(“str[:-2]=”,str[:-2])
print(“str[-5:-2]=”,str[-5:-2])
</code></pre>
<p><strong>Example:3</strong></p>
<pre><code>str=”welcome to the world of python”
print(“str[2:10]=”,str[2:10])
print(“str[2:10:1]=”,str[2:10:1])
print(“str[2:10:2]=”,str[2:10:2])
print(“str[2:13:4]=”,str[2:13:4])
print(“str[::3]=”,str[::3])
print(“str[::-1]=”,str[::-1])
print(“str[::-3]=”,str[::-3])
</code></pre>
<p><strong>6.String Immutability</strong><br>
•	Python strings are immutable<br>
•	Once the strings are created it cannot be modified<br>
•	To modify an existing string variable, a new string is created<br>
•	The id() returns the memory address of that object<br>
•	Str1 and str2 have the same object, then both point to same object</p>
<p><strong>6.String Immutability</strong><br>
•	Python strings are immutable<br>
•	Once the strings are created it cannot be modified<br>
•	To modify an existing string variable, a new string is created<br>
•	The id() returns the memory address of that object<br>
•	Str1 and str2 have the same object, then both point to same object</p>
<h3 id="string-functions-and-methods">3.4.6. String functions and methods</h3>
<p>•	Python supports many build-in methods to manipulate strings<br>
•	A method is like a function</p>

<table>
<thead>
<tr>
<th>SNo</th>
<th>Function</th>
<th>Descrition</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td>1</td>
<td>capitalize()</td>
<td>Capitalizes first letter of string</td>
<td>str=”hello” print(str.capitalize())</td>
</tr>
<tr>
<td>2</td>
<td>count(str,beg,end)</td>
<td>Count the number of times str occurs in a String</td>
<td>str=”he” m=”hellohellohello” print(m.count(str,0,len(m))</td>
</tr>
<tr>
<td>3</td>
<td>endwith(suffix,beg,end)</td>
<td>Check the string is end with given end string</td>
<td>m=”she is my friend” print(m.endwith(“end”,0,len(m))</td>
</tr>
<tr>
<td>4</td>
<td>startwith(prefix,beg,end)</td>
<td>Check the string starts with given string</td>
<td>m=”the world” print(m.startwith(“th”,0,len(m))</td>
</tr>
<tr>
<td>5</td>
<td>find(str,beg,end)</td>
<td>Check if the str is present in the string</td>
<td>m=”she is my friend” print(m.find(“my”,0,len(m))</td>
</tr>
<tr>
<td>6</td>
<td>isalpha()</td>
<td>Return true,if the string contain only alphabet</td>
<td>m=”jamesbond007” print(m.isalpha())</td>
</tr>
<tr>
<td>7</td>
<td>isdigit()</td>
<td>Return true,if the string contain only digit</td>
<td>m=”007”print(m.isdigit())</td>
</tr>
<tr>
<td>8</td>
<td>isalnum()</td>
<td>Return True,if string contain both alphabets and number</td>
<td>m=”james007” print(m.isalnum())</td>
</tr>
<tr>
<td>9</td>
<td>islower()</td>
<td>Returns true,if string contain only lower case</td>
<td>m=”hello” print(m.islower())</td>
</tr>
<tr>
<td>10</td>
<td>isupper()</td>
<td>Returns true,if string contain only upper case</td>
<td>m=”hello” print(m.isupper())</td>
</tr>
<tr>
<td>11</td>
<td>len(string)</td>
<td>Returns the length of the string</td>
<td>str=”hello” print(len(str))</td>
</tr>
<tr>
<td>12</td>
<td>lower()</td>
<td>Convert all the character into lowercase</td>
<td>m=”HELLO” print(m.lower())</td>
</tr>
<tr>
<td>13</td>
<td>upper()</td>
<td>Convert all the character into uppercase</td>
<td>m=” hello” print(m.upper())</td>
</tr>
<tr>
<td>14</td>
<td>strip()</td>
<td>Remove all the white space</td>
<td>m=”he llo” print(m.strip())</td>
</tr>
<tr>
<td>15</td>
<td>max(str)</td>
<td>Returns highest alphabetic character(ASCII value)</td>
<td>m=”hello zuzu” print(max(m))</td>
</tr>
<tr>
<td>16</td>
<td>min(str)</td>
<td>Returns the lowest alphabetical character</td>
<td>m=”hello zuzu” print(min(m))</td>
</tr>
<tr>
<td>17</td>
<td>split(delim)</td>
<td>Returns the list of substrings separated by the specified delimiter</td>
<td>m=”hello,hai,sai” print(m.split(‘,’))</td>
</tr>
</tbody>
</table>