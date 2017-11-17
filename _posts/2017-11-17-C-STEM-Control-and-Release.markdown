I think I'm going to stop trying to come up with cute names for these posts because this one barely makes sense.

Point is (no pun intended) that I've gotten deletion for any object and control points working.

I had an issue with deletion where a selected object would get slightly darker, because another identical object was being created in the exact same spot. When you went to delete this object (you can only delete the selected object), the trace would be left over and not wiped off until a new object was drawn or a different object was selected. This posed problems when deleting the only object on the page, because there was nothing to cause the canvas to wipe itself clean.

The next thing that I did was make a working control point. Because I'd already implemented shapes as a set of Point objects to demark each corner, it was fairly easy to extend the implementation that I had for moving Shapes around to the corners. I managed the whole thing in around 20 minutes (which lowkey surprised me; I thought it'd take a bit longer). 

Now, I'm not really sure what to do next:

 - Start making the page look nice and usable, which means adding background images of graffiti that can be scrolled through. (Estimated: Medium)

 - Find a way to group the html elements of the coordinates for a Shape's Points and add a way to delete the form elements of a deleted Shape. (Estimated: Easy-Medium)

 - Add a way to change a point by changing the corresponding html input. (Estimated: Hard, given current implementation)

 - Start implementing polar coordinates and bendy shapes (Estimated: I'd rather not do this right now)

Talk soon!