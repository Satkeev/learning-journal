### USING WHILE LOOPS
>Here is an example of awhil e 
loop. It writes out the 5 times 
table. Each time the loop is run, 
another calculation is written 
into the variable called msg. 
This loop will continue to run 
for as long as the condition in 
the parentheses is true. That 
condition is a counter indicating 
that, as long as the variable 
i remains less than 10, the 
statements in the subsequent 
code block should run. 
Inside the code block there are 
two statements:    
>The first statement uses the      
new content to the msg variable.    
Each time the loop runs, a new    
calculation and line break is    
added to the end of the message     
being stored in it. So+" works as    
a shorthand for writing:    
msg = msg + 'new msg'    
(See bottom of the next page for   
a breakdown of this statement.)   
The second statement   
increments the counter variable   
by one. (This is done inside   
the loop rather than with the  
condition.)  
When the loop has finished, the  
interpreter goes to the next line   
of code, which writes the msg   
variable to the page.    

##USING FOR LOOPS  

#JAVASCRIPT c04/js/for-loop .js  

>var scores= [24. 32, 17]; //Array of scores  
var arraylength scores.l ength; // Items in array  
var roundNumber = O; //Current round  
var msg ''; //Message  
var i ; // Counter  
//Loop through the items in the array  
for (i = O; i < arraylength; i++) {  
//Arrays are zero based (so 0 is round 1)  
//Add 1 to the current round  
roundNumber = (i + l);  
// Write the current round to message  
msg += 'Round ' + roundNumber + ' : ';  
//Get the score from the scores array  
msg += scores[i] + '<br / >' ;  
document .getElementByid( 'answer') .i nnerHTML msg;  
i;ff>iiiil  
Round 1: 24  
Round 2: 32  
Round 3: 17  
The counter and array both start from 0 (rather than 1). So, within the loop,  
to select the current item from the array, you use the counter variable i to  
specify the item from the array, e.g., scores [ i]. But remember that it is a  
number lower then you might expect (e.g., first iteration is 0, second is 1).  
A for loop is often used to loop  
through the items in an array.  
In this example, the scores for  
each round of a test are stored in  
an array called scores.  
The total number of items in  
the array is stored in a variable  
called arrayl ength. This  
number is obtained using the  
l ength property of the array.  
There are three more variables:  
roundNumber holds the round of   
to display; i is the counter  
(declared outside the loop).  
The loop starts with the for  
keyword, then contains the  
condition inside the parentheses.  
As long as the counter is less  
than the total number of items  
in the array, the contents of the  
curly braces will continue to  
run. Each time the loop runs, the  
round number is increased by     
Inside the curly braces are rules  
that write the round number and  
the score to the msg variable. The  
variables declared outside of the  
loop are used within the loop.  
The msg variable is then written  
into the page. It contains HTML  
so the i nnerHTML property is  
used to do this. Remember,
p228 will talk about security
issues relating to this property.
