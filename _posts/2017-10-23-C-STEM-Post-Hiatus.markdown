Hey, everybody. After a hectic couple of weeks, I'm diving back in. 

I've started learning about JavaScript prototypes, so I'm working on getting a few 'classes' set up so that the shapes can be manipulated.

Many thanks to Simon Sarris' tutorial on making an interactive HTML canvas:
https://simonsarris.com/making-html5-canvas-useful/

This lays out the basic functionality of dragging objects. Because HTML canvases (much like real-life canvases) have no concept of what is on them, they cannot tell you where anything is and thus you are left with no way of easily dragging. Instead, you must create a way to detect if where you click is inside a shape (which is its own class and "knows" its own dimensions), and use that to continuously update the canvas, similar to frames in animation. 

The goal for this week is to finish implementing the simple drag-and-drop used in Mr. Sarris' tutorial. The geometry is a little trickier than just copying it, because not every shape that is added is a rectangle.

Once that's done, I'll start implementing control points in the corners, so that shapes can be distorted in various ways, similar to the current Flash app. An interesting thing I've learned is that it's considerably more efficient to use 1x1 pixel rectangles (maybe larger in the future) to demarcate the control points than it would be to use circles. And, because many of these points might be updated many times a second, we really start getting into serious performance impacts, which would make the interactivity a real drag (pun intended).
