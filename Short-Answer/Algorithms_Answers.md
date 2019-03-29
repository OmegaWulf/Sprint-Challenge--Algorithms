Add your answers to the Algorithms exercises here.
a) This would be O(n). It's technicaly O(n + 1) but we can remove the constant. The while loop runs until a is greater than 
    n^3 and we're incrementing a by n^2 each time. This means it's going to take n number of times until a == n^3 and then
    after one more loop, the while statement will be fulfilled. 
    
    For example, if n = 3, the loop runs until a < 27 and increments by 9 each loop. At loop 3, a == 27 but we need one more 
    loop for it to break the while loop. 
    
b) This would be O(n^3). 3 nested for-loops have a worst-case runtime of O(n^3). The last for-loop is running at a constant
    time since it only runs 10 times per loop. Constant time gets rounded away so we're left with O(n^3). 

c) This is O(n). The function keeps recursively calling itself until n == 0 and decrementing by 1. So an N of 100 would run 
    the function 100 times. 
    
    
#2 

Since a building always has an ordered number of floors, go to the middle floor and throw an egg. If it breaks then we 
know f is in the bottom half of the floors. So we divide the bottom half and throw the egg. Repeat until we have f. 


while 
    