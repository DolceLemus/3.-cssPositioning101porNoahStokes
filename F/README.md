# instrucciones

_basado en el documento alist_

If the relative value acts like Superman, then the absolute value mirrors Inception—a place where you design your own world. Unlike the static and relative values, an absolutely positioned element is removed from the normal flow. This means you can put it anywhere, and it won’t affect or be affected by any other element in the flow. Think of it as an element with a giant strip of velcro on its back. Just tell it where to stick and it sticks. Exactly like the relative value, absolutely positioned elements respond to offset properties for positioning. You can set an element to top: 100px and left: 200px; and that element will sit exactly 100px from the top and 200px from the left of the document. Let’s look at an example using four elements:

#box_1 {
	position: absolute;
	top: 0;
	left: 0;
	width: 200px;
	height: 200px;
	background: #ee3e64;
}
#box_2 {
	position: absolute;
	top: 0;
	right: 0;
	width: 200px;
	height: 200px;
	background: #44accf;
}
#box_3 {
	position: absolute;
	bottom: 0;
	left: 0;
	width: 200px;
	height: 200px;
	background: #b7d84b;
}
#box_4 {
	position: absolute;
	bottom: 0;
	right: 0;
	width: 200px;
	height: 200px;
	background: #ebde52;
}
Example E shows four boxes, each in a corner of the browser window. Since we set each box’s position value to absolute, we’ve essentially velcroed a box to each corner of our browser window. As you resize the browser, those boxes will stay in their respective corners. If you shrink the browser window so that the boxes overlap, you’ll notice that there is no interaction at all—that’s because they’re out of the document’s normal flow.

**Just like relative elements, absolute elements create a new coordinate system for child elements. Example F extends Example E, with an orange element set inside each box. Notice the offset coordinates are in respect to each parent element.**
