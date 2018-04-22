# instrucciones

_basado en el documento alist_

For starters, we can adjust a relatively positioned element with offset properties: top, right, bottom, and left. Using the markup from our previous example, let’s add an offset position to #box_2:

#box_2 {
	position: relative;
	left: 200px;
	width: 200px;
	height: 200px;
	background: #44accf;
}
Example C shows this relative positioning in action. Our three blocks are stacked up nicely, but this time the blue block (#box_2) is pushed out 200 pixels from the left. This is where we start to bend the law of gravity to our will. The blue block is still in the flow of the document—elements are stacking one on top of the other—but notice the green block (#box_3) on the bottom. It’s sitting underneath the blue block, even though the blue block isn’t directly above it. When you use the offset property to shift a relatively positioned element, it doesn’t affect the element(s) that follow. The green box is still positioned as if the blue box were in its non-offset position. Try that with your alphabet block tower.
