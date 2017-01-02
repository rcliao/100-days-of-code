# 100 Days Of Code - Log

## Day 1: December 30, 2016

**Today's Progress**

I made a simple index.html with canvas to handle Tetris game board does the following:

* Have basic game loop
* Have a base block dropping from the top
* Stop the block when it hits the bottom) and spawn new block
* Handle basic input from the keyboard input

**Thoughts:** 

Build everything from the start is quite ... painful when there is no framework
to support some common actions (such handling inputs and game loop). This generally
implies the main responbility goes down to me.

**Link to work:** 

https://github.com/rcliao/tetris

## Day 2: December 31, 2016

**Today's Progress**

I continue to work on the collision logic part today.

First thing I did today was to split out the code into multiple files. To do so,
I include Babel and Webpack for building ES6 code into modern browser competitable
code.

And then, I research into how to make a better game logic by replacing setInterval
into window.requestAnimationFrame.

Furthermore, I did some improvement onto the collision to be better with single
block dropping (including boundary checking and so on).

**Thoughts:** 

Collision is quite tricky to implement when I have multiple places to move the 
block. Right now, there are two move method being invoked on each update run,
this implies that the move method can cause different level of bugs.

I probably should simplify the update method to handle input better.

And tomorrow, I'm hoping to work on different type of blocks -- this is going to
be tricky as the logic to check different shape becomes different.

**Link to work:** 

https://github.com/rcliao/tetris

