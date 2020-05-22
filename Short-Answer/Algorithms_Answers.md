#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) I would say that this is a runtime of O(n). My reasoning is that while 'a' is less than 3n (O(n)), 'a' will be 'a' + 2N (O(n)). As long as 'a' is less than 3n the loop will run, meaning that this is O(n).


b) I think that this runtime is O(nlogn) because in a range of n, while 'j' is less than 'n' it will multiply by 2 until it reaches the point where it is larger than n, anytime I see something multiplying by 2 I think logn because we are closing that gap faster and faster, like Binary sort. So, logn times n times another n. O(2nlogn) take out the constant and O(nlogn).


c) My answer, O(n). The first two lines of the function are O(1) because it's saying if this condition, return this constant (Base Case). Else, 2 + function(n - 1) (Recursive Case). Since the only option is to recurse if bunnies isn't 0, n would grow linearly. 

## Exercise II  

n = number of floors  
egg = eggs dropped  
f = floor where eggs can be safely dropped from    

I assume the floors are from smallest to largest.  

There are two ways to do this, each with a different runtime complexity. First, if I go floor by floor until I find the floor where I can drop eggs from (for i in n, egg + 1) n would grow at a linear rate. This is O(n).  

The best way I can do this would be to use binary search instead, resulting in a runtime of O(logn). I would do this by taking the number of floors and finding the middle, n // 2 , then I would drop and egg. If the egg broke, I would know I need to go lower to find f, if the egg didn't break I would need to go higher to find f. This is O(logn) because I quickly approach floor f. 

