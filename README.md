Did you really need to make that turn?
======================================

A simple Snake-like game with a twist in 120 lines of F#

*by Andreas From*

Gameplay
--------
You move the blue "snake" around with the arrow keys.
Everytime you turn you add a "mine" that will kill you if you touch it.
You can wrap around the screen so you only have to watch out for the mines.
If you touch them, you get to see your final score and then the game starts over.

The objective is to get as high a score as possible by collecting "apples".
Red apples are worth 1 point and green apples 3 points.
They don't have any effect except increasing your score which you can see in the topleft corner.

Have fun!

![Image of the gameplay](http://i.imgur.com/5N7F13J.png)

Code
----
I wanted to learn F# so I decided to write a simple game using Winforms.
The snake moves around on a 60 by 40 grid which I draw ten times larger.
This simplifies collision detection to simply comparing points.

The game loop is run asynchronously and the main loop is used to get key events.

Download
--------
Playing the game requires either the [F# 2.0 Runtime for Windows](http://www.microsoft.com/en-us/download/details.aspx?id=13450)
or Mono for Mac and Linux with support for F# 2.0.

Then you should be able to download and run [Snake.exe](https://www.dropbox.com/s/2g5t7llicfqq53a/Snake.exe)
