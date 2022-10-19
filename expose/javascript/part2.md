# Part 2
## Steven Khaw
<hr>

### Question 1.  
Line 12 will print out the length of the discounted array. In this case it 
will print out '3'. The for loop runs 3 times, from i..2, however, i ends up
being 3 because of the way how for loops work. The i is incremented one more
time and because i ended up being greater than or equal to the prices.length,
the for loop halted. The variable 'i' is also still able to be read and 
accessed because it was defined using the var keyword, meaning it has a 
function scope.

### Question 2.
Line 13 will print '150' because that is 300 * (1 - 0.5). 