# instrucciones

In example A, you can see three elements stacked like a simple tower. Fascinating, isn’t it? This is block building 101. Congratulations!

You can use the static value for simple, single-column layouts where each element must sit on top of the next one. If you want to start shifting those elements around using offset properties such as top, right, bottom, and left, you’re out of luck. These properties are unavailable to a static element. In fact, a static element can’t even create a new coordinate system for child elements. Wait. What? You lost me at coordinate system. Roger that, Roger. Let’s explain using the relative value.

Relatively positioned elements behave just like statically positioned elements; they play well with others, stack nicely, and don’t cause a ruckus. Hard to believe, right? Take a look at our previous example. This time, we’ve applied the relative value:

#box_1 {
	position: relative;
	width: 200px;
	height: 200px;
	background: #ee3e64;
}

#box_2 {
	position: relative;
	width: 200px;
	height: 200px;
	background: #44accf;
}

#box_3 {
	position: relative;
	width: 200px;
	height: 200px;
	background: #b7d84b;
}
