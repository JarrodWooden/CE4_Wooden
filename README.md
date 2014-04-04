CE4_Wooden
==========

First Assignment with Prism and Assembly Coding


Computer Exercise Four is about learning how to right code in assembly.

#Simple Memory Manipulation

The first program that we were tasked with to write was Simple Memory Manipulation

The objectives that needed to met are as follows:

      Write a program that stores the value $9 in location $B0, $8 in $C4 and $B in $CB. (Target program end: $11)
      
A picture of what I wrote for the code is below and the code worked!!

![alt text](https://raw.githubusercontent.com/JarrodWooden/CE4_Wooden/master/MemoryManipulation.PNG "Code written for the Simple Memory Manipulation")

Pretty easy right?

#Mathematics

The mathematics code was more difficult but still pretty basic

The Objectives for this code are below:

      Write a program that retrieves a value from location $B0, doubles it, and subtracts 4.  
      The result should be output to Port 2. You will need to place a positive test value in this location 
      prior to running the program.  Although RAM is volatile and you normally cannot directly change values in 
      it without having a program do it, you can in this simulation by checking “Allowed RAM values to be edited” 
      in the Programming Wizard.  (Target program end: $0C)
      
The Picture of how I solved the code is below

![alt text](https://raw.githubusercontent.com/JarrodWooden/CE4_Wooden/master/MathematicsPicture.PNG "Code written for Mathematics")

Still pretty easy... but I guess I'll kinda give a description of how I did this one if future me gets dumb and doesn't
remember how to do this... ugh.

--First Load the data in the RAM adress B0 then add the data in BO to the accumulator in order to double the number.

--Next! Then store the number in location B1 so that we don't lose it

--Load up the number four to the accumulator and NEG it to get negative four

--Add the accumulator to the doubled number we have in location B0

--output the result to Pin2 and go into an infinate loop to stop

Okay Jarrod... so frustrating.

#Loop

The Loop code was the most difficult objectives to achieve

The objectives for the program are below:

      Write a program that starts by reading what is on Input Port 3 and then displaying that on Output Port 0.  
      One less than that should then display on Port 1 and one less than what is on Port 1 will display on Port 2.  
      The program then decrements what is on Port 0, then decrements what is on Port 1, then decrements what is 
      on Port 2.  This process is continued in an infinite loop (i.e. If Input Port 3 contains a ‘2’ , Ports 0-2 
      will show 2,1,0, respectively.  The 2, 1, 0 will then change to 1,0,F, then 0, F, E, and so on). 
      (Target program end: $10)
      
The picture of code that shows how I implemented the objectives are below

![alt text](https://raw.githubusercontent.com/JarrodWooden/CE4_Wooden/master/LoopsPic.PNG "Code written for Loop")

A video of a click by click walkthrough of the program is above.

Here's a text walkthrough.

--First I loaded -1 into the accumulator and stored it at adress B4

--Then I recieved the input from pin 3

--I entered the loop, first by sending the value in the accumulator to pin 0

--Then added -1 to the accumulator and sent that to output pin 1

--I stored that value at adress B0 to use at the end of the loop

--Then added -1 to the accumulator and sent that to output pin 2

--Then added -1 to the accumulator and sent that to output pin 3 (see a pattern?)

--I loaded up num (adress B0) back to the accumulator and restarted this loop

MEANING THAT the number in B0 that was loaded back to the accumulator was the value of the number we started with
minus one to use for the next run through the loop.

#Done

thank you for reading my read me! Have a great air force day!
