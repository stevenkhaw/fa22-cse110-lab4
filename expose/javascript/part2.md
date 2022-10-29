# Part 2
## Steven Khaw
<hr>

### Question 1.  
Line 12 will print out the length of the discounted array. In this case it 
will print out 3. The for loop runs 3 times, from i..2, however, i ends up
being 3 because of the way how for loops work. The i is incremented one more
time and because i ended up being greater than or equal to the prices.length,
the for loop halted. The variable 'i' is also still able to be read and 
accessed because it was defined using the var keyword, meaning it has a 
function scope.

### Question 2.
Line 13 will print '150' because it will print the last instance of 
discountedPrice which is 300 * (1 - 0.5). It prints the last discountedPrice 
which is composed of prices[2] (which is equal to 300), then multiply that 
by (1 - discount) which is 0.5. Ultimately, this results to 150.

### Question 3.
Line 14 will print '150' because it will print the last instance of finalPrice.
finalPrice is equal to the rounded value of the last discounted price, 
first multiplied by 100 to get it to round the cent, then divided to 
turn it back into a dollar.cent format. 

### Question 4.
This function will print the array [50, 100, 150]. This is because it 
returns discounted which is a variable that holds a list with a scope of the 
function. The function appends/pushes each finalPrice to the list that it 
outputs. Therefore, because the input was 100 200 and 300, it will output
a list of the prices discounted by 50%, thus, 50, 100, 150.

### Question 5.
Line 12 will cause an error. This is because the variable 'i' was defined
using the keyword 'let' meaning it is defined within the block scope. Because
of this, the variable 'i' can only be used within the for statement and no 
where else unless defined otherwise.It causes an error because there is 
no such thing as 'i' outside of the for statement.

### Question 6. 
Line 13 will cause an error. This is again because the variable 
'discountedPrices' was defined with the 'let' keyword inside the for statement
meaning that the variable can only be called within the for statement. It 
causes an error because there is no such thing as 'discountedPrice' outside
of the for statement.

### Question 7. 
Line 14 will print 'finalPrice' which is 150. The variable exists because 
it was created with the let keyword but within the function block, thus
anything within the function can use this variable. The math behind why the 
number is 150 does not change from question 3. 

### Question 8.
This function will return the same as when the variables were defined via the
keyword var. It will return [50, 100, 150]. The math does not change from 
question 4. This is because all variables are still used within their same 
scope and no errors occur in the code.

### Question 9.
Line 11 will result in an error. This is because, like question 5, the variable
'i' was defined with the let keyword making it within the scope of the for 
statement only. Line 11 cannot read/access 'i' because it does not exist in 
its scope.

### Question 10.
Line 10 will print 3. The variable 'length' is a constant and was defined
only once and never redefined or modified after its initialization. The
const variable has the scope of the whole function, thus it can be called 
anywhere inside the function.

### Question 11.
This function will return [50, 100, 150]. A common mistake people might make is
that becuase the array is a constant, that you cannot add elements to it. 
However, that is wrong. Because it is a constant, you are no longer able to 
redeclare the array, however, you can modify the elements inside of it.

### Question 12.
A. student.name;  
B. student['Grad Year'];  
C. student.greeting();  
D. student["Favorite Teacher"].name;  
E. student.courseLoad[0];  

### Question 13.
A. 32 because '3' + 2 will convert 2 to a string and append it to '3' making it
'32'.  
B. 1 because '3' - 2 will map '3' to 3 and compute 3 - 2 resulting in 1.  
C. 3 because 3 + null will map null to 0, thus the computation is 3 + 0.  
D. '3null' because it will map null to the string 'null' and append it to '3'.  
E. 4 because true maps to 1, thus the computation is 1 + 3.  
F. 0 because false maps to 0 and null maps to 0, thus 0 + 0.  
G. '3undefined' becuase it maps undefined to 'undefined' and appends it to '3'.  
H. NaN becuase undefined cannot map to a number resulting in a Nan.  

### Question 14.
A. true because '2' maps to 2 which is greater than 1.  
B. false because the first char '2' is less than the first char '1'.  
C. true because '2' maps to 2 which is equal to 2.  
D. false becuase === checks equality without type conversion. Thus, already
2 is not of the same type as '2'.  
E. false because true maps to 1 which is not equal to 2.  
F. true because Boolean(2) maps to the true boolean which is equal to true.

### Question 15.
== is the equal comparison with type-casting enabled while === is the equal
comparaison without type-casting.

### Question 17.
The function will return [2, 4, 6]. This function takes in an array and a 
callback function. In conjunction, this function will apply the callback 
function on every element in array. This is basically the map function. What 
is going on inside the function is the following: First, the output array is 
initalized. Then the function iterates through the input array and calls the 
callback function on every element and appends the resulting element to the 
output array. Lastly, the output array is returned. 

### Question 19.
The output should be 
1
4
3
2
The first 1 and 4 prints instantly because there is no timeout. Then 3 is 
printed because there is a slight timeout of 4 ms normally. Lastly, 2 is 
printed after 1 second or 1000 milliseconds.