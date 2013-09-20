turning-snake
=============

A simple Snake-like game with a twist in 117 lines of F#

Gameplay
--------
You move the "snake" around with the arrow keys.
Everytime you turn you add a "mine" that will kill you if you touch it.
You can wrap around the screen so you only have to watch out for the mines.

The objective is to get as high a score as possible by collecting "apples".
Red apples are worth 1 point and green apples 3 points.
They don't have any effect except increasing your score which you can see in the topleft corner.

Have fun!

Code
----
I wanted to learn F# so I decided to write a simple game using Winforms.
The snake moves around on a 60 by 40 grid which I draw ten times larger.
This simplifies collision detection to simply comparing points.

The game loop is run asynchronously and the main loop is used to get key events.
