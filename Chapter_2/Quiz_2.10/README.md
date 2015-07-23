#2.10 — Chapter 2 comprehensive quiz
>Note: When using symbolic constants to replace magic numbers, try to use *const* instead of #define  

Comprehensive quiz

**Question 1**

Why are symbolic constants usually a better choice than literal constants? Why are const symbolic constants usually a better choice than #defined symbolic constants?

**Question 2**

Pick the appropriate data type for a variable in each of the following situations. Be as specific as possible. If the answer is an integer, pick a specific integer type (e.g. int16_t) based on range. If the variable should be unsigned or const, say so. Favor signed numbers over unsigned numbers.

a) The age of the user (in years)
b) Whether the user wants color or not
c) pi (3.14159265)
d) The number of pages in a textbook
e) The price of a stock in dollars (to 2 decimal places)
f) How many times you’ve blinked since you were born (note: answer is in the millions)
g) A user selecting an option from a menu by letter
h) The year someone was born

**Question 3**

Write the following program: The user is asked to enter 2 floating point numbers (use doubles). The user is then asked to enter one of the following mathematical symbols: +, -, *, or /. The program computes the answer on the two numbers the user entered and prints the results. If the user enters an invalid symbol, the program should print nothing.

Example of program:

Enter a double value: 7  
Enter a second double value: 5  
Enter one of the following: +, -, *, or /: *  
7 * 5 is 35  
Hint: You can check if the user has entered a plus symbol using an if statement, covered in section 2.6 -- Boolean values.

**Question 4**

This one is a little more challenging. Write a short program to simulate a ball being dropped off of a tower. To start, the user should be asked for the initial height of the tower in meters. Assume normal gravity (9.8 m/s2), and that the ball has no initial velocity. Have the program output the height of the ball above the ground after 0, 1, 2, 3, 4, and 5 seconds. The ball should not go underneath the ground (height 0).

Your program should include a header file named constants.h that includes a namespace called myConstants. In the myConstants namespace, define a symbolic constant to hold the value of gravity (9.8 meters per second). See section 2.9 -- Symbolic constants and the const keyword for a reminder on how to do this.

Use a function to calculate the height of the ball after x seconds. The function can calculate how far the ball has fallen after x seconds using the following formula: distance fallen = gravity_constant * x_seconds2 / 2

Sample output:

Enter the initial height of the tower in meters: 100  
At 0 seconds, the ball is at height: 100 meters  
At 1 seconds, the ball is at height: 95.1 meters  
At 2 seconds, the ball is at height: 80.4 meters  
At 3 seconds, the ball is at height: 55.9 meters  
At 4 seconds, the ball is at height: 21.6 meters  
At 5 seconds, the ball is at height: 0 meters  