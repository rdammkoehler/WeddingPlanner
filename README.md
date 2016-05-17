# WeddingPlanner
An programming exercise

Party Planner with GoT characters

Each character has an affinity for other characters. For example, Jamie Lannister always wants to be close to his sister Cersi Lannister. But Jamie has no love for Rob Stark and would perfer that he were not in the room. Simiarly, Rob Stark has no interest in any Lannister.

```
                    |  JL  |  CL  |  RS  |
Jamie Lannister (JL)|  0   |  1   |  10  |
Cersi Lannister (CL)|  1   |  0   |  10  |
Rob Stark (RS)      |  10  |  10  |  0   |
```

So layed out on a grid (the party venue) an stable arrangement might appear as follows;

```
*--------------------------------------------------*
|RS                                                |
|             ########                             |
|             ########                             |
|                                              JLCL|
*------------------------@-------------------------*
```

# Rules of the game

  1) Each character has an zero affinity for themselves
  
  2) Each character has a default affinity for others in the range 1-16. One representing very intimate/familar and 16 representing totally repulsed by the other.
  
  3) Each character moves on space/cell per turn. Movement can be in any direction, but only to an unoccupied space/cell. Characters cannot pass through walls, obsticles, or other party participants.
  
  4) Each character must move once every five (5) cycles of the game
  
  5) The game continues for a fixed number of cycles. Pretend that each cycle is one minute of time. A formal wedding might take 4 hours, so the game would play for 240 cycles

  6) The venue is randomly generated at the begining of the game. The available space (number of cells) must be equal to the number of participants squared plus one (s = p^2+1).
  
  7) The venue can be any shape
  
  8) The venue should contain at least one obstical. A banquet table, pillars, or other furniture. Use '#' to represent those items
  
  9) The venue must have at least one entrance/exit along its boarder denoted with an '@' character
  
  10) Characters start the game by entering through any of the available entrances along the boarder. 
  
  11) Every cycle of the game, characters may move one more space to attempt to be more 'comfortable'
  
  12) At the end of the game, all characters exit the scene through the entrance that they arrived. While exiting they attempt to remain comfortable.
  
  

