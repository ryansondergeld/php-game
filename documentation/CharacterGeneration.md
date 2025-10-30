# Generation  

Initially the unit starts with all stats at 7.  

Follow this process:  
- We will keep an extra pool of 9 points
- Decrement 1 from 3 random stats (could be the same stat 3 times)
- Add 3 to 1 random stat (could be the same stat we decremented 3 times) 
- Decrement 1 from 2 random stats (could be the same stat 2 times)  
- Add 2 to 1 random stat (could be the same stat we decremented 2 times)  
- Decrement 1 from 1 random stat
- Add 1 to 1 random stat 
- Look through each stat.  If any stats are less than 3 add the required number of points to that stat to make it three.  Decrement these points from the pool.  
- Decrement 1 from 3 random stats (could be the same stat 3 times)  
- Add 3 to 1 random stat (could be the same stat we decremented 3 times)  
- There is a 1 in 4 chance of one of the following:
  - Add 6 points from the pool to 1 random stat 
  - Add 3 points from the pool to 2 random stats (6 points total from the pool)  
  - Add 2 points from the pool to 3 random stats (6 points total from the pool)  
  - Add 1 point from the pool to 6 random stats (6 points total from the pool)
- Add any remaining points in the pool 1 by 1 to a random stat
