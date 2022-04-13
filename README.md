# Sandrouge
Feb 26th Changes:
- Rearanged the variables in the struct to be more visually pleasing and organized
- Renamed some variables to make them make more sense
- Reworked the entirity of the movement code because I just remembered that I could do it a way better way than before and I was being dumb
- Made and ate a grilled cheese, it was pretty good :D
- Reworked some collision and sprinting mechanics to better fit the new moving system
- Added vInput and hInput in the debug tool

March 2nd Changes:
- Updated the player sprite to the idle sprite given by Oreo
- Made the room background light blue to better show the new sprite
- fixed an inventory logic bug
- Doomed my mortal enemy to ten years of horse plinko.
- added a "Radius" stat to the player, it relates to how close the player needs to be before they are able to interact with objects and monsters (Excluding ranged attacks and actions). Not yet implemented other than a visual circle that goes around the player (Temp Ofc).
- added a stats struct to the parent block to add HP, blast risistance, and seethrough (like glass, for monsters).
- Organized the files a little.
- Started working on a state machine and implimented it a little
- used it in combonation with an unused, now used, variable, to fix a food and energy bug where the player could not use energy or food by hugging a wall.
- Added a debug block for testing (Not currently implemented with anything
- Changed some debug things around.

March 9th Changes:
- Added a two parent objects to deal with items
- Added a functional item pickup system with "Item crawling"
- Added text that pops up when you collect an item (No data is currently stored when you do so)
- Found a cool rock
- Added yet another changeable stat with the player called pickupRange, deals with the range you can pick up
  items
- Added a counter that counts how many items you picked up

March 10th Changes:
- Added A Temp folder in sprites and moved colours folder in there
- Added a Temp inventory frame sprite
- Added an Inventory Group
- Added an Inventory handler that deals with practically everything inventory visually (and some internally)
- Although not currently functional due to there not being items in the game, an item counter was added. 
  0 and negative numbers do show, but that's due to the fact that I simply haven't gotten to that yet.
- Kicked the cool rock around, it was cool.
- Added Another debug tool dedicated to inventory (In the room)
- Removed the default debug tool from the room to see Inventory stuff (I will bring it back with code making the
  text be on the bottom left instead later, if you want it in for some reason, it still functions, so just
  drag it in the room)
  
  March 11th
- Made it so you can't go under 0 items
- Made it so it didn't show the amount of items the player has if they run out (0 items)
- Added a thing that detects what you inventory slot you have selected. (Switch using the scrollwheel)
- Made it so the selected number doesn't underflow or overflow below 0 or above the max player inventory slots
- Reflected the selected inventory fram visually.
- Moved the origin for the inventory frame sprite from top left to middle center for a scaling thing, breaking
  absolutley eveything visually
- Fixed the issue and added scaling to the text too to compliment the look even more.
- Added a tileset folder and added Oreo's tileset
- The rock started to kick back
- Added a grass sprite that corrupted the entire project somehow 
  (Thank god for constant backups, nothing was lost)
- Fixed everything, and got the grass sprite working
- Updated Oreo's Tileset slightly to better fit with itself (Sizing issue with the turns)
- Added a scr_item script that makes it so the item actually goes into the inventory properly when picked up.
  Things without durability (Like wood) are stackable, and things with durability (Like tools) are not. This
  can be changed, but it's how it's set for now.
- Began working on a thing that shows the item visually, emphasis on began.

March 11th part 2 
- Added a timer between item pickups so if you don't pick up an item in a certain amount of time, the amount
  counter resets. (Bad explination I know, but I can show what I mean)
- Updated scr_item() to better fit things and remove redundancies.
- Started to fail to fight back from the rock
- Made it so items draw on the screen in the inventory
- Added an item script


March 12th
- Added a debug sword called the stick of gaming
- Added a debug pickaxe called the pickaxe of gaming
- Identified a bug where the item counter was going up, regardless if the items are different are not
- Added a "Type" variable to the inventory struct.
- Got beat up by the cool rock :(
- Added a few things to both the player and pItem to fix the bug where picking up an item after your inventory
  was full would crash the game. (Not workarounds, just missing code that is now added)
- Reorganized the test room to better reflect what an actual room setup would look like 
  (Look at room editor layers)
- Lowered the players hitbox so players can squeeze through things that they look like they can
- Added yet another changeable player stat (yay) called swordAOE.

March 13th
- Screamed at functions, graphs, and more pain unessasarily
- Added a slash effect and a cursor that surrounds the player
- Started to train to fight back and regain my honour
- Added the mobs given by lucid in the game sprite wise
- Added the slime to the game and added basic AI, Chase AI, and Lunge AI (Although they can currently
  phase through walls)
  
March 30th through April 13th
	-Updated the Stick of gaming sprite because I thought it was ugly. 
	Still a debug item for my amusement and testing, I just like the new sprite.
	-Added some functionality to block breaking animations
	-Made the breaking animation accurate to health of the block
	-Revalued tools damLow and damHigh to just efficiency, as tools are not weapons.
	-Updated inventory struct to reflect this
  	-Updated various other places to reflect this
	-Stood the test of time against the allmighty rock... Won by the skin of my teeth.
	-Made it so you can break the block, it appears as an item, and is pickupable
	-Noted the very noticable bug where when picking up a block item, it is huge. Due to
	 how I programmed things, it's much harder to fix this issue than you would think.
