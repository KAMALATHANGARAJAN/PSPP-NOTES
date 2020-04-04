---


---

<h2 id="unit-iii-control-flow-functions">UNIT III CONTROL FLOW, FUNCTIONS</h2>
<p><strong>Conditionals: Boolean values and operators, conditional (if), alternative (if-else), chained conditional (if-elif-else); Iteration: state, while, for, break, continue, pass; Fruitful functions: return values, parameters, local and global scope, function composition, recursion; Strings: string slices, immutability, string functions and methods, string module; Lists as arrays. Illustrative programs: square root, gcd, exponentiation, sum an array of numbers, linear search, binary search</strong></p>
<h3 id="conditionals">3.1. CONDITIONALS:</h3>
<h4 id="boolean-values-and-operators">3.1.1 BOOLEAN VALUES AND OPERATORS:</h4>
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
</table><h4 id="boolean-and-logical-operators">Boolean and Logical operators</h4>
<h4 id="and-operator">1. <em>and</em> Operator:</h4>

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
</table><h4 id="or-operator">1. <em>or</em> Operator:</h4>

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
</table><h4 id="example-1-“and”-operator">Example 1: “and” operator</h4>
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
<h4 id="example-1-“or”-operator">Example 1: “or” operator</h4>
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
<h4 id="operators">3.1.2. OPERATORS</h4>
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
<h4 id="i-arithmetic-operators">i) Arithmetic operators</h4>
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
</table><h4 id="ii-comparison-operators">(ii)	Comparison Operators</h4>
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
</table><h4 id="iii-assignment--and-compound-operators">(iii)	Assignment  and Compound Operators</h4>
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
</table><h4 id="iv-logical-operators">iv) Logical Operators</h4>
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
</table><h4 id="v-membership-operators">v) Membership Operators</h4>
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
</table><h4 id="vi-identity-opertors">vi) Identity Opertors</h4>
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
</table><h4 id="conditional-statements">3.1.3	CONDITIONAL STATEMENTS</h4>
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
<h4 id="‘if’--statement-conditional-statement">1. ‘if’  STATEMENT (CONDITIONAL STATEMENT)</h4>
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
</blockquote>

