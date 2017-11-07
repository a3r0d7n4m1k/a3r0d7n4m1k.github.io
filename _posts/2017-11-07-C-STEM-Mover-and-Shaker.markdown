Whoo! So it's not super pretty, but it works! These past couple of weeks have been dedicated to getting multiple shapes to be added to the canvas and dragged around the screen.

It was a little difficult to keep track because the shapes are drawn by connecting point to point, but the representation of these points change a bit throughout the code. For example, there is a point object, but the coordinates of a given point are written in as strings which then must be parsed as an int.

That was actually the biggest issue for a while. Because the x and y values of the points were strings, the movement wasn't added but concatenated, so even the slightest bit of dragging sent the entire shape completely off the screen.

Now that it's up, I just need to make sure I've covered every test case and then I'll move on to deleting things.

Deleting might be tricky because while the shape itself might be easy to delete, it'll be hard to remove the shape's points from the shape form. I also really want to clean up the application itself so it looks a little nicer.
