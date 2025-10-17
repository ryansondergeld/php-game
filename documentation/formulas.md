# Formulas

## P.Atk
The goal is to balance the atacker's power, the defenders resistance and some variance.  

P.Damage = ((P.Atk x 4 - P.Def x 2) x Type.Multiplier x Luck.Multiplier + Critical.bonus

- Use the character's stats, multiplying P.Atk x 4 and P.Def by 2 gives more impact to the formula.  
- Type.Multiplier factors in any strengths or weaknesses
  - 1.5 might be a good multiplier for a strength (strong against type)
  - 1.0 would be neutral and doesn't affect the damage
  - 0.5 might be a good multiplier for a weakness (weak against type)
- Luck.Multiplier would factor in a random amount
  - Example:  (Random number between -5 and 5 divided by 100) + (Attacker's luck divided by 150)
  - The above formula should give a +/- 5% random factor to the values
- Critical bonus (occurs if a critical hit happens)
  - Critical chance formula: (Luck of attacker / 15)
  - Above means a 15 = 100% chance of critical where a 7/15 = 46% chance
  - Critical bonus is the damage added, like +20

## M.Atk

M.Damage = ((M.Atk x 5 - M.Def x 3) x Type.Multiplier x Luck Multiplier + Critical.Bonus

- This formula is slightly higher and would balance the lower stamina values.  
- Type.Multiplier, Luck.Multiplier and Critical.Bonus operate the same as the physical damage formula.

## HP Calculation  
Max HP = 100 x (Stamina x 20)

This means a stamina of 0 = 100 HP
A stamina of 15 = 400 HP


