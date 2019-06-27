# pythonc-challenge-01
this is a challenge for students learning python.


01  Generate the random outcome of flipping a coin using Python. Use the letter 'H' for Heads, and the letter 'T' for Tails. 
 
Your output should be: 

 ```
  H 
  Or 
  T 
 ```

02  Simulate the flipping of the coin until I throw a 'T' (Tails). 
 
  Your output should be: 

```
  T 

  Or 
  H 
  H 
  H 
  T 
  ```
 
03 Let a user enter an integer that is used to determine the number of coin flips you program will make. 
  
So if the user enters 20, your code will simulate 20 coin flips. At the end of your program, it will display a summary of the frequency of Heads ('H') and Tails ('T') that were flipped. 
Here is some start code: 
```python
import random 
coin = ["H", "T"] 
targetFlips = int(input("Enter number of flips: ")) 
totalFlips = 0 
# declare any other variables here 
while totalFlips < targetFlips: 
  # your code here 
  totalFlips += 1 
```
Output  for 5 should look like this: 
```
H 
T 
H 
T 
T 
T 
T 
T 
Number of flips 8 
```
 
 
04  Add the following functionality to your existing coin flip program: 
Ability to target a particular side of the coin ('H' or 'T') 
Ability to target the number of flips of the target side in a row, for the program to exit (e.g. 10 'Heads' in a row to exit) 
A timer using timeit, to determine how long the program took (see example below) 
(Here is some source code to get started) 

'''python
import random 
import timeit 
  
coin = ["H", "T"] 
  
sideToTarget = input("Target Heads or Tails? Enter 'H' or 'T': ") 
frequencyToTarget = int(input("How many to target in a row: ")) 
  
targetReached = False 
totalFlips = 0 
# declare other variables here 
  
# main loop: 
timeStarted = timeit.default_timer() 
while not (targetReached): 
    # ...code to process flip 
    totalFlips += 1 
  
print("Target reached in", totalFlips, "flip(s).") 
elapsed = timeit.default_timer() - timeStarted 
print("Program took " + "{0:.2f}".format(round(elapsed, 2)) + " seconds.") 
```
