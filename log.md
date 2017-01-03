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

## Day 3: January 1, 2017

**Today's Progress**

Today, I finished the following:

* Multiple types of complex block (o shape, z, shape and so on)
* Able to rotate complex type of block
* Able to clear line when a line is filled

**Thoughts:** 

I spent quite a lot of time debating if my approach of composing the complex block
with basic block would work or what not. I was fighting myself all along.

Everything turns out to be working in my brain but my body refused to implement
it because I was afraid that my design doesn't cover some of the "edge cases".

This was quite sad to realize afterward but it's one of the weakness I need to 
adjust.

Overall, I enjoyed the work I've done today and felt proud of it!

Tomorrow, I can start look into adding scores and fix some edge case bugs.

**Link to work:** 

https://github.com/rcliao/tetris

## Day 4: January 2, 2016

**Today's Progress**

Today, I worked on improving multiple blocks logic and scoring system, which can
be summarized below:

* Score system
* Color each block differently (for user experience)
* Space to drop the block all the way

**Thoughts:** 

It's quite interesting to realize that color of blocks actually improve the 
game experience by a lot. I'm actually able to enjoy the game myself! I found
myself spending something like hours to play my own game and tried to figure
what would be interesting to add on next.

Although, all the new addons code I did today wasn't planned in the whole system
all at once. In other word, those were easy to add on to existing code. I was
also afrid that these things will be something I had to change in future.

Next thing to do would be adding "next block" and make it easier to move block
around when collision was about to happen.

Of course, I still was interested to apply some software design patter (like
composite) into my current code for better maintainability.

**Link to work:** 

https://github.com/rcliao/tetris

