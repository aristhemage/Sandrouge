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
