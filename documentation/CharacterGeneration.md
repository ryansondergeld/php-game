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

This seems to generate a decent variety of characters.  

The above stats generated are for level 1.  

During generation, each character will have 4 random growth stats also saved to their file.  For example, a character might have growth stats of P.Atk, Luck, Stamina, and Speed in that order.  

When a character levels up they have the following chances to gain a statistic point:
- 40% chance to gain a point in thier first growth stat
- 30% chance to gain a piont in thier second growth stat
- 20% chance to gain a point in their third growth stat
- 10% chance to gain a point in thier fourth growth stat

During the level up, if a stat is already at 15, the additional point will go into the stat from the top down.  For example, if we roleld and were going to put a point in to the third growth stat but it is already 15, we will check the first growth stat.  If that isn't 15 the point will be added there.  If it is 15, we will move on to the 2nd growth stat.  If all growth stats are at 15, the point will go to a random stat that isn't 15.  

Every 3rd level, each character has a 25% chance to score an additional point.  That point will go through the same process as above.  

The maximum level for a character is 15.  

After level 15, the character will store "silent" level ups to 100.  This will be used later on to deterine if a character will retire or not.  
