# Formulas

## Damage Caculations for single opponent
Atk = P.Atk for Physical Attacks or M.Atk for magic attacks

Base.Damage = (Atk x 2) - (Def x 0.7)  
Type.Multiplier = 1.5(strength), 1.0(neutral), or 0.5(weakness)  
Luck.Multiplier = 1 + (Random number between -5 and 5 / 100) + (Luck / 150)   
Critical.Bonus = (Atk / 2) + (Luck / 2)  
Critical.Check = (Luck - 2) / 15 vs random number between 0 and 15.  (~86% chance maximum)   
Final.Damage = (Base.Damage x Type.Multiplier x Luck.Multiplier + Critical.Bonus) / 2  

All damage is clamped between 1 and 15 and will be an integer value.  

## Damage calculations for multiple enemies
For attacks that target multiple enemies, a slightly different formula is used for the base damage and the critical damage:
Base.Damage = (Atk x 1.8) - (Def x 0.7)
Critical.Bonus = (Atk / 3) + (Luck / 3)  

The Type.Multiplier, Luck.Multiplier, and Critical.Check will need to be performed by each enemy the attack hits.  This is still true if the attack targets the same enemy more than once.  


