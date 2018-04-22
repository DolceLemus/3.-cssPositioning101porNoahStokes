# instrucciones

_basado en el documento alist_

The static and relative position properties behave like your childhood blocks—they stack as you would expect. Note that static is the default position value of an element, should you fail to apply any other value. If you have three statically positioned elements in your code, they will stack one on top of the next, as you might expect. Let’s take a look at an example with three elements, all with a position value of static:

#box_1 {
	position: static;
	width: 200px;
	height: 200px;
	background: #ee3e64;
}

#box_2 {
	position: static;
	width: 200px;
	height: 200px;
	background: #44accf;
}

#box_3 {
	position: static;
	width: 200px;
	height: 200px;
	background: #b7d84b;
}
In example A, you can see three elements stacked like a simple tower. Fascinating, isn’t it? This is block building 101. Congratulations!
