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
