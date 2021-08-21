## How many ways are there to tile `2*n` size rectangle with `2*1` tiles? (n is even)
---
The main observation is here we can 
* either place a tile vertically covering `2*1` area 
* or place 2 tiles horizontally covering `2*2` area.
  
There is one way to tile `2*1` size rectangle
* Placing a tile vertically.
  
and 2 ways to tile `2*2` size rectangle-
* Placing two tiles vertically.
* Placing two tiles.
  
Suppose there are $f(n)$ ways to tile the rectangles.

so  `f(n) = f(n-1) + f(n-2)`

The base cases `f(1) = 1` and `f(2) = 2`  


It seems like Fibonacci right? Exactly! the answer is from the Fibonacci series.
So we just need to write a code for Fibonacci.
