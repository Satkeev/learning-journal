### JAVASCR IPT c04/ js/ do-while-loop.j s  

>var i = l; //Set counter  
var msg : ' '; //Message      
 
// Store 5 times table in a variable 
do { 
msg += i + ' x 5 = ' + (i * 5) + '<br I>' ;s 
i++; 
} wh il e ( i < 1) ; 
>II Note how this is already 1 and it still runs 
document .getEl ementByld(' answer').innerHTML = msg; 


lxS=S 
Breaking down the first statement in these examples: 
1 2 3 4 5 6 
1. Take variable called msg 4. Write out the string x 5 = 
2. Add to the following to its value 5. The counter multiplied by 5 
3. The number in the counter 6. Add a line break 
The key difference between 
a whi 1 e loop and a do whi 1 e 
loop is that the statements in 
the code block come before the 
condition. This means that those 
statements are run once whether 
or not the condition is met. 
If you take a look at the 
condition, it is checking that the 
value of the variable called i is 
less than 1, but that variable has 
already been set to a value of 1. 
Therefore, in this example the 
result is that the 5 times table is 
written out once, even though 
the counter is not less than 1. 
Some people like to write while 
on a separate line from the 
closing curly brace before it.  

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